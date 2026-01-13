# AppStoreConnect.Net.Api.GameCenterAchievementImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementImagesCreateInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagescreateinstance) | **POST** /v1/gameCenterAchievementImages |  |
| [**GameCenterAchievementImagesDeleteInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesdeleteinstance) | **DELETE** /v1/gameCenterAchievementImages/{id} |  |
| [**GameCenterAchievementImagesGetInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesgetinstance) | **GET** /v1/gameCenterAchievementImages/{id} |  |
| [**GameCenterAchievementImagesUpdateInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesupdateinstance) | **PATCH** /v1/gameCenterAchievementImages/{id} |  |
| [**GameCenterAchievementImagesV2CreateInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesv2createinstance) | **POST** /v2/gameCenterAchievementImages |  |
| [**GameCenterAchievementImagesV2DeleteInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesv2deleteinstance) | **DELETE** /v2/gameCenterAchievementImages/{id} |  |
| [**GameCenterAchievementImagesV2GetInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesv2getinstance) | **GET** /v2/gameCenterAchievementImages/{id} |  |
| [**GameCenterAchievementImagesV2UpdateInstance**](GameCenterAchievementImagesApi.md#gamecenterachievementimagesv2updateinstance) | **PATCH** /v2/gameCenterAchievementImages/{id} |  |

<a id="gamecenterachievementimagescreateinstance"></a>
# **GameCenterAchievementImagesCreateInstance**
> GameCenterAchievementImageResponse GameCenterAchievementImagesCreateInstance (GameCenterAchievementImageCreateRequest gameCenterAchievementImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementImageCreateRequest** | [**GameCenterAchievementImageCreateRequest**](GameCenterAchievementImageCreateRequest.md) | GameCenterAchievementImage representation |  |

### Return type

[**GameCenterAchievementImageResponse**](GameCenterAchievementImageResponse.md)

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
| **201** | Single GameCenterAchievementImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementimagesdeleteinstance"></a>
# **GameCenterAchievementImagesDeleteInstance**
> void GameCenterAchievementImagesDeleteInstance (string id)




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

<a id="gamecenterachievementimagesgetinstance"></a>
# **GameCenterAchievementImagesGetInstance**
> GameCenterAchievementImageResponse GameCenterAchievementImagesGetInstance (string id, List<string> fieldsGameCenterAchievementImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementImageResponse**](GameCenterAchievementImageResponse.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementimagesupdateinstance"></a>
# **GameCenterAchievementImagesUpdateInstance**
> GameCenterAchievementImageResponse GameCenterAchievementImagesUpdateInstance (string id, GameCenterAchievementImageUpdateRequest gameCenterAchievementImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementImageUpdateRequest** | [**GameCenterAchievementImageUpdateRequest**](GameCenterAchievementImageUpdateRequest.md) | GameCenterAchievementImage representation |  |

### Return type

[**GameCenterAchievementImageResponse**](GameCenterAchievementImageResponse.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementimagesv2createinstance"></a>
# **GameCenterAchievementImagesV2CreateInstance**
> GameCenterAchievementImageV2Response GameCenterAchievementImagesV2CreateInstance (GameCenterAchievementImageV2CreateRequest gameCenterAchievementImageV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementImageV2CreateRequest** | [**GameCenterAchievementImageV2CreateRequest**](GameCenterAchievementImageV2CreateRequest.md) | GameCenterAchievementImage representation |  |

### Return type

[**GameCenterAchievementImageV2Response**](GameCenterAchievementImageV2Response.md)

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
| **201** | Single GameCenterAchievementImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementimagesv2deleteinstance"></a>
# **GameCenterAchievementImagesV2DeleteInstance**
> void GameCenterAchievementImagesV2DeleteInstance (string id)




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

<a id="gamecenterachievementimagesv2getinstance"></a>
# **GameCenterAchievementImagesV2GetInstance**
> GameCenterAchievementImageV2Response GameCenterAchievementImagesV2GetInstance (string id, List<string> fieldsGameCenterAchievementImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementImageV2Response**](GameCenterAchievementImageV2Response.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementimagesv2updateinstance"></a>
# **GameCenterAchievementImagesV2UpdateInstance**
> GameCenterAchievementImageV2Response GameCenterAchievementImagesV2UpdateInstance (string id, GameCenterAchievementImageV2UpdateRequest gameCenterAchievementImageV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementImageV2UpdateRequest** | [**GameCenterAchievementImageV2UpdateRequest**](GameCenterAchievementImageV2UpdateRequest.md) | GameCenterAchievementImage representation |  |

### Return type

[**GameCenterAchievementImageV2Response**](GameCenterAchievementImageV2Response.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

