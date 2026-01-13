# AppStoreConnect.Net.Api.GameCenterLeaderboardSetVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetVersionsV2CreateInstance**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2createinstance) | **POST** /v2/gameCenterLeaderboardSetVersions |  |
| [**GameCenterLeaderboardSetVersionsV2GetInstance**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2getinstance) | **GET** /v2/gameCenterLeaderboardSetVersions/{id} |  |
| [**GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardSetVersions/{id}/localizations |  |
| [**GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardSetVersions/{id}/relationships/localizations |  |

<a id="gamecenterleaderboardsetversionsv2createinstance"></a>
# **GameCenterLeaderboardSetVersionsV2CreateInstance**
> GameCenterLeaderboardSetVersionV2Response GameCenterLeaderboardSetVersionsV2CreateInstance (GameCenterLeaderboardSetVersionV2CreateRequest gameCenterLeaderboardSetVersionV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetVersionV2CreateRequest** | [**GameCenterLeaderboardSetVersionV2CreateRequest**](GameCenterLeaderboardSetVersionV2CreateRequest.md) | GameCenterLeaderboardSetVersion representation |  |

### Return type

[**GameCenterLeaderboardSetVersionV2Response**](GameCenterLeaderboardSetVersionV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetversionsv2getinstance"></a>
# **GameCenterLeaderboardSetVersionsV2GetInstance**
> GameCenterLeaderboardSetVersionV2Response GameCenterLeaderboardSetVersionsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardSetVersions = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetVersionV2Response**](GameCenterLeaderboardSetVersionV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetversionsv2localizationsgettomanyrelated"></a>
# **GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated**
> GameCenterLeaderboardSetLocalizationsV2Response GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboardSetVersions = null, List<string> fieldsGameCenterLeaderboardSetImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationsV2Response**](GameCenterLeaderboardSetLocalizationsV2Response.md)

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
| **200** | List of GameCenterLeaderboardSetLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship**
> GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse**](GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse.md)

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

