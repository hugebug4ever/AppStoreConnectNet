# AppStoreConnect.Net.Api.GameCenterPlayerAchievementSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterPlayerAchievementSubmissionsCreateInstance**](GameCenterPlayerAchievementSubmissionsApi.md#gamecenterplayerachievementsubmissionscreateinstance) | **POST** /v1/gameCenterPlayerAchievementSubmissions |  |

<a id="gamecenterplayerachievementsubmissionscreateinstance"></a>
# **GameCenterPlayerAchievementSubmissionsCreateInstance**
> GameCenterPlayerAchievementSubmissionResponse GameCenterPlayerAchievementSubmissionsCreateInstance (GameCenterPlayerAchievementSubmissionCreateRequest gameCenterPlayerAchievementSubmissionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterPlayerAchievementSubmissionCreateRequest** | [**GameCenterPlayerAchievementSubmissionCreateRequest**](GameCenterPlayerAchievementSubmissionCreateRequest.md) | GameCenterPlayerAchievementSubmission representation |  |

### Return type

[**GameCenterPlayerAchievementSubmissionResponse**](GameCenterPlayerAchievementSubmissionResponse.md)

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
| **201** | Single GameCenterPlayerAchievementSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

