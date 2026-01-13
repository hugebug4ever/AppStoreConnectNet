# AppStoreConnect.Net.Api.GameCenterLeaderboardReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardReleasesCreateInstance**](GameCenterLeaderboardReleasesApi.md#gamecenterleaderboardreleasescreateinstance) | **POST** /v1/gameCenterLeaderboardReleases |  |
| [**GameCenterLeaderboardReleasesDeleteInstance**](GameCenterLeaderboardReleasesApi.md#gamecenterleaderboardreleasesdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardReleases/{id} |  |
| [**GameCenterLeaderboardReleasesGetInstance**](GameCenterLeaderboardReleasesApi.md#gamecenterleaderboardreleasesgetinstance) | **GET** /v1/gameCenterLeaderboardReleases/{id} |  |

<a id="gamecenterleaderboardreleasescreateinstance"></a>
# **GameCenterLeaderboardReleasesCreateInstance**
> GameCenterLeaderboardReleaseResponse GameCenterLeaderboardReleasesCreateInstance (GameCenterLeaderboardReleaseCreateRequest gameCenterLeaderboardReleaseCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardReleaseCreateRequest** | [**GameCenterLeaderboardReleaseCreateRequest**](GameCenterLeaderboardReleaseCreateRequest.md) | GameCenterLeaderboardRelease representation |  |

### Return type

[**GameCenterLeaderboardReleaseResponse**](GameCenterLeaderboardReleaseResponse.md)

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
| **201** | Single GameCenterLeaderboardRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardreleasesdeleteinstance"></a>
# **GameCenterLeaderboardReleasesDeleteInstance**
> void GameCenterLeaderboardReleasesDeleteInstance (string id)




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

<a id="gamecenterleaderboardreleasesgetinstance"></a>
# **GameCenterLeaderboardReleasesGetInstance**
> GameCenterLeaderboardReleaseResponse GameCenterLeaderboardReleasesGetInstance (string id, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardReleaseResponse**](GameCenterLeaderboardReleaseResponse.md)

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
| **200** | Single GameCenterLeaderboardRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

