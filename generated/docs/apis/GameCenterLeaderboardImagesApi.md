# AppStoreConnect.Net.Api.GameCenterLeaderboardImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardImagesCreateInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagescreateinstance) | **POST** /v1/gameCenterLeaderboardImages |  |
| [**GameCenterLeaderboardImagesDeleteInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardImages/{id} |  |
| [**GameCenterLeaderboardImagesGetInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesgetinstance) | **GET** /v1/gameCenterLeaderboardImages/{id} |  |
| [**GameCenterLeaderboardImagesUpdateInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesupdateinstance) | **PATCH** /v1/gameCenterLeaderboardImages/{id} |  |
| [**GameCenterLeaderboardImagesV2CreateInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesv2createinstance) | **POST** /v2/gameCenterLeaderboardImages |  |
| [**GameCenterLeaderboardImagesV2DeleteInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardImages/{id} |  |
| [**GameCenterLeaderboardImagesV2GetInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesv2getinstance) | **GET** /v2/gameCenterLeaderboardImages/{id} |  |
| [**GameCenterLeaderboardImagesV2UpdateInstance**](GameCenterLeaderboardImagesApi.md#gamecenterleaderboardimagesv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardImages/{id} |  |

<a id="gamecenterleaderboardimagescreateinstance"></a>
# **GameCenterLeaderboardImagesCreateInstance**
> GameCenterLeaderboardImageResponse GameCenterLeaderboardImagesCreateInstance (GameCenterLeaderboardImageCreateRequest gameCenterLeaderboardImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardImageCreateRequest** | [**GameCenterLeaderboardImageCreateRequest**](GameCenterLeaderboardImageCreateRequest.md) | GameCenterLeaderboardImage representation |  |

### Return type

[**GameCenterLeaderboardImageResponse**](GameCenterLeaderboardImageResponse.md)

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
| **201** | Single GameCenterLeaderboardImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardimagesdeleteinstance"></a>
# **GameCenterLeaderboardImagesDeleteInstance**
> void GameCenterLeaderboardImagesDeleteInstance (string id)




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

<a id="gamecenterleaderboardimagesgetinstance"></a>
# **GameCenterLeaderboardImagesGetInstance**
> GameCenterLeaderboardImageResponse GameCenterLeaderboardImagesGetInstance (string id, List<string> fieldsGameCenterLeaderboardImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardImageResponse**](GameCenterLeaderboardImageResponse.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardimagesupdateinstance"></a>
# **GameCenterLeaderboardImagesUpdateInstance**
> GameCenterLeaderboardImageResponse GameCenterLeaderboardImagesUpdateInstance (string id, GameCenterLeaderboardImageUpdateRequest gameCenterLeaderboardImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardImageUpdateRequest** | [**GameCenterLeaderboardImageUpdateRequest**](GameCenterLeaderboardImageUpdateRequest.md) | GameCenterLeaderboardImage representation |  |

### Return type

[**GameCenterLeaderboardImageResponse**](GameCenterLeaderboardImageResponse.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardimagesv2createinstance"></a>
# **GameCenterLeaderboardImagesV2CreateInstance**
> GameCenterLeaderboardImageV2Response GameCenterLeaderboardImagesV2CreateInstance (GameCenterLeaderboardImageV2CreateRequest gameCenterLeaderboardImageV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardImageV2CreateRequest** | [**GameCenterLeaderboardImageV2CreateRequest**](GameCenterLeaderboardImageV2CreateRequest.md) | GameCenterLeaderboardImage representation |  |

### Return type

[**GameCenterLeaderboardImageV2Response**](GameCenterLeaderboardImageV2Response.md)

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
| **201** | Single GameCenterLeaderboardImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardimagesv2deleteinstance"></a>
# **GameCenterLeaderboardImagesV2DeleteInstance**
> void GameCenterLeaderboardImagesV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardimagesv2getinstance"></a>
# **GameCenterLeaderboardImagesV2GetInstance**
> GameCenterLeaderboardImageV2Response GameCenterLeaderboardImagesV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardImageV2Response**](GameCenterLeaderboardImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardimagesv2updateinstance"></a>
# **GameCenterLeaderboardImagesV2UpdateInstance**
> GameCenterLeaderboardImageV2Response GameCenterLeaderboardImagesV2UpdateInstance (string id, GameCenterLeaderboardImageV2UpdateRequest gameCenterLeaderboardImageV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardImageV2UpdateRequest** | [**GameCenterLeaderboardImageV2UpdateRequest**](GameCenterLeaderboardImageV2UpdateRequest.md) | GameCenterLeaderboardImage representation |  |

### Return type

[**GameCenterLeaderboardImageV2Response**](GameCenterLeaderboardImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

