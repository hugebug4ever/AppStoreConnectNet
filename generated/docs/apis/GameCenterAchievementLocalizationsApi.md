# AppStoreConnect.Net.Api.GameCenterAchievementLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementLocalizationsCreateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationscreateinstance) | **POST** /v1/gameCenterAchievementLocalizations |  |
| [**GameCenterAchievementLocalizationsDeleteInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementgettoonerelated) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievement |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementgettoonerelationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievement |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelated) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievementImage |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievementImage |  |
| [**GameCenterAchievementLocalizationsGetInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgetinstance) | **GET** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsUpdateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsupdateinstance) | **PATCH** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2CreateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2createinstance) | **POST** /v2/gameCenterAchievementLocalizations |  |
| [**GameCenterAchievementLocalizationsV2DeleteInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2GetInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2getinstance) | **GET** /v2/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2ImageGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterAchievementLocalizations/{id}/image |  |
| [**GameCenterAchievementLocalizationsV2ImageGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterAchievementLocalizations/{id}/relationships/image |  |
| [**GameCenterAchievementLocalizationsV2UpdateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterAchievementLocalizations/{id} |  |

<a id="gamecenterachievementlocalizationscreateinstance"></a>
# **GameCenterAchievementLocalizationsCreateInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsCreateInstance (GameCenterAchievementLocalizationCreateRequest gameCenterAchievementLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementLocalizationCreateRequest** | [**GameCenterAchievementLocalizationCreateRequest**](GameCenterAchievementLocalizationCreateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **201** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsdeleteinstance"></a>
# **GameCenterAchievementLocalizationsDeleteInstance**
> void GameCenterAchievementLocalizationsDeleteInstance (string id)




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

<a id="gamecenterachievementlocalizationsgamecenterachievementgettoonerelated"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated**
> GameCenterAchievementResponse GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated (string id, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> fieldsGameCenterActivities = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsgamecenterachievementgettoonerelationship"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship**
> GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelated"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated**
> GameCenterAchievementImageResponse GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated (string id, List<string> fieldsGameCenterAchievementImages = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
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

<a id="gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelationship"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship**
> GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsgetinstance"></a>
# **GameCenterAchievementLocalizationsGetInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsGetInstance (string id, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterAchievementImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsupdateinstance"></a>
# **GameCenterAchievementLocalizationsUpdateInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsUpdateInstance (string id, GameCenterAchievementLocalizationUpdateRequest gameCenterAchievementLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementLocalizationUpdateRequest** | [**GameCenterAchievementLocalizationUpdateRequest**](GameCenterAchievementLocalizationUpdateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsv2createinstance"></a>
# **GameCenterAchievementLocalizationsV2CreateInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2CreateInstance (GameCenterAchievementLocalizationV2CreateRequest gameCenterAchievementLocalizationV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementLocalizationV2CreateRequest** | [**GameCenterAchievementLocalizationV2CreateRequest**](GameCenterAchievementLocalizationV2CreateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **201** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsv2deleteinstance"></a>
# **GameCenterAchievementLocalizationsV2DeleteInstance**
> void GameCenterAchievementLocalizationsV2DeleteInstance (string id)




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

<a id="gamecenterachievementlocalizationsv2getinstance"></a>
# **GameCenterAchievementLocalizationsV2GetInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2GetInstance (string id, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementlocalizationsv2imagegettoonerelated"></a>
# **GameCenterAchievementLocalizationsV2ImageGetToOneRelated**
> GameCenterAchievementImageV2Response GameCenterAchievementLocalizationsV2ImageGetToOneRelated (string id, List<string> fieldsGameCenterAchievementImages = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
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

<a id="gamecenterachievementlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterAchievementLocalizationsV2ImageGetToOneRelationship**
> GameCenterAchievementLocalizationV2ImageLinkageResponse GameCenterAchievementLocalizationsV2ImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationV2ImageLinkageResponse**](GameCenterAchievementLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsv2updateinstance"></a>
# **GameCenterAchievementLocalizationsV2UpdateInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2UpdateInstance (string id, GameCenterAchievementLocalizationV2UpdateRequest gameCenterAchievementLocalizationV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementLocalizationV2UpdateRequest** | [**GameCenterAchievementLocalizationV2UpdateRequest**](GameCenterAchievementLocalizationV2UpdateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

