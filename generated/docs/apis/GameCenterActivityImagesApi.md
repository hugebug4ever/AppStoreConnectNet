# AppStoreConnect.Net.Api.GameCenterActivityImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityImagesCreateInstance**](GameCenterActivityImagesApi.md#gamecenteractivityimagescreateinstance) | **POST** /v1/gameCenterActivityImages |  |
| [**GameCenterActivityImagesDeleteInstance**](GameCenterActivityImagesApi.md#gamecenteractivityimagesdeleteinstance) | **DELETE** /v1/gameCenterActivityImages/{id} |  |
| [**GameCenterActivityImagesGetInstance**](GameCenterActivityImagesApi.md#gamecenteractivityimagesgetinstance) | **GET** /v1/gameCenterActivityImages/{id} |  |
| [**GameCenterActivityImagesUpdateInstance**](GameCenterActivityImagesApi.md#gamecenteractivityimagesupdateinstance) | **PATCH** /v1/gameCenterActivityImages/{id} |  |

<a id="gamecenteractivityimagescreateinstance"></a>
# **GameCenterActivityImagesCreateInstance**
> GameCenterActivityImageResponse GameCenterActivityImagesCreateInstance (GameCenterActivityImageCreateRequest gameCenterActivityImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityImageCreateRequest** | [**GameCenterActivityImageCreateRequest**](GameCenterActivityImageCreateRequest.md) | GameCenterActivityImage representation |  |

### Return type

[**GameCenterActivityImageResponse**](GameCenterActivityImageResponse.md)

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
| **201** | Single GameCenterActivityImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityimagesdeleteinstance"></a>
# **GameCenterActivityImagesDeleteInstance**
> void GameCenterActivityImagesDeleteInstance (string id)




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

<a id="gamecenteractivityimagesgetinstance"></a>
# **GameCenterActivityImagesGetInstance**
> GameCenterActivityImageResponse GameCenterActivityImagesGetInstance (string id, List<string> fieldsGameCenterActivityImages = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |

### Return type

[**GameCenterActivityImageResponse**](GameCenterActivityImageResponse.md)

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
| **200** | Single GameCenterActivityImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityimagesupdateinstance"></a>
# **GameCenterActivityImagesUpdateInstance**
> GameCenterActivityImageResponse GameCenterActivityImagesUpdateInstance (string id, GameCenterActivityImageUpdateRequest gameCenterActivityImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityImageUpdateRequest** | [**GameCenterActivityImageUpdateRequest**](GameCenterActivityImageUpdateRequest.md) | GameCenterActivityImage representation |  |

### Return type

[**GameCenterActivityImageResponse**](GameCenterActivityImageResponse.md)

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
| **200** | Single GameCenterActivityImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

