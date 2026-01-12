# AppStoreConnect.Net.Api.GameCenterLeaderboardSetImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetImagesCreateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagescreateinstance) | **POST** /v1/gameCenterLeaderboardSetImages |  |
| [**GameCenterLeaderboardSetImagesDeleteInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesGetInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesgetinstance) | **GET** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesUpdateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2CreateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2createinstance) | **POST** /v2/gameCenterLeaderboardSetImages |  |
| [**GameCenterLeaderboardSetImagesV2DeleteInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2GetInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2getinstance) | **GET** /v2/gameCenterLeaderboardSetImages/{id} |  |
| [**GameCenterLeaderboardSetImagesV2UpdateInstance**](GameCenterLeaderboardSetImagesApi.md#gamecenterleaderboardsetimagesv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardSetImages/{id} |  |

<a id="gamecenterleaderboardsetimagescreateinstance"></a>
# **GameCenterLeaderboardSetImagesCreateInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesCreateInstance (GameCenterLeaderboardSetImageCreateRequest gameCenterLeaderboardSetImageCreateRequest)



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
    public class GameCenterLeaderboardSetImagesCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetImageCreateRequest = new GameCenterLeaderboardSetImageCreateRequest(); // GameCenterLeaderboardSetImageCreateRequest | GameCenterLeaderboardSetImage representation

            try
            {
                GameCenterLeaderboardSetImageResponse result = apiInstance.GameCenterLeaderboardSetImagesCreateInstance(gameCenterLeaderboardSetImageCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageResponse> response = apiInstance.GameCenterLeaderboardSetImagesCreateInstanceWithHttpInfo(gameCenterLeaderboardSetImageCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetImageCreateRequest** | [**GameCenterLeaderboardSetImageCreateRequest**](GameCenterLeaderboardSetImageCreateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **201** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetimagesdeleteinstance"></a>
# **GameCenterLeaderboardSetImagesDeleteInstance**
> void GameCenterLeaderboardSetImagesDeleteInstance (string id)



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
    public class GameCenterLeaderboardSetImagesDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetImagesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetImagesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetimagesgetinstance"></a>
# **GameCenterLeaderboardSetImagesGetInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesGetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetImagesGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetImageResponse result = apiInstance.GameCenterLeaderboardSetImagesGetInstance(id, fieldsGameCenterLeaderboardSetImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageResponse> response = apiInstance.GameCenterLeaderboardSetImagesGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetimagesupdateinstance"></a>
# **GameCenterLeaderboardSetImagesUpdateInstance**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetImagesUpdateInstance (string id, GameCenterLeaderboardSetImageUpdateRequest gameCenterLeaderboardSetImageUpdateRequest)



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
    public class GameCenterLeaderboardSetImagesUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetImageUpdateRequest = new GameCenterLeaderboardSetImageUpdateRequest(); // GameCenterLeaderboardSetImageUpdateRequest | GameCenterLeaderboardSetImage representation

            try
            {
                GameCenterLeaderboardSetImageResponse result = apiInstance.GameCenterLeaderboardSetImagesUpdateInstance(id, gameCenterLeaderboardSetImageUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageResponse> response = apiInstance.GameCenterLeaderboardSetImagesUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetImageUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetImageUpdateRequest** | [**GameCenterLeaderboardSetImageUpdateRequest**](GameCenterLeaderboardSetImageUpdateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetimagesv2createinstance"></a>
# **GameCenterLeaderboardSetImagesV2CreateInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2CreateInstance (GameCenterLeaderboardSetImageV2CreateRequest gameCenterLeaderboardSetImageV2CreateRequest)



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
    public class GameCenterLeaderboardSetImagesV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetImageV2CreateRequest = new GameCenterLeaderboardSetImageV2CreateRequest(); // GameCenterLeaderboardSetImageV2CreateRequest | GameCenterLeaderboardSetImage representation

            try
            {
                GameCenterLeaderboardSetImageV2Response result = apiInstance.GameCenterLeaderboardSetImagesV2CreateInstance(gameCenterLeaderboardSetImageV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageV2Response> response = apiInstance.GameCenterLeaderboardSetImagesV2CreateInstanceWithHttpInfo(gameCenterLeaderboardSetImageV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetImageV2CreateRequest** | [**GameCenterLeaderboardSetImageV2CreateRequest**](GameCenterLeaderboardSetImageV2CreateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetimagesv2deleteinstance"></a>
# **GameCenterLeaderboardSetImagesV2DeleteInstance**
> void GameCenterLeaderboardSetImagesV2DeleteInstance (string id)



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
    public class GameCenterLeaderboardSetImagesV2DeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetImagesV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetImagesV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetimagesv2getinstance"></a>
# **GameCenterLeaderboardSetImagesV2GetInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetImagesV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetImageV2Response result = apiInstance.GameCenterLeaderboardSetImagesV2GetInstance(id, fieldsGameCenterLeaderboardSetImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageV2Response> response = apiInstance.GameCenterLeaderboardSetImagesV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetimagesv2updateinstance"></a>
# **GameCenterLeaderboardSetImagesV2UpdateInstance**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetImagesV2UpdateInstance (string id, GameCenterLeaderboardSetImageV2UpdateRequest gameCenterLeaderboardSetImageV2UpdateRequest)



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
    public class GameCenterLeaderboardSetImagesV2UpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetImagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetImageV2UpdateRequest = new GameCenterLeaderboardSetImageV2UpdateRequest(); // GameCenterLeaderboardSetImageV2UpdateRequest | GameCenterLeaderboardSetImage representation

            try
            {
                GameCenterLeaderboardSetImageV2Response result = apiInstance.GameCenterLeaderboardSetImagesV2UpdateInstance(id, gameCenterLeaderboardSetImageV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetImagesV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageV2Response> response = apiInstance.GameCenterLeaderboardSetImagesV2UpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetImageV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetImagesApi.GameCenterLeaderboardSetImagesV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetImageV2UpdateRequest** | [**GameCenterLeaderboardSetImageV2UpdateRequest**](GameCenterLeaderboardSetImageV2UpdateRequest.md) | GameCenterLeaderboardSetImage representation |  |

### Return type

[**GameCenterLeaderboardSetImageV2Response**](GameCenterLeaderboardSetImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

