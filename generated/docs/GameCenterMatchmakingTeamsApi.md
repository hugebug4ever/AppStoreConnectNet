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
    public class GameCenterMatchmakingTeamsCreateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingTeamsApi(httpClient, config, httpClientHandler);
            var gameCenterMatchmakingTeamCreateRequest = new GameCenterMatchmakingTeamCreateRequest(); // GameCenterMatchmakingTeamCreateRequest | GameCenterMatchmakingTeam representation

            try
            {
                GameCenterMatchmakingTeamResponse result = apiInstance.GameCenterMatchmakingTeamsCreateInstance(gameCenterMatchmakingTeamCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingTeamsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingTeamResponse> response = apiInstance.GameCenterMatchmakingTeamsCreateInstanceWithHttpInfo(gameCenterMatchmakingTeamCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingteamsdeleteinstance"></a>
# **GameCenterMatchmakingTeamsDeleteInstance**
> void GameCenterMatchmakingTeamsDeleteInstance (string id)



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
    public class GameCenterMatchmakingTeamsDeleteInstanceExample
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
            var apiInstance = new GameCenterMatchmakingTeamsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterMatchmakingTeamsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingTeamsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterMatchmakingTeamsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsDeleteInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingteamsupdateinstance"></a>
# **GameCenterMatchmakingTeamsUpdateInstance**
> GameCenterMatchmakingTeamResponse GameCenterMatchmakingTeamsUpdateInstance (string id, GameCenterMatchmakingTeamUpdateRequest gameCenterMatchmakingTeamUpdateRequest)



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
    public class GameCenterMatchmakingTeamsUpdateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingTeamsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterMatchmakingTeamUpdateRequest = new GameCenterMatchmakingTeamUpdateRequest(); // GameCenterMatchmakingTeamUpdateRequest | GameCenterMatchmakingTeam representation

            try
            {
                GameCenterMatchmakingTeamResponse result = apiInstance.GameCenterMatchmakingTeamsUpdateInstance(id, gameCenterMatchmakingTeamUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingTeamsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingTeamResponse> response = apiInstance.GameCenterMatchmakingTeamsUpdateInstanceWithHttpInfo(id, gameCenterMatchmakingTeamUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingTeamsApi.GameCenterMatchmakingTeamsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

