# AppStoreConnect.Net.Api.GameCenterChallengeVersionReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeVersionReleasesCreateInstance**](GameCenterChallengeVersionReleasesApi.md#gamecenterchallengeversionreleasescreateinstance) | **POST** /v1/gameCenterChallengeVersionReleases |  |
| [**GameCenterChallengeVersionReleasesDeleteInstance**](GameCenterChallengeVersionReleasesApi.md#gamecenterchallengeversionreleasesdeleteinstance) | **DELETE** /v1/gameCenterChallengeVersionReleases/{id} |  |
| [**GameCenterChallengeVersionReleasesGetInstance**](GameCenterChallengeVersionReleasesApi.md#gamecenterchallengeversionreleasesgetinstance) | **GET** /v1/gameCenterChallengeVersionReleases/{id} |  |

<a id="gamecenterchallengeversionreleasescreateinstance"></a>
# **GameCenterChallengeVersionReleasesCreateInstance**
> GameCenterChallengeVersionReleaseResponse GameCenterChallengeVersionReleasesCreateInstance (GameCenterChallengeVersionReleaseCreateRequest gameCenterChallengeVersionReleaseCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeVersionReleaseCreateRequest** | [**GameCenterChallengeVersionReleaseCreateRequest**](GameCenterChallengeVersionReleaseCreateRequest.md) | GameCenterChallengeVersionRelease representation |  |

### Return type

[**GameCenterChallengeVersionReleaseResponse**](GameCenterChallengeVersionReleaseResponse.md)

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
| **201** | Single GameCenterChallengeVersionRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengeversionreleasesdeleteinstance"></a>
# **GameCenterChallengeVersionReleasesDeleteInstance**
> void GameCenterChallengeVersionReleasesDeleteInstance (string id)




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

<a id="gamecenterchallengeversionreleasesgetinstance"></a>
# **GameCenterChallengeVersionReleasesGetInstance**
> GameCenterChallengeVersionReleaseResponse GameCenterChallengeVersionReleasesGetInstance (string id, List<string> fieldsGameCenterChallengeVersionReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterChallengeVersionReleaseResponse**](GameCenterChallengeVersionReleaseResponse.md)

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
| **200** | Single GameCenterChallengeVersionRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

