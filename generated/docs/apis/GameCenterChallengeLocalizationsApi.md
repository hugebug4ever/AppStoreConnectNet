# AppStoreConnect.Net.Api.GameCenterChallengeLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeLocalizationsCreateInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationscreateinstance) | **POST** /v1/gameCenterChallengeLocalizations |  |
| [**GameCenterChallengeLocalizationsDeleteInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsdeleteinstance) | **DELETE** /v1/gameCenterChallengeLocalizations/{id} |  |
| [**GameCenterChallengeLocalizationsGetInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsgetinstance) | **GET** /v1/gameCenterChallengeLocalizations/{id} |  |
| [**GameCenterChallengeLocalizationsImageGetToOneRelated**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsimagegettoonerelated) | **GET** /v1/gameCenterChallengeLocalizations/{id}/image |  |
| [**GameCenterChallengeLocalizationsImageGetToOneRelationship**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsimagegettoonerelationship) | **GET** /v1/gameCenterChallengeLocalizations/{id}/relationships/image |  |
| [**GameCenterChallengeLocalizationsUpdateInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsupdateinstance) | **PATCH** /v1/gameCenterChallengeLocalizations/{id} |  |

<a id="gamecenterchallengelocalizationscreateinstance"></a>
# **GameCenterChallengeLocalizationsCreateInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsCreateInstance (GameCenterChallengeLocalizationCreateRequest gameCenterChallengeLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeLocalizationCreateRequest** | [**GameCenterChallengeLocalizationCreateRequest**](GameCenterChallengeLocalizationCreateRequest.md) | GameCenterChallengeLocalization representation |  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **201** | Single GameCenterChallengeLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengelocalizationsdeleteinstance"></a>
# **GameCenterChallengeLocalizationsDeleteInstance**
> void GameCenterChallengeLocalizationsDeleteInstance (string id)




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

<a id="gamecenterchallengelocalizationsgetinstance"></a>
# **GameCenterChallengeLocalizationsGetInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsGetInstance (string id, List<string> fieldsGameCenterChallengeLocalizations = null, List<string> fieldsGameCenterChallengeImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **200** | Single GameCenterChallengeLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengelocalizationsimagegettoonerelated"></a>
# **GameCenterChallengeLocalizationsImageGetToOneRelated**
> GameCenterChallengeImageResponse GameCenterChallengeLocalizationsImageGetToOneRelated (string id, List<string> fieldsGameCenterChallengeImages = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |

### Return type

[**GameCenterChallengeImageResponse**](GameCenterChallengeImageResponse.md)

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
| **200** | Single GameCenterChallengeImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengelocalizationsimagegettoonerelationship"></a>
# **GameCenterChallengeLocalizationsImageGetToOneRelationship**
> GameCenterChallengeLocalizationImageLinkageResponse GameCenterChallengeLocalizationsImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterChallengeLocalizationImageLinkageResponse**](GameCenterChallengeLocalizationImageLinkageResponse.md)

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

<a id="gamecenterchallengelocalizationsupdateinstance"></a>
# **GameCenterChallengeLocalizationsUpdateInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsUpdateInstance (string id, GameCenterChallengeLocalizationUpdateRequest gameCenterChallengeLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeLocalizationUpdateRequest** | [**GameCenterChallengeLocalizationUpdateRequest**](GameCenterChallengeLocalizationUpdateRequest.md) | GameCenterChallengeLocalization representation |  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **200** | Single GameCenterChallengeLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

