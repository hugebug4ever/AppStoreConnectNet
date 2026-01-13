# AppStoreConnect.Net.Api.BetaBuildLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaBuildLocalizationsBuildGetToOneRelated**](BetaBuildLocalizationsApi.md#betabuildlocalizationsbuildgettoonerelated) | **GET** /v1/betaBuildLocalizations/{id}/build |  |
| [**BetaBuildLocalizationsBuildGetToOneRelationship**](BetaBuildLocalizationsApi.md#betabuildlocalizationsbuildgettoonerelationship) | **GET** /v1/betaBuildLocalizations/{id}/relationships/build |  |
| [**BetaBuildLocalizationsCreateInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationscreateinstance) | **POST** /v1/betaBuildLocalizations |  |
| [**BetaBuildLocalizationsDeleteInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsdeleteinstance) | **DELETE** /v1/betaBuildLocalizations/{id} |  |
| [**BetaBuildLocalizationsGetCollection**](BetaBuildLocalizationsApi.md#betabuildlocalizationsgetcollection) | **GET** /v1/betaBuildLocalizations |  |
| [**BetaBuildLocalizationsGetInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsgetinstance) | **GET** /v1/betaBuildLocalizations/{id} |  |
| [**BetaBuildLocalizationsUpdateInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsupdateinstance) | **PATCH** /v1/betaBuildLocalizations/{id} |  |

<a id="betabuildlocalizationsbuildgettoonerelated"></a>
# **BetaBuildLocalizationsBuildGetToOneRelated**
> BuildWithoutIncludesResponse BetaBuildLocalizationsBuildGetToOneRelated (string id, List<string> fieldsBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |

### Return type

[**BuildWithoutIncludesResponse**](BuildWithoutIncludesResponse.md)

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
| **200** | Single Build with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betabuildlocalizationsbuildgettoonerelationship"></a>
# **BetaBuildLocalizationsBuildGetToOneRelationship**
> BetaBuildLocalizationBuildLinkageResponse BetaBuildLocalizationsBuildGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaBuildLocalizationBuildLinkageResponse**](BetaBuildLocalizationBuildLinkageResponse.md)

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

<a id="betabuildlocalizationscreateinstance"></a>
# **BetaBuildLocalizationsCreateInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsCreateInstance (BetaBuildLocalizationCreateRequest betaBuildLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaBuildLocalizationCreateRequest** | [**BetaBuildLocalizationCreateRequest**](BetaBuildLocalizationCreateRequest.md) | BetaBuildLocalization representation |  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **201** | Single BetaBuildLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betabuildlocalizationsdeleteinstance"></a>
# **BetaBuildLocalizationsDeleteInstance**
> void BetaBuildLocalizationsDeleteInstance (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

void (empty response body)

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
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betabuildlocalizationsgetcollection"></a>
# **BetaBuildLocalizationsGetCollection**
> BetaBuildLocalizationsResponse BetaBuildLocalizationsGetCollection (List<string> filterLocale = null, List<string> filterBuild = null, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsBuilds = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterLocale** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **filterBuild** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;build&#39; | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaBuildLocalizationsResponse**](BetaBuildLocalizationsResponse.md)

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
| **200** | List of BetaBuildLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betabuildlocalizationsgetinstance"></a>
# **BetaBuildLocalizationsGetInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsGetInstance (string id, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsBuilds = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

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
| **200** | Single BetaBuildLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betabuildlocalizationsupdateinstance"></a>
# **BetaBuildLocalizationsUpdateInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsUpdateInstance (string id, BetaBuildLocalizationUpdateRequest betaBuildLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaBuildLocalizationUpdateRequest** | [**BetaBuildLocalizationUpdateRequest**](BetaBuildLocalizationUpdateRequest.md) | BetaBuildLocalization representation |  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **200** | Single BetaBuildLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

