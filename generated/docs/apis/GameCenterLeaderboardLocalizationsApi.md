# AppStoreConnect.Net.Api.GameCenterLeaderboardLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardLocalizationsCreateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationscreateinstance) | **POST** /v1/gameCenterLeaderboardLocalizations |  |
| [**GameCenterLeaderboardLocalizationsDeleteInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelated) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/gameCenterLeaderboardImage |  |
| [**GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelationship) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/relationships/gameCenterLeaderboardImage |  |
| [**GameCenterLeaderboardLocalizationsGetInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgetinstance) | **GET** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsUpdateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2CreateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2createinstance) | **POST** /v2/gameCenterLeaderboardLocalizations |  |
| [**GameCenterLeaderboardLocalizationsV2DeleteInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2GetInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2getinstance) | **GET** /v2/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterLeaderboardLocalizations/{id}/image |  |
| [**GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterLeaderboardLocalizations/{id}/relationships/image |  |
| [**GameCenterLeaderboardLocalizationsV2UpdateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardLocalizations/{id} |  |

<a id="gamecenterleaderboardlocalizationscreateinstance"></a>
# **GameCenterLeaderboardLocalizationsCreateInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsCreateInstance (GameCenterLeaderboardLocalizationCreateRequest gameCenterLeaderboardLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardLocalizationCreateRequest** | [**GameCenterLeaderboardLocalizationCreateRequest**](GameCenterLeaderboardLocalizationCreateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **201** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardlocalizationsdeleteinstance"></a>
# **GameCenterLeaderboardLocalizationsDeleteInstance**
> void GameCenterLeaderboardLocalizationsDeleteInstance (string id)




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

<a id="gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelated"></a>
# **GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated**
> GameCenterLeaderboardImageResponse GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboardImages = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
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

<a id="gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelationship"></a>
# **GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship**
> GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse**](GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse.md)

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

<a id="gamecenterleaderboardlocalizationsgetinstance"></a>
# **GameCenterLeaderboardLocalizationsGetInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsGetInstance (string id, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardlocalizationsupdateinstance"></a>
# **GameCenterLeaderboardLocalizationsUpdateInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsUpdateInstance (string id, GameCenterLeaderboardLocalizationUpdateRequest gameCenterLeaderboardLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardLocalizationUpdateRequest** | [**GameCenterLeaderboardLocalizationUpdateRequest**](GameCenterLeaderboardLocalizationUpdateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardlocalizationsv2createinstance"></a>
# **GameCenterLeaderboardLocalizationsV2CreateInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2CreateInstance (GameCenterLeaderboardLocalizationV2CreateRequest gameCenterLeaderboardLocalizationV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardLocalizationV2CreateRequest** | [**GameCenterLeaderboardLocalizationV2CreateRequest**](GameCenterLeaderboardLocalizationV2CreateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **201** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardlocalizationsv2deleteinstance"></a>
# **GameCenterLeaderboardLocalizationsV2DeleteInstance**
> void GameCenterLeaderboardLocalizationsV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardlocalizationsv2getinstance"></a>
# **GameCenterLeaderboardLocalizationsV2GetInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardlocalizationsv2imagegettoonerelated"></a>
# **GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated**
> GameCenterLeaderboardImageV2Response GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboardImages = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
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

<a id="gamecenterleaderboardlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship**
> GameCenterLeaderboardLocalizationV2ImageLinkageResponse GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardLocalizationV2ImageLinkageResponse**](GameCenterLeaderboardLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterleaderboardlocalizationsv2updateinstance"></a>
# **GameCenterLeaderboardLocalizationsV2UpdateInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2UpdateInstance (string id, GameCenterLeaderboardLocalizationV2UpdateRequest gameCenterLeaderboardLocalizationV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardLocalizationV2UpdateRequest** | [**GameCenterLeaderboardLocalizationV2UpdateRequest**](GameCenterLeaderboardLocalizationV2UpdateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

