# AppStoreConnect.Net.Api.GameCenterLeaderboardVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardVersionsV2CreateInstance**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2createinstance) | **POST** /v2/gameCenterLeaderboardVersions |  |
| [**GameCenterLeaderboardVersionsV2GetInstance**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2getinstance) | **GET** /v2/gameCenterLeaderboardVersions/{id} |  |
| [**GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardVersions/{id}/localizations |  |
| [**GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardVersions/{id}/relationships/localizations |  |

<a id="gamecenterleaderboardversionsv2createinstance"></a>
# **GameCenterLeaderboardVersionsV2CreateInstance**
> GameCenterLeaderboardVersionV2Response GameCenterLeaderboardVersionsV2CreateInstance (GameCenterLeaderboardVersionV2CreateRequest gameCenterLeaderboardVersionV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardVersionV2CreateRequest** | [**GameCenterLeaderboardVersionV2CreateRequest**](GameCenterLeaderboardVersionV2CreateRequest.md) | GameCenterLeaderboardVersion representation |  |

### Return type

[**GameCenterLeaderboardVersionV2Response**](GameCenterLeaderboardVersionV2Response.md)

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
| **201** | Single GameCenterLeaderboardVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardversionsv2getinstance"></a>
# **GameCenterLeaderboardVersionsV2GetInstance**
> GameCenterLeaderboardVersionV2Response GameCenterLeaderboardVersionsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardVersions = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardVersionV2Response**](GameCenterLeaderboardVersionV2Response.md)

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
| **200** | Single GameCenterLeaderboardVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardversionsv2localizationsgettomanyrelated"></a>
# **GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated**
> GameCenterLeaderboardLocalizationsV2Response GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardVersions = null, List<string> fieldsGameCenterLeaderboardImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationsV2Response**](GameCenterLeaderboardLocalizationsV2Response.md)

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
| **200** | List of GameCenterLeaderboardLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship**
> GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse**](GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse.md)

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

