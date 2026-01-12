# AppStoreConnect.Net.Api.GameCenterLeaderboardEntrySubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardEntrySubmissionsCreateInstance**](GameCenterLeaderboardEntrySubmissionsApi.md#gamecenterleaderboardentrysubmissionscreateinstance) | **POST** /v1/gameCenterLeaderboardEntrySubmissions |  |

<a id="gamecenterleaderboardentrysubmissionscreateinstance"></a>
# **GameCenterLeaderboardEntrySubmissionsCreateInstance**
> GameCenterLeaderboardEntrySubmissionResponse GameCenterLeaderboardEntrySubmissionsCreateInstance (GameCenterLeaderboardEntrySubmissionCreateRequest gameCenterLeaderboardEntrySubmissionCreateRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterLeaderboardEntrySubmissionsCreateInstanceExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterLeaderboardEntrySubmissionsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardEntrySubmissionCreateRequest = new GameCenterLeaderboardEntrySubmissionCreateRequest(); // GameCenterLeaderboardEntrySubmissionCreateRequest | GameCenterLeaderboardEntrySubmission representation

            try
            {
                GameCenterLeaderboardEntrySubmissionResponse result = apiInstance.GameCenterLeaderboardEntrySubmissionsCreateInstance(gameCenterLeaderboardEntrySubmissionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardEntrySubmissionsApi.GameCenterLeaderboardEntrySubmissionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardEntrySubmissionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardEntrySubmissionResponse> response = apiInstance.GameCenterLeaderboardEntrySubmissionsCreateInstanceWithHttpInfo(gameCenterLeaderboardEntrySubmissionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardEntrySubmissionsApi.GameCenterLeaderboardEntrySubmissionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

