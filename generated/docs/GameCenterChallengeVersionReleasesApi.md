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
    public class GameCenterChallengeVersionReleasesCreateInstanceExample
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
            var apiInstance = new GameCenterChallengeVersionReleasesApi(httpClient, config, httpClientHandler);
            var gameCenterChallengeVersionReleaseCreateRequest = new GameCenterChallengeVersionReleaseCreateRequest(); // GameCenterChallengeVersionReleaseCreateRequest | GameCenterChallengeVersionRelease representation

            try
            {
                GameCenterChallengeVersionReleaseResponse result = apiInstance.GameCenterChallengeVersionReleasesCreateInstance(gameCenterChallengeVersionReleaseCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionReleasesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionReleaseResponse> response = apiInstance.GameCenterChallengeVersionReleasesCreateInstanceWithHttpInfo(gameCenterChallengeVersionReleaseCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengeversionreleasesdeleteinstance"></a>
# **GameCenterChallengeVersionReleasesDeleteInstance**
> void GameCenterChallengeVersionReleasesDeleteInstance (string id)



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
    public class GameCenterChallengeVersionReleasesDeleteInstanceExample
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
            var apiInstance = new GameCenterChallengeVersionReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterChallengeVersionReleasesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionReleasesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterChallengeVersionReleasesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterchallengeversionreleasesgetinstance"></a>
# **GameCenterChallengeVersionReleasesGetInstance**
> GameCenterChallengeVersionReleaseResponse GameCenterChallengeVersionReleasesGetInstance (string id, List<string>? fieldsGameCenterChallengeVersionReleases = null, List<string>? include = null)



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
    public class GameCenterChallengeVersionReleasesGetInstanceExample
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
            var apiInstance = new GameCenterChallengeVersionReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeVersionReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterChallengeVersionReleaseResponse result = apiInstance.GameCenterChallengeVersionReleasesGetInstance(id, fieldsGameCenterChallengeVersionReleases, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionReleasesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionReleaseResponse> response = apiInstance.GameCenterChallengeVersionReleasesGetInstanceWithHttpInfo(id, fieldsGameCenterChallengeVersionReleases, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionReleasesApi.GameCenterChallengeVersionReleasesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

