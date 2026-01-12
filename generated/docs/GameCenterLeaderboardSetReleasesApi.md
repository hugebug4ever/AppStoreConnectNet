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
    public class GameCenterLeaderboardSetReleasesCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetReleasesApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetReleaseCreateRequest = new GameCenterLeaderboardSetReleaseCreateRequest(); // GameCenterLeaderboardSetReleaseCreateRequest | GameCenterLeaderboardSetRelease representation

            try
            {
                GameCenterLeaderboardSetReleaseResponse result = apiInstance.GameCenterLeaderboardSetReleasesCreateInstance(gameCenterLeaderboardSetReleaseCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetReleasesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetReleaseResponse> response = apiInstance.GameCenterLeaderboardSetReleasesCreateInstanceWithHttpInfo(gameCenterLeaderboardSetReleaseCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetreleasesdeleteinstance"></a>
# **GameCenterLeaderboardSetReleasesDeleteInstance**
> void GameCenterLeaderboardSetReleasesDeleteInstance (string id)



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
    public class GameCenterLeaderboardSetReleasesDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetReleasesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetReleasesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetReleasesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetreleasesgetinstance"></a>
# **GameCenterLeaderboardSetReleasesGetInstance**
> GameCenterLeaderboardSetReleaseResponse GameCenterLeaderboardSetReleasesGetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetReleasesGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetReleaseResponse result = apiInstance.GameCenterLeaderboardSetReleasesGetInstance(id, fieldsGameCenterLeaderboardSetReleases, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetReleasesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetReleaseResponse> response = apiInstance.GameCenterLeaderboardSetReleasesGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetReleases, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetReleasesApi.GameCenterLeaderboardSetReleasesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

