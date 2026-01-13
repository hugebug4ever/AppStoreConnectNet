# AppStoreConnect.Net.Api.GameCenterActivityVersionReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityVersionReleasesCreateInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasescreateinstance) | **POST** /v1/gameCenterActivityVersionReleases |  |
| [**GameCenterActivityVersionReleasesDeleteInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasesdeleteinstance) | **DELETE** /v1/gameCenterActivityVersionReleases/{id} |  |
| [**GameCenterActivityVersionReleasesGetInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasesgetinstance) | **GET** /v1/gameCenterActivityVersionReleases/{id} |  |

<a id="gamecenteractivityversionreleasescreateinstance"></a>
# **GameCenterActivityVersionReleasesCreateInstance**
> GameCenterActivityVersionReleaseResponse GameCenterActivityVersionReleasesCreateInstance (GameCenterActivityVersionReleaseCreateRequest gameCenterActivityVersionReleaseCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityVersionReleaseCreateRequest** | [**GameCenterActivityVersionReleaseCreateRequest**](GameCenterActivityVersionReleaseCreateRequest.md) | GameCenterActivityVersionRelease representation |  |

### Return type

[**GameCenterActivityVersionReleaseResponse**](GameCenterActivityVersionReleaseResponse.md)

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
| **201** | Single GameCenterActivityVersionRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivityversionreleasesdeleteinstance"></a>
# **GameCenterActivityVersionReleasesDeleteInstance**
> void GameCenterActivityVersionReleasesDeleteInstance (string id)




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

<a id="gamecenteractivityversionreleasesgetinstance"></a>
# **GameCenterActivityVersionReleasesGetInstance**
> GameCenterActivityVersionReleaseResponse GameCenterActivityVersionReleasesGetInstance (string id, List<string> fieldsGameCenterActivityVersionReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityVersionReleaseResponse**](GameCenterActivityVersionReleaseResponse.md)

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
| **200** | Single GameCenterActivityVersionRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

