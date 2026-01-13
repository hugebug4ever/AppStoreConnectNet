# AppStoreConnect.Net.Api.GameCenterLeaderboardEntrySubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardEntrySubmissionsCreateInstance**](GameCenterLeaderboardEntrySubmissionsApi.md#gamecenterleaderboardentrysubmissionscreateinstance) | **POST** /v1/gameCenterLeaderboardEntrySubmissions |  |

<a id="gamecenterleaderboardentrysubmissionscreateinstance"></a>
# **GameCenterLeaderboardEntrySubmissionsCreateInstance**
> GameCenterLeaderboardEntrySubmissionResponse GameCenterLeaderboardEntrySubmissionsCreateInstance (GameCenterLeaderboardEntrySubmissionCreateRequest gameCenterLeaderboardEntrySubmissionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardEntrySubmissionCreateRequest** | [**GameCenterLeaderboardEntrySubmissionCreateRequest**](GameCenterLeaderboardEntrySubmissionCreateRequest.md) | GameCenterLeaderboardEntrySubmission representation |  |

### Return type

[**GameCenterLeaderboardEntrySubmissionResponse**](GameCenterLeaderboardEntrySubmissionResponse.md)

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
| **201** | Single GameCenterLeaderboardEntrySubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

