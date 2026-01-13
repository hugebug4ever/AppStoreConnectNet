# AppStoreConnect.Net.Api.PreReleaseVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**PreReleaseVersionsAppGetToOneRelated**](PreReleaseVersionsApi.md#prereleaseversionsappgettoonerelated) | **GET** /v1/preReleaseVersions/{id}/app |  |
| [**PreReleaseVersionsAppGetToOneRelationship**](PreReleaseVersionsApi.md#prereleaseversionsappgettoonerelationship) | **GET** /v1/preReleaseVersions/{id}/relationships/app |  |
| [**PreReleaseVersionsBuildsGetToManyRelated**](PreReleaseVersionsApi.md#prereleaseversionsbuildsgettomanyrelated) | **GET** /v1/preReleaseVersions/{id}/builds |  |
| [**PreReleaseVersionsBuildsGetToManyRelationship**](PreReleaseVersionsApi.md#prereleaseversionsbuildsgettomanyrelationship) | **GET** /v1/preReleaseVersions/{id}/relationships/builds |  |
| [**PreReleaseVersionsGetCollection**](PreReleaseVersionsApi.md#prereleaseversionsgetcollection) | **GET** /v1/preReleaseVersions |  |
| [**PreReleaseVersionsGetInstance**](PreReleaseVersionsApi.md#prereleaseversionsgetinstance) | **GET** /v1/preReleaseVersions/{id} |  |

<a id="prereleaseversionsappgettoonerelated"></a>
# **PreReleaseVersionsAppGetToOneRelated**
> AppWithoutIncludesResponse PreReleaseVersionsAppGetToOneRelated (string id, List<string> fieldsApps = null)




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

<a id="prereleaseversionsappgettoonerelationship"></a>
# **PreReleaseVersionsAppGetToOneRelationship**
> PrereleaseVersionAppLinkageResponse PreReleaseVersionsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**PrereleaseVersionAppLinkageResponse**](PrereleaseVersionAppLinkageResponse.md)

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

<a id="prereleaseversionsbuildsgettomanyrelated"></a>
# **PreReleaseVersionsBuildsGetToManyRelated**
> BuildsWithoutIncludesResponse PreReleaseVersionsBuildsGetToManyRelated (string id, List<string> fieldsBuilds = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildsWithoutIncludesResponse**](BuildsWithoutIncludesResponse.md)

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
| **200** | List of Builds with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="prereleaseversionsbuildsgettomanyrelationship"></a>
# **PreReleaseVersionsBuildsGetToManyRelationship**
> PrereleaseVersionBuildsLinkagesResponse PreReleaseVersionsBuildsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**PrereleaseVersionBuildsLinkagesResponse**](PrereleaseVersionBuildsLinkagesResponse.md)

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

<a id="prereleaseversionsgetcollection"></a>
# **PreReleaseVersionsGetCollection**
> PreReleaseVersionsResponse PreReleaseVersionsGetCollection (List<string> filterBuildsBuildAudienceType = null, List<string> filterBuildsExpired = null, List<string> filterBuildsProcessingState = null, List<string> filterBuildsVersion = null, List<string> filterPlatform = null, List<string> filterVersion = null, List<string> filterApp = null, List<string> filterBuilds = null, List<string> sort = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBuilds = null, List<string> fieldsApps = null, int limit = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuildsBuildAudienceType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;builds.buildAudienceType&#39; | [optional]  |
| **filterBuildsExpired** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;builds.expired&#39; | [optional]  |
| **filterBuildsProcessingState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;builds.processingState&#39; | [optional]  |
| **filterBuildsVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;builds.version&#39; | [optional]  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**PreReleaseVersionsResponse**](PreReleaseVersionsResponse.md)

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
| **200** | List of PreReleaseVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="prereleaseversionsgetinstance"></a>
# **PreReleaseVersionsGetInstance**
> PrereleaseVersionResponse PreReleaseVersionsGetInstance (string id, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBuilds = null, List<string> fieldsApps = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**PrereleaseVersionResponse**](PrereleaseVersionResponse.md)

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
| **200** | Single PrereleaseVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

