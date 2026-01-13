# AppStoreConnect.Net.Api.GameCenterChallengeImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeImagesCreateInstance**](GameCenterChallengeImagesApi.md#gamecenterchallengeimagescreateinstance) | **POST** /v1/gameCenterChallengeImages |  |
| [**GameCenterChallengeImagesDeleteInstance**](GameCenterChallengeImagesApi.md#gamecenterchallengeimagesdeleteinstance) | **DELETE** /v1/gameCenterChallengeImages/{id} |  |
| [**GameCenterChallengeImagesGetInstance**](GameCenterChallengeImagesApi.md#gamecenterchallengeimagesgetinstance) | **GET** /v1/gameCenterChallengeImages/{id} |  |
| [**GameCenterChallengeImagesUpdateInstance**](GameCenterChallengeImagesApi.md#gamecenterchallengeimagesupdateinstance) | **PATCH** /v1/gameCenterChallengeImages/{id} |  |

<a id="gamecenterchallengeimagescreateinstance"></a>
# **GameCenterChallengeImagesCreateInstance**
> GameCenterChallengeImageResponse GameCenterChallengeImagesCreateInstance (GameCenterChallengeImageCreateRequest gameCenterChallengeImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeImageCreateRequest** | [**GameCenterChallengeImageCreateRequest**](GameCenterChallengeImageCreateRequest.md) | GameCenterChallengeImage representation |  |

### Return type

[**GameCenterChallengeImageResponse**](GameCenterChallengeImageResponse.md)

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
| **201** | Single GameCenterChallengeImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengeimagesdeleteinstance"></a>
# **GameCenterChallengeImagesDeleteInstance**
> void GameCenterChallengeImagesDeleteInstance (string id)




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

<a id="gamecenterchallengeimagesgetinstance"></a>
# **GameCenterChallengeImagesGetInstance**
> GameCenterChallengeImageResponse GameCenterChallengeImagesGetInstance (string id, List<string> fieldsGameCenterChallengeImages = null)




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

<a id="gamecenterchallengeimagesupdateinstance"></a>
# **GameCenterChallengeImagesUpdateInstance**
> GameCenterChallengeImageResponse GameCenterChallengeImagesUpdateInstance (string id, GameCenterChallengeImageUpdateRequest gameCenterChallengeImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeImageUpdateRequest** | [**GameCenterChallengeImageUpdateRequest**](GameCenterChallengeImageUpdateRequest.md) | GameCenterChallengeImage representation |  |

### Return type

[**GameCenterChallengeImageResponse**](GameCenterChallengeImageResponse.md)

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
| **200** | Single GameCenterChallengeImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

