# AppStoreConnect.Net.Api.GameCenterLeaderboardSetImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetImagesCreateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagescreateinstance) | **POST** /v1/gameCenterLeaderboardSetImages |  |
| [**GameCenterLeaderboardSetImagesDeleteInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesGetInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesgetinstance) | **GET** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesUpdateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2CreateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2createinstance) | **POST** /v2/gameCenterLeaderboardSetImages |  |
| [**GameCenterLeaderboardSetImagesV2DeleteInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2GetInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2getinstance) | **GET** /v2/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2UpdateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardSetImages/{id} |  |

<a id="gamecenterleaderboardsetimagescreateinstance"></a>
# **GameCenterLeaderboardSetImagesCreateInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesCreateInstance (GameCenterLeaderboardSetImageCreateRequest gameCenterLeaderboardSetImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetImageCreateRequest** | [**GameCenterLeaderboardSetImageCreateRequest**](GameCenterLeaderboardSetImageCreateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **201** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetimagesdeleteinstance"></a>
# **GameCenterLeaderboardSetImagesDeleteInstance**
> void GameCenterLeaderboardSetImagesDeleteInstance (string id)




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

<a id="gamecenterleaderboardsetimagesgetinstance"></a>
# **GameCenterLeaderboardSetImagesGetInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesGetInstance (string id, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetimagesupdateinstance"></a>
# **GameCenterLeaderboardSetImagesUpdateInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesUpdateInstance (string id, GameCenterLeaderboardSetImageUpdateRequest gameCenterLeaderboardSetImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetImageUpdateRequest** | [**GameCenterLeaderboardSetImageUpdateRequest**](GameCenterLeaderboardSetImageUpdateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetimagesv2createinstance"></a>
# **GameCenterLeaderboardSetImagesV2CreateInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2CreateInstance (GameCenterLeaderboardSetImageV2CreateRequest gameCenterLeaderboardSetImageV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetImageV2CreateRequest** | [**GameCenterLeaderboardSetImageV2CreateRequest**](GameCenterLeaderboardSetImageV2CreateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetimagesv2deleteinstance"></a>
# **GameCenterLeaderboardSetImagesV2DeleteInstance**
> void GameCenterLeaderboardSetImagesV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardsetimagesv2getinstance"></a>
# **GameCenterLeaderboardSetImagesV2GetInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetimagesv2updateinstance"></a>
# **GameCenterLeaderboardSetImagesV2UpdateInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2UpdateInstance (string id, GameCenterLeaderboardSetImageV2UpdateRequest gameCenterLeaderboardSetImageV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetImageV2UpdateRequest** | [**GameCenterLeaderboardSetImageV2UpdateRequest**](GameCenterLeaderboardSetImageV2UpdateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

