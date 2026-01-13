# AppStoreConnect.Net.Api.GameCenterAchievementVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementVersionsV2CreateInstance**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2createinstance) | **POST** /v2/gameCenterAchievementVersions |  |
| [**GameCenterAchievementVersionsV2GetInstance**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2getinstance) | **GET** /v2/gameCenterAchievementVersions/{id} |  |
| [**GameCenterAchievementVersionsV2LocalizationsGetToManyRelated**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterAchievementVersions/{id}/localizations |  |
| [**GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterAchievementVersions/{id}/relationships/localizations |  |

<a id="gamecenterachievementversionsv2createinstance"></a>
# **GameCenterAchievementVersionsV2CreateInstance**
> GameCenterAchievementVersionV2Response GameCenterAchievementVersionsV2CreateInstance (GameCenterAchievementVersionV2CreateRequest gameCenterAchievementVersionV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementVersionV2CreateRequest** | [**GameCenterAchievementVersionV2CreateRequest**](GameCenterAchievementVersionV2CreateRequest.md) | GameCenterAchievementVersion representation |  |

### Return type

[**GameCenterAchievementVersionV2Response**](GameCenterAchievementVersionV2Response.md)

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
| **201** | Single GameCenterAchievementVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementversionsv2getinstance"></a>
# **GameCenterAchievementVersionsV2GetInstance**
> GameCenterAchievementVersionV2Response GameCenterAchievementVersionsV2GetInstance (string id, List<string> fieldsGameCenterAchievementVersions = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementVersionV2Response**](GameCenterAchievementVersionV2Response.md)

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
| **200** | Single GameCenterAchievementVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementversionsv2localizationsgettomanyrelated"></a>
# **GameCenterAchievementVersionsV2LocalizationsGetToManyRelated**
> GameCenterAchievementLocalizationsV2Response GameCenterAchievementVersionsV2LocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementVersions = null, List<string> fieldsGameCenterAchievementImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationsV2Response**](GameCenterAchievementLocalizationsV2Response.md)

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
| **200** | List of GameCenterAchievementLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship**
> GameCenterAchievementVersionV2LocalizationsLinkagesResponse GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterAchievementVersionV2LocalizationsLinkagesResponse**](GameCenterAchievementVersionV2LocalizationsLinkagesResponse.md)

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

