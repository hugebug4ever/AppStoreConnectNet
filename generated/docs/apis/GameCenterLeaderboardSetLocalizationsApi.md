# AppStoreConnect.Net.Api.GameCenterLeaderboardSetLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetLocalizationsCreateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationscreateinstance) | **POST** /v1/gameCenterLeaderboardSetLocalizations |  |
| [**GameCenterLeaderboardSetLocalizationsDeleteInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelated) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id}/gameCenterLeaderboardSetImage |  |
| [**GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelationship) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id}/relationships/gameCenterLeaderboardSetImage |  |
| [**GameCenterLeaderboardSetLocalizationsGetInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgetinstance) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsUpdateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2CreateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2createinstance) | **POST** /v2/gameCenterLeaderboardSetLocalizations |  |
| [**GameCenterLeaderboardSetLocalizationsV2DeleteInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2GetInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2getinstance) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id}/image |  |
| [**GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id}/relationships/image |  |
| [**GameCenterLeaderboardSetLocalizationsV2UpdateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |

<a id="gamecenterleaderboardsetlocalizationscreateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsCreateInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsCreateInstance (GameCenterLeaderboardSetLocalizationCreateRequest gameCenterLeaderboardSetLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetLocalizationCreateRequest** | [**GameCenterLeaderboardSetLocalizationCreateRequest**](GameCenterLeaderboardSetLocalizationCreateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **201** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetlocalizationsdeleteinstance"></a>
# **GameCenterLeaderboardSetLocalizationsDeleteInstance**
> void GameCenterLeaderboardSetLocalizationsDeleteInstance (string id)




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

<a id="gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelated"></a>
# **GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
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

<a id="gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelationship"></a>
# **GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship**
> GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse**](GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse.md)

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

<a id="gamecenterleaderboardsetlocalizationsgetinstance"></a>
# **GameCenterLeaderboardSetLocalizationsGetInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsGetInstance (string id, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetlocalizationsupdateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsUpdateInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsUpdateInstance (string id, GameCenterLeaderboardSetLocalizationUpdateRequest gameCenterLeaderboardSetLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetLocalizationUpdateRequest** | [**GameCenterLeaderboardSetLocalizationUpdateRequest**](GameCenterLeaderboardSetLocalizationUpdateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2createinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2CreateInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2CreateInstance (GameCenterLeaderboardSetLocalizationV2CreateRequest gameCenterLeaderboardSetLocalizationV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetLocalizationV2CreateRequest** | [**GameCenterLeaderboardSetLocalizationV2CreateRequest**](GameCenterLeaderboardSetLocalizationV2CreateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2deleteinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2DeleteInstance**
> void GameCenterLeaderboardSetLocalizationsV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardsetlocalizationsv2getinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2GetInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2imagegettoonerelated"></a>
# **GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboardSetImages = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
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

<a id="gamecenterleaderboardsetlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship**
> GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse**](GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterleaderboardsetlocalizationsv2updateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2UpdateInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2UpdateInstance (string id, GameCenterLeaderboardSetLocalizationV2UpdateRequest gameCenterLeaderboardSetLocalizationV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetLocalizationV2UpdateRequest** | [**GameCenterLeaderboardSetLocalizationV2UpdateRequest**](GameCenterLeaderboardSetLocalizationV2UpdateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

