# AppStoreConnect.Net.Api.GameCenterChallengeVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeVersionsCreateInstance**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionscreateinstance) | **POST** /v1/gameCenterChallengeVersions |  |
| [**GameCenterChallengeVersionsDefaultImageGetToOneRelated**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsdefaultimagegettoonerelated) | **GET** /v1/gameCenterChallengeVersions/{id}/defaultImage |  |
| [**GameCenterChallengeVersionsDefaultImageGetToOneRelationship**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsdefaultimagegettoonerelationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/defaultImage |  |
| [**GameCenterChallengeVersionsGetInstance**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsgetinstance) | **GET** /v1/gameCenterChallengeVersions/{id} |  |
| [**GameCenterChallengeVersionsLocalizationsGetToManyRelated**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionslocalizationsgettomanyrelated) | **GET** /v1/gameCenterChallengeVersions/{id}/localizations |  |
| [**GameCenterChallengeVersionsLocalizationsGetToManyRelationship**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/localizations |  |

<a id="gamecenterchallengeversionscreateinstance"></a>
# **GameCenterChallengeVersionsCreateInstance**
> GameCenterChallengeVersionResponse GameCenterChallengeVersionsCreateInstance (GameCenterChallengeVersionCreateRequest gameCenterChallengeVersionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeVersionCreateRequest** | [**GameCenterChallengeVersionCreateRequest**](GameCenterChallengeVersionCreateRequest.md) | GameCenterChallengeVersion representation |  |

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
| **201** | Single GameCenterChallengeVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengeversionsdefaultimagegettoonerelated"></a>
# **GameCenterChallengeVersionsDefaultImageGetToOneRelated**
> GameCenterChallengeImageResponse GameCenterChallengeVersionsDefaultImageGetToOneRelated (string id, List<string> fieldsGameCenterChallengeImages = null)




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

<a id="gamecenterchallengeversionsdefaultimagegettoonerelationship"></a>
# **GameCenterChallengeVersionsDefaultImageGetToOneRelationship**
> GameCenterChallengeVersionDefaultImageLinkageResponse GameCenterChallengeVersionsDefaultImageGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterChallengeVersionDefaultImageLinkageResponse**](GameCenterChallengeVersionDefaultImageLinkageResponse.md)

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

<a id="gamecenterchallengeversionsgetinstance"></a>
# **GameCenterChallengeVersionsGetInstance**
> GameCenterChallengeVersionResponse GameCenterChallengeVersionsGetInstance (string id, List<string> fieldsGameCenterChallengeVersions = null, List<string> fieldsGameCenterChallengeLocalizations = null, List<string> fieldsGameCenterChallengeImages = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
| **200** | Single GameCenterChallengeVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengeversionslocalizationsgettomanyrelated"></a>
# **GameCenterChallengeVersionsLocalizationsGetToManyRelated**
> GameCenterChallengeLocalizationsResponse GameCenterChallengeVersionsLocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterChallengeLocalizations = null, List<string> fieldsGameCenterChallengeVersions = null, List<string> fieldsGameCenterChallengeImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterChallengeLocalizationsResponse**](GameCenterChallengeLocalizationsResponse.md)

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
| **200** | List of GameCenterChallengeLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengeversionslocalizationsgettomanyrelationship"></a>
# **GameCenterChallengeVersionsLocalizationsGetToManyRelationship**
> GameCenterChallengeVersionLocalizationsLinkagesResponse GameCenterChallengeVersionsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterChallengeVersionLocalizationsLinkagesResponse**](GameCenterChallengeVersionLocalizationsLinkagesResponse.md)

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

