# AppStoreConnect.Net.Api.GameCenterEnabledVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterEnabledVersionsCompatibleVersionsCreateToManyRelationship**](GameCenterEnabledVersionsApi.md#gamecenterenabledversionscompatibleversionscreatetomanyrelationship) | **POST** /v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions |  |
| [**GameCenterEnabledVersionsCompatibleVersionsDeleteToManyRelationship**](GameCenterEnabledVersionsApi.md#gamecenterenabledversionscompatibleversionsdeletetomanyrelationship) | **DELETE** /v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions |  |
| [**GameCenterEnabledVersionsCompatibleVersionsGetToManyRelated**](GameCenterEnabledVersionsApi.md#gamecenterenabledversionscompatibleversionsgettomanyrelated) | **GET** /v1/gameCenterEnabledVersions/{id}/compatibleVersions |  |
| [**GameCenterEnabledVersionsCompatibleVersionsGetToManyRelationship**](GameCenterEnabledVersionsApi.md#gamecenterenabledversionscompatibleversionsgettomanyrelationship) | **GET** /v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions |  |
| [**GameCenterEnabledVersionsCompatibleVersionsReplaceToManyRelationship**](GameCenterEnabledVersionsApi.md#gamecenterenabledversionscompatibleversionsreplacetomanyrelationship) | **PATCH** /v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions |  |

<a id="gamecenterenabledversionscompatibleversionscreatetomanyrelationship"></a>
# **GameCenterEnabledVersionsCompatibleVersionsCreateToManyRelationship**
> void GameCenterEnabledVersionsCompatibleVersionsCreateToManyRelationship (string id, GameCenterEnabledVersionCompatibleVersionsLinkagesRequest gameCenterEnabledVersionCompatibleVersionsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterEnabledVersionCompatibleVersionsLinkagesRequest** | [**GameCenterEnabledVersionCompatibleVersionsLinkagesRequest**](GameCenterEnabledVersionCompatibleVersionsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterenabledversionscompatibleversionsdeletetomanyrelationship"></a>
# **GameCenterEnabledVersionsCompatibleVersionsDeleteToManyRelationship**
> void GameCenterEnabledVersionsCompatibleVersionsDeleteToManyRelationship (string id, GameCenterEnabledVersionCompatibleVersionsLinkagesRequest gameCenterEnabledVersionCompatibleVersionsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterEnabledVersionCompatibleVersionsLinkagesRequest** | [**GameCenterEnabledVersionCompatibleVersionsLinkagesRequest**](GameCenterEnabledVersionCompatibleVersionsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterenabledversionscompatibleversionsgettomanyrelated"></a>
# **GameCenterEnabledVersionsCompatibleVersionsGetToManyRelated**
> GameCenterEnabledVersionsResponse GameCenterEnabledVersionsCompatibleVersionsGetToManyRelated (string id, List<string> filterPlatform = null, List<string> filterVersionString = null, List<string> filterApp = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsGameCenterEnabledVersions = null, List<string> fieldsApps = null, int limit = null, List<string> include = null, int limitCompatibleVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterVersionString** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;versionString&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsGameCenterEnabledVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterEnabledVersions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCompatibleVersions** | **int** | maximum number of related compatibleVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterEnabledVersionsResponse**](GameCenterEnabledVersionsResponse.md)

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
| **200** | List of GameCenterEnabledVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterenabledversionscompatibleversionsgettomanyrelationship"></a>
# **GameCenterEnabledVersionsCompatibleVersionsGetToManyRelationship**
> GameCenterEnabledVersionCompatibleVersionsLinkagesResponse GameCenterEnabledVersionsCompatibleVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterEnabledVersionCompatibleVersionsLinkagesResponse**](GameCenterEnabledVersionCompatibleVersionsLinkagesResponse.md)

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

<a id="gamecenterenabledversionscompatibleversionsreplacetomanyrelationship"></a>
# **GameCenterEnabledVersionsCompatibleVersionsReplaceToManyRelationship**
> void GameCenterEnabledVersionsCompatibleVersionsReplaceToManyRelationship (string id, GameCenterEnabledVersionCompatibleVersionsLinkagesRequest gameCenterEnabledVersionCompatibleVersionsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterEnabledVersionCompatibleVersionsLinkagesRequest** | [**GameCenterEnabledVersionCompatibleVersionsLinkagesRequest**](GameCenterEnabledVersionCompatibleVersionsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

