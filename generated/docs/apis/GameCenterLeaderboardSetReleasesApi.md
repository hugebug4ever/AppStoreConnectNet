# AppStoreConnect.Net.Api.GameCenterLeaderboardSetReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetReleasesCreateInstance**](GameCenterLeaderboardSetReleasesApi.md#gamecenterleaderboardsetreleasescreateinstance) | **POST** /v1/gameCenterLeaderboardSetReleases |  |
| [**GameCenterLeaderboardSetReleasesDeleteInstance**](GameCenterLeaderboardSetReleasesApi.md#gamecenterleaderboardsetreleasesdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetReleases/{id} |  |
| [**GameCenterLeaderboardSetReleasesGetInstance**](GameCenterLeaderboardSetReleasesApi.md#gamecenterleaderboardsetreleasesgetinstance) | **GET** /v1/gameCenterLeaderboardSetReleases/{id} |  |

<a id="gamecenterleaderboardsetreleasescreateinstance"></a>
# **GameCenterLeaderboardSetReleasesCreateInstance**
> GameCenterLeaderboardSetReleaseResponse GameCenterLeaderboardSetReleasesCreateInstance (GameCenterLeaderboardSetReleaseCreateRequest gameCenterLeaderboardSetReleaseCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetReleaseCreateRequest** | [**GameCenterLeaderboardSetReleaseCreateRequest**](GameCenterLeaderboardSetReleaseCreateRequest.md) | GameCenterLeaderboardSetRelease representation |  |

### Return type

[**GameCenterLeaderboardSetReleaseResponse**](GameCenterLeaderboardSetReleaseResponse.md)

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
| **201** | Single GameCenterLeaderboardSetRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetreleasesdeleteinstance"></a>
# **GameCenterLeaderboardSetReleasesDeleteInstance**
> void GameCenterLeaderboardSetReleasesDeleteInstance (string id)




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

<a id="gamecenterleaderboardsetreleasesgetinstance"></a>
# **GameCenterLeaderboardSetReleasesGetInstance**
> GameCenterLeaderboardSetReleaseResponse GameCenterLeaderboardSetReleasesGetInstance (string id, List<string> fieldsGameCenterLeaderboardSetReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetReleaseResponse**](GameCenterLeaderboardSetReleaseResponse.md)

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
| **200** | Single GameCenterLeaderboardSetRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

