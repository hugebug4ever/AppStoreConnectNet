# AppStoreConnect.Net.Api.GameCenterActivityVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityVersionsCreateInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionscreateinstance) | **POST** /v1/gameCenterActivityVersions |  |
| [**GameCenterActivityVersionsDefaultImageGetToOneRelated**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsdefaultimagegettoonerelated) | **GET** /v1/gameCenterActivityVersions/{id}/defaultImage |  |
| [**GameCenterActivityVersionsDefaultImageGetToOneRelationship**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsdefaultimagegettoonerelationship) | **GET** /v1/gameCenterActivityVersions/{id}/relationships/defaultImage |  |
| [**GameCenterActivityVersionsGetInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsgetinstance) | **GET** /v1/gameCenterActivityVersions/{id} |  |
| [**GameCenterActivityVersionsLocalizationsGetToManyRelated**](GameCenterActivityVersionsApi.md#gamecenteractivityversionslocalizationsgettomanyrelated) | **GET** /v1/gameCenterActivityVersions/{id}/localizations |  |
| [**GameCenterActivityVersionsLocalizationsGetToManyRelationship**](GameCenterActivityVersionsApi.md#gamecenteractivityversionslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterActivityVersions/{id}/relationships/localizations |  |
| [**GameCenterActivityVersionsUpdateInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsupdateinstance) | **PATCH** /v1/gameCenterActivityVersions/{id} |  |

<a id="gamecenteractivityversionscreateinstance"></a>
# **GameCenterActivityVersionsCreateInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsCreateInstance (GameCenterActivityVersionCreateRequest gameCenterActivityVersionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityVersionCreateRequest** | [**GameCenterActivityVersionCreateRequest**](GameCenterActivityVersionCreateRequest.md) | GameCenterActivityVersion representation |  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **201** | Single GameCenterActivityVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityversionsdefaultimagegettoonerelated"></a>
# **GameCenterActivityVersionsDefaultImageGetToOneRelated**
> GameCenterActivityImageResponse GameCenterActivityVersionsDefaultImageGetToOneRelated (string id, List<string> fieldsGameCenterActivityImages = null)




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

<a id="gamecenteractivityversionsdefaultimagegettoonerelationship"></a>
# **GameCenterActivityVersionsDefaultImageGetToOneRelationship**
> GameCenterActivityVersionDefaultImageLinkageResponse GameCenterActivityVersionsDefaultImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterActivityVersionDefaultImageLinkageResponse**](GameCenterActivityVersionDefaultImageLinkageResponse.md)

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

<a id="gamecenteractivityversionsgetinstance"></a>
# **GameCenterActivityVersionsGetInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsGetInstance (string id, List<string> fieldsGameCenterActivityVersions = null, List<string> fieldsGameCenterActivityLocalizations = null, List<string> fieldsGameCenterActivityImages = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **200** | Single GameCenterActivityVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityversionslocalizationsgettomanyrelated"></a>
# **GameCenterActivityVersionsLocalizationsGetToManyRelated**
> GameCenterActivityLocalizationsResponse GameCenterActivityVersionsLocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterActivityLocalizations = null, List<string> fieldsGameCenterActivityVersions = null, List<string> fieldsGameCenterActivityImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityLocalizationsResponse**](GameCenterActivityLocalizationsResponse.md)

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
| **200** | List of GameCenterActivityLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityversionslocalizationsgettomanyrelationship"></a>
# **GameCenterActivityVersionsLocalizationsGetToManyRelationship**
> GameCenterActivityVersionLocalizationsLinkagesResponse GameCenterActivityVersionsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterActivityVersionLocalizationsLinkagesResponse**](GameCenterActivityVersionLocalizationsLinkagesResponse.md)

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
| **200** | List of related linkages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityversionsupdateinstance"></a>
# **GameCenterActivityVersionsUpdateInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsUpdateInstance (string id, GameCenterActivityVersionUpdateRequest gameCenterActivityVersionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityVersionUpdateRequest** | [**GameCenterActivityVersionUpdateRequest**](GameCenterActivityVersionUpdateRequest.md) | GameCenterActivityVersion representation |  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **200** | Single GameCenterActivityVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

