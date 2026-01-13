# AppStoreConnect.Net.Api.BuildBundlesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildBundlesAppClipDomainCacheStatusGetToOneRelated**](BuildBundlesApi.md#buildbundlesappclipdomaincachestatusgettoonerelated) | **GET** /v1/buildBundles/{id}/appClipDomainCacheStatus |  |
| [**BuildBundlesAppClipDomainCacheStatusGetToOneRelationship**](BuildBundlesApi.md#buildbundlesappclipdomaincachestatusgettoonerelationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainCacheStatus |  |
| [**BuildBundlesAppClipDomainDebugStatusGetToOneRelated**](BuildBundlesApi.md#buildbundlesappclipdomaindebugstatusgettoonerelated) | **GET** /v1/buildBundles/{id}/appClipDomainDebugStatus |  |
| [**BuildBundlesAppClipDomainDebugStatusGetToOneRelationship**](BuildBundlesApi.md#buildbundlesappclipdomaindebugstatusgettoonerelationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainDebugStatus |  |
| [**BuildBundlesBetaAppClipInvocationsGetToManyRelated**](BuildBundlesApi.md#buildbundlesbetaappclipinvocationsgettomanyrelated) | **GET** /v1/buildBundles/{id}/betaAppClipInvocations |  |
| [**BuildBundlesBetaAppClipInvocationsGetToManyRelationship**](BuildBundlesApi.md#buildbundlesbetaappclipinvocationsgettomanyrelationship) | **GET** /v1/buildBundles/{id}/relationships/betaAppClipInvocations |  |
| [**BuildBundlesBuildBundleFileSizesGetToManyRelated**](BuildBundlesApi.md#buildbundlesbuildbundlefilesizesgettomanyrelated) | **GET** /v1/buildBundles/{id}/buildBundleFileSizes |  |
| [**BuildBundlesBuildBundleFileSizesGetToManyRelationship**](BuildBundlesApi.md#buildbundlesbuildbundlefilesizesgettomanyrelationship) | **GET** /v1/buildBundles/{id}/relationships/buildBundleFileSizes |  |

<a id="buildbundlesappclipdomaincachestatusgettoonerelated"></a>
# **BuildBundlesAppClipDomainCacheStatusGetToOneRelated**
> AppClipDomainStatusResponse BuildBundlesAppClipDomainCacheStatusGetToOneRelated (string id, List<string> fieldsAppClipDomainStatuses = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipDomainStatuses** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDomainStatuses | [optional]  |

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | Single AppClipDomainStatus |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesappclipdomaincachestatusgettoonerelationship"></a>
# **BuildBundlesAppClipDomainCacheStatusGetToOneRelationship**
> BuildBundleAppClipDomainCacheStatusLinkageResponse BuildBundlesAppClipDomainCacheStatusGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBundleAppClipDomainCacheStatusLinkageResponse**](BuildBundleAppClipDomainCacheStatusLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | Related linkage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesappclipdomaindebugstatusgettoonerelated"></a>
# **BuildBundlesAppClipDomainDebugStatusGetToOneRelated**
> AppClipDomainStatusResponse BuildBundlesAppClipDomainDebugStatusGetToOneRelated (string id, List<string> fieldsAppClipDomainStatuses = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipDomainStatuses** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDomainStatuses | [optional]  |

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | Single AppClipDomainStatus |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesappclipdomaindebugstatusgettoonerelationship"></a>
# **BuildBundlesAppClipDomainDebugStatusGetToOneRelationship**
> BuildBundleAppClipDomainDebugStatusLinkageResponse BuildBundlesAppClipDomainDebugStatusGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBundleAppClipDomainDebugStatusLinkageResponse**](BuildBundleAppClipDomainDebugStatusLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | Related linkage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesbetaappclipinvocationsgettomanyrelated"></a>
# **BuildBundlesBetaAppClipInvocationsGetToManyRelated**
> BetaAppClipInvocationsResponse BuildBundlesBetaAppClipInvocationsGetToManyRelated (string id, List<string> fieldsBetaAppClipInvocations = null, List<string> fieldsBetaAppClipInvocationLocalizations = null, int limit = null, List<string> include = null, int limitBetaAppClipInvocationLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppClipInvocations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppClipInvocations | [optional]  |
| **fieldsBetaAppClipInvocationLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppClipInvocationLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaAppClipInvocationLocalizations** | **int** | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) | [optional]  |

### Return type

[**BetaAppClipInvocationsResponse**](BetaAppClipInvocationsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of BetaAppClipInvocations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesbetaappclipinvocationsgettomanyrelationship"></a>
# **BuildBundlesBetaAppClipInvocationsGetToManyRelationship**
> BuildBundleBetaAppClipInvocationsLinkagesResponse BuildBundlesBetaAppClipInvocationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildBundleBetaAppClipInvocationsLinkagesResponse**](BuildBundleBetaAppClipInvocationsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of related linkages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesbuildbundlefilesizesgettomanyrelated"></a>
# **BuildBundlesBuildBundleFileSizesGetToManyRelated**
> BuildBundleFileSizesResponse BuildBundlesBuildBundleFileSizesGetToManyRelated (string id, List<string> fieldsBuildBundleFileSizes = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildBundleFileSizes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBundleFileSizes | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildBundleFileSizesResponse**](BuildBundleFileSizesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of BuildBundleFileSizes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbundlesbuildbundlefilesizesgettomanyrelationship"></a>
# **BuildBundlesBuildBundleFileSizesGetToManyRelationship**
> BuildBundleBuildBundleFileSizesLinkagesResponse BuildBundlesBuildBundleFileSizesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildBundleBuildBundleFileSizesLinkagesResponse**](BuildBundleBuildBundleFileSizesLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of related linkages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

