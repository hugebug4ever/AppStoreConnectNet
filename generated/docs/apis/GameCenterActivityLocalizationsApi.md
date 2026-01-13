# AppStoreConnect.Net.Api.GameCenterActivityLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityLocalizationsCreateInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationscreateinstance) | **POST** /v1/gameCenterActivityLocalizations |  |
| [**GameCenterActivityLocalizationsDeleteInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsdeleteinstance) | **DELETE** /v1/gameCenterActivityLocalizations/{id} |  |
| [**GameCenterActivityLocalizationsGetInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsgetinstance) | **GET** /v1/gameCenterActivityLocalizations/{id} |  |
| [**GameCenterActivityLocalizationsImageGetToOneRelated**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsimagegettoonerelated) | **GET** /v1/gameCenterActivityLocalizations/{id}/image |  |
| [**GameCenterActivityLocalizationsImageGetToOneRelationship**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsimagegettoonerelationship) | **GET** /v1/gameCenterActivityLocalizations/{id}/relationships/image |  |
| [**GameCenterActivityLocalizationsUpdateInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsupdateinstance) | **PATCH** /v1/gameCenterActivityLocalizations/{id} |  |

<a id="gamecenteractivitylocalizationscreateinstance"></a>
# **GameCenterActivityLocalizationsCreateInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsCreateInstance (GameCenterActivityLocalizationCreateRequest gameCenterActivityLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityLocalizationCreateRequest** | [**GameCenterActivityLocalizationCreateRequest**](GameCenterActivityLocalizationCreateRequest.md) | GameCenterActivityLocalization representation |  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **201** | Single GameCenterActivityLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitylocalizationsdeleteinstance"></a>
# **GameCenterActivityLocalizationsDeleteInstance**
> void GameCenterActivityLocalizationsDeleteInstance (string id)




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

<a id="gamecenteractivitylocalizationsgetinstance"></a>
# **GameCenterActivityLocalizationsGetInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsGetInstance (string id, List<string> fieldsGameCenterActivityLocalizations = null, List<string> fieldsGameCenterActivityImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **200** | Single GameCenterActivityLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitylocalizationsimagegettoonerelated"></a>
# **GameCenterActivityLocalizationsImageGetToOneRelated**
> GameCenterActivityImageResponse GameCenterActivityLocalizationsImageGetToOneRelated (string id, List<string> fieldsGameCenterActivityImages = null)




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

<a id="gamecenteractivitylocalizationsimagegettoonerelationship"></a>
# **GameCenterActivityLocalizationsImageGetToOneRelationship**
> GameCenterActivityLocalizationImageLinkageResponse GameCenterActivityLocalizationsImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterActivityLocalizationImageLinkageResponse**](GameCenterActivityLocalizationImageLinkageResponse.md)

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

<a id="gamecenteractivitylocalizationsupdateinstance"></a>
# **GameCenterActivityLocalizationsUpdateInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsUpdateInstance (string id, GameCenterActivityLocalizationUpdateRequest gameCenterActivityLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLocalizationUpdateRequest** | [**GameCenterActivityLocalizationUpdateRequest**](GameCenterActivityLocalizationUpdateRequest.md) | GameCenterActivityLocalization representation |  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **200** | Single GameCenterActivityLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

