# AppStoreConnect.Net.Api.GameCenterMatchmakingTeamsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterMatchmakingTeamsCreateInstance**](GameCenterMatchmakingTeamsApi.md#gamecentermatchmakingteamscreateinstance) | **POST** /v1/gameCenterMatchmakingTeams |  |
| [**GameCenterMatchmakingTeamsDeleteInstance**](GameCenterMatchmakingTeamsApi.md#gamecentermatchmakingteamsdeleteinstance) | **DELETE** /v1/gameCenterMatchmakingTeams/{id} |  |
| [**GameCenterMatchmakingTeamsUpdateInstance**](GameCenterMatchmakingTeamsApi.md#gamecentermatchmakingteamsupdateinstance) | **PATCH** /v1/gameCenterMatchmakingTeams/{id} |  |

<a id="gamecentermatchmakingteamscreateinstance"></a>
# **GameCenterMatchmakingTeamsCreateInstance**
> GameCenterMatchmakingTeamResponse GameCenterMatchmakingTeamsCreateInstance (GameCenterMatchmakingTeamCreateRequest gameCenterMatchmakingTeamCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterMatchmakingTeamCreateRequest** | [**GameCenterMatchmakingTeamCreateRequest**](GameCenterMatchmakingTeamCreateRequest.md) | GameCenterMatchmakingTeam representation |  |

### Return type

[**GameCenterMatchmakingTeamResponse**](GameCenterMatchmakingTeamResponse.md)

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
| **201** | Single GameCenterMatchmakingTeam |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingteamsdeleteinstance"></a>
# **GameCenterMatchmakingTeamsDeleteInstance**
> void GameCenterMatchmakingTeamsDeleteInstance (string id)




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

<a id="gamecentermatchmakingteamsupdateinstance"></a>
# **GameCenterMatchmakingTeamsUpdateInstance**
> GameCenterMatchmakingTeamResponse GameCenterMatchmakingTeamsUpdateInstance (string id, GameCenterMatchmakingTeamUpdateRequest gameCenterMatchmakingTeamUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterMatchmakingTeamUpdateRequest** | [**GameCenterMatchmakingTeamUpdateRequest**](GameCenterMatchmakingTeamUpdateRequest.md) | GameCenterMatchmakingTeam representation |  |

### Return type

[**GameCenterMatchmakingTeamResponse**](GameCenterMatchmakingTeamResponse.md)

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
| **200** | Single GameCenterMatchmakingTeam |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

