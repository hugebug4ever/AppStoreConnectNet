# AppStoreConnect.Net.Api.BundleIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BundleIdsAppGetToOneRelated**](BundleIdsApi.md#bundleidsappgettoonerelated) | **GET** /v1/bundleIds/{id}/app |  |
| [**BundleIdsAppGetToOneRelationship**](BundleIdsApi.md#bundleidsappgettoonerelationship) | **GET** /v1/bundleIds/{id}/relationships/app |  |
| [**BundleIdsBundleIdCapabilitiesGetToManyRelated**](BundleIdsApi.md#bundleidsbundleidcapabilitiesgettomanyrelated) | **GET** /v1/bundleIds/{id}/bundleIdCapabilities |  |
| [**BundleIdsBundleIdCapabilitiesGetToManyRelationship**](BundleIdsApi.md#bundleidsbundleidcapabilitiesgettomanyrelationship) | **GET** /v1/bundleIds/{id}/relationships/bundleIdCapabilities |  |
| [**BundleIdsCreateInstance**](BundleIdsApi.md#bundleidscreateinstance) | **POST** /v1/bundleIds |  |
| [**BundleIdsDeleteInstance**](BundleIdsApi.md#bundleidsdeleteinstance) | **DELETE** /v1/bundleIds/{id} |  |
| [**BundleIdsGetCollection**](BundleIdsApi.md#bundleidsgetcollection) | **GET** /v1/bundleIds |  |
| [**BundleIdsGetInstance**](BundleIdsApi.md#bundleidsgetinstance) | **GET** /v1/bundleIds/{id} |  |
| [**BundleIdsProfilesGetToManyRelated**](BundleIdsApi.md#bundleidsprofilesgettomanyrelated) | **GET** /v1/bundleIds/{id}/profiles |  |
| [**BundleIdsProfilesGetToManyRelationship**](BundleIdsApi.md#bundleidsprofilesgettomanyrelationship) | **GET** /v1/bundleIds/{id}/relationships/profiles |  |
| [**BundleIdsUpdateInstance**](BundleIdsApi.md#bundleidsupdateinstance) | **PATCH** /v1/bundleIds/{id} |  |

<a id="bundleidsappgettoonerelated"></a>
# **BundleIdsAppGetToOneRelated**
> AppWithoutIncludesResponse BundleIdsAppGetToOneRelated (string id, List<string> fieldsApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsappgettoonerelationship"></a>
# **BundleIdsAppGetToOneRelationship**
> BundleIdAppLinkageResponse BundleIdsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BundleIdAppLinkageResponse**](BundleIdAppLinkageResponse.md)

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

<a id="bundleidsbundleidcapabilitiesgettomanyrelated"></a>
# **BundleIdsBundleIdCapabilitiesGetToManyRelated**
> BundleIdCapabilitiesWithoutIncludesResponse BundleIdsBundleIdCapabilitiesGetToManyRelated (string id, List<string> fieldsBundleIdCapabilities = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBundleIdCapabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIdCapabilities | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BundleIdCapabilitiesWithoutIncludesResponse**](BundleIdCapabilitiesWithoutIncludesResponse.md)

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
| **200** | List of BundleIdCapabilities with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsbundleidcapabilitiesgettomanyrelationship"></a>
# **BundleIdsBundleIdCapabilitiesGetToManyRelationship**
> BundleIdBundleIdCapabilitiesLinkagesResponse BundleIdsBundleIdCapabilitiesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BundleIdBundleIdCapabilitiesLinkagesResponse**](BundleIdBundleIdCapabilitiesLinkagesResponse.md)

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

<a id="bundleidscreateinstance"></a>
# **BundleIdsCreateInstance**
> BundleIdResponse BundleIdsCreateInstance (BundleIdCreateRequest bundleIdCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **bundleIdCreateRequest** | [**BundleIdCreateRequest**](BundleIdCreateRequest.md) | BundleId representation |  |

### Return type

[**BundleIdResponse**](BundleIdResponse.md)

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
| **201** | Single BundleId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsdeleteinstance"></a>
# **BundleIdsDeleteInstance**
> void BundleIdsDeleteInstance (string id)




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

<a id="bundleidsgetcollection"></a>
# **BundleIdsGetCollection**
> BundleIdsResponse BundleIdsGetCollection (List<string> filterName = null, List<string> filterPlatform = null, List<string> filterIdentifier = null, List<string> filterSeedId = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsBundleIds = null, List<string> fieldsProfiles = null, List<string> fieldsBundleIdCapabilities = null, List<string> fieldsApps = null, int limit = null, List<string> include = null, int limitBundleIdCapabilities = null, int limitProfiles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterIdentifier** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;identifier&#39; | [optional]  |
| **filterSeedId** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;seedId&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBundleIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIds | [optional]  |
| **fieldsProfiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type profiles | [optional]  |
| **fieldsBundleIdCapabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIdCapabilities | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBundleIdCapabilities** | **int** | maximum number of related bundleIdCapabilities returned (when they are included) | [optional]  |
| **limitProfiles** | **int** | maximum number of related profiles returned (when they are included) | [optional]  |

### Return type

[**BundleIdsResponse**](BundleIdsResponse.md)

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
| **200** | List of BundleIds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsgetinstance"></a>
# **BundleIdsGetInstance**
> BundleIdResponse BundleIdsGetInstance (string id, List<string> fieldsBundleIds = null, List<string> fieldsProfiles = null, List<string> fieldsBundleIdCapabilities = null, List<string> fieldsApps = null, List<string> include = null, int limitBundleIdCapabilities = null, int limitProfiles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBundleIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIds | [optional]  |
| **fieldsProfiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type profiles | [optional]  |
| **fieldsBundleIdCapabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIdCapabilities | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBundleIdCapabilities** | **int** | maximum number of related bundleIdCapabilities returned (when they are included) | [optional]  |
| **limitProfiles** | **int** | maximum number of related profiles returned (when they are included) | [optional]  |

### Return type

[**BundleIdResponse**](BundleIdResponse.md)

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
| **200** | Single BundleId |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsprofilesgettomanyrelated"></a>
# **BundleIdsProfilesGetToManyRelated**
> ProfilesWithoutIncludesResponse BundleIdsProfilesGetToManyRelated (string id, List<string> fieldsProfiles = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsProfiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type profiles | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ProfilesWithoutIncludesResponse**](ProfilesWithoutIncludesResponse.md)

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
| **200** | List of Profiles with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidsprofilesgettomanyrelationship"></a>
# **BundleIdsProfilesGetToManyRelationship**
> BundleIdProfilesLinkagesResponse BundleIdsProfilesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BundleIdProfilesLinkagesResponse**](BundleIdProfilesLinkagesResponse.md)

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

<a id="bundleidsupdateinstance"></a>
# **BundleIdsUpdateInstance**
> BundleIdResponse BundleIdsUpdateInstance (string id, BundleIdUpdateRequest bundleIdUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **bundleIdUpdateRequest** | [**BundleIdUpdateRequest**](BundleIdUpdateRequest.md) | BundleId representation |  |

### Return type

[**BundleIdResponse**](BundleIdResponse.md)

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
| **200** | Single BundleId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

