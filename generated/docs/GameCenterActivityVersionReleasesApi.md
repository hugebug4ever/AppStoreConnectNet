# AppStoreConnect.Net.Api.GameCenterActivityVersionReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityVersionReleasesCreateInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasescreateinstance) | **POST** /v1/gameCenterActivityVersionReleases |  |
| [**GameCenterActivityVersionReleasesDeleteInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasesdeleteinstance) | **DELETE** /v1/gameCenterActivityVersionReleases/{id} |  |
| [**GameCenterActivityVersionReleasesGetInstance**](GameCenterActivityVersionReleasesApi.md#gamecenteractivityversionreleasesgetinstance) | **GET** /v1/gameCenterActivityVersionReleases/{id} |  |

<a id="gamecenteractivityversionreleasescreateinstance"></a>
# **GameCenterActivityVersionReleasesCreateInstance**
> GameCenterActivityVersionReleaseResponse GameCenterActivityVersionReleasesCreateInstance (GameCenterActivityVersionReleaseCreateRequest gameCenterActivityVersionReleaseCreateRequest)



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
    public class GameCenterActivityVersionReleasesCreateInstanceExample
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
            var apiInstance = new GameCenterActivityVersionReleasesApi(httpClient, config, httpClientHandler);
            var gameCenterActivityVersionReleaseCreateRequest = new GameCenterActivityVersionReleaseCreateRequest(); // GameCenterActivityVersionReleaseCreateRequest | GameCenterActivityVersionRelease representation

            try
            {
                GameCenterActivityVersionReleaseResponse result = apiInstance.GameCenterActivityVersionReleasesCreateInstance(gameCenterActivityVersionReleaseCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionReleasesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionReleaseResponse> response = apiInstance.GameCenterActivityVersionReleasesCreateInstanceWithHttpInfo(gameCenterActivityVersionReleaseCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityVersionReleaseCreateRequest** | [**GameCenterActivityVersionReleaseCreateRequest**](GameCenterActivityVersionReleaseCreateRequest.md) | GameCenterActivityVersionRelease representation |  |

### Return type

[**GameCenterActivityVersionReleaseResponse**](GameCenterActivityVersionReleaseResponse.md)

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
| **201** | Single GameCenterActivityVersionRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivityversionreleasesdeleteinstance"></a>
# **GameCenterActivityVersionReleasesDeleteInstance**
> void GameCenterActivityVersionReleasesDeleteInstance (string id)



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
    public class GameCenterActivityVersionReleasesDeleteInstanceExample
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
            var apiInstance = new GameCenterActivityVersionReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterActivityVersionReleasesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionReleasesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterActivityVersionReleasesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenteractivityversionreleasesgetinstance"></a>
# **GameCenterActivityVersionReleasesGetInstance**
> GameCenterActivityVersionReleaseResponse GameCenterActivityVersionReleasesGetInstance (string id, List<string>? fieldsGameCenterActivityVersionReleases = null, List<string>? include = null)



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
    public class GameCenterActivityVersionReleasesGetInstanceExample
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
            var apiInstance = new GameCenterActivityVersionReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityVersionReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityVersionReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterActivityVersionReleaseResponse result = apiInstance.GameCenterActivityVersionReleasesGetInstance(id, fieldsGameCenterActivityVersionReleases, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionReleasesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionReleaseResponse> response = apiInstance.GameCenterActivityVersionReleasesGetInstanceWithHttpInfo(id, fieldsGameCenterActivityVersionReleases, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionReleasesApi.GameCenterActivityVersionReleasesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityVersionReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityVersionReleaseResponse**](GameCenterActivityVersionReleaseResponse.md)

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
| **200** | Single GameCenterActivityVersionRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

