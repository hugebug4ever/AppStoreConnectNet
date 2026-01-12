# AppStoreConnect.Net.Api.GameCenterActivityLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityLocalizationsCreateInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationscreateinstance) | **POST** /v1/gameCenterActivityLocalizations |  |
| [**GameCenterActivityLocalizationsDeleteInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsdeleteinstance) | **DELETE** /v1/gameCenterActivityLocalizations/{id} |  |
| [**GameCenterActivityLocalizationsGetInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsgetinstance) | **GET** /v1/gameCenterActivityLocalizations/{id} |  |
| [**GameCenterActivityLocalizationsImageGetToOneRelated**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsimagegettoonerelated) | **GET** /v1/gameCenterActivityLocalizations/{id}/image |  |
| [**GameCenterActivityLocalizationsImageGetToOneRelationship**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsimagegettoonerelationship) | **GET** /v1/gameCenterActivityLocalizations/{id}/relationships/image |  |
| [**GameCenterActivityLocalizationsUpdateInstance**](GameCenterActivityLocalizationsApi.md#gamecenteractivitylocalizationsupdateinstance) | **PATCH** /v1/gameCenterActivityLocalizations/{id} |  |

<a id="gamecenteractivitylocalizationscreateinstance"></a>
# **GameCenterActivityLocalizationsCreateInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsCreateInstance (GameCenterActivityLocalizationCreateRequest gameCenterActivityLocalizationCreateRequest)



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
    public class GameCenterActivityLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterActivityLocalizationCreateRequest = new GameCenterActivityLocalizationCreateRequest(); // GameCenterActivityLocalizationCreateRequest | GameCenterActivityLocalization representation

            try
            {
                GameCenterActivityLocalizationResponse result = apiInstance.GameCenterActivityLocalizationsCreateInstance(gameCenterActivityLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityLocalizationResponse> response = apiInstance.GameCenterActivityLocalizationsCreateInstanceWithHttpInfo(gameCenterActivityLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityLocalizationCreateRequest** | [**GameCenterActivityLocalizationCreateRequest**](GameCenterActivityLocalizationCreateRequest.md) | GameCenterActivityLocalization representation |  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **201** | Single GameCenterActivityLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivitylocalizationsdeleteinstance"></a>
# **GameCenterActivityLocalizationsDeleteInstance**
> void GameCenterActivityLocalizationsDeleteInstance (string id)



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
    public class GameCenterActivityLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterActivityLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterActivityLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenteractivitylocalizationsgetinstance"></a>
# **GameCenterActivityLocalizationsGetInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsGetInstance (string id, List<string>? fieldsGameCenterActivityLocalizations = null, List<string>? fieldsGameCenterActivityImages = null, List<string>? include = null)



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
    public class GameCenterActivityLocalizationsGetInstanceExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityLocalizations (optional) 
            var fieldsGameCenterActivityImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterActivityLocalizationResponse result = apiInstance.GameCenterActivityLocalizationsGetInstance(id, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityLocalizationResponse> response = apiInstance.GameCenterActivityLocalizationsGetInstanceWithHttpInfo(id, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **200** | Single GameCenterActivityLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivitylocalizationsimagegettoonerelated"></a>
# **GameCenterActivityLocalizationsImageGetToOneRelated**
> GameCenterActivityImageResponse GameCenterActivityLocalizationsImageGetToOneRelated (string id, List<string>? fieldsGameCenterActivityImages = null)



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
    public class GameCenterActivityLocalizationsImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityImages (optional) 

            try
            {
                GameCenterActivityImageResponse result = apiInstance.GameCenterActivityLocalizationsImageGetToOneRelated(id, fieldsGameCenterActivityImages);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityImageResponse> response = apiInstance.GameCenterActivityLocalizationsImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterActivityImages);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |

### Return type

[**GameCenterActivityImageResponse**](GameCenterActivityImageResponse.md)

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
| **200** | Single GameCenterActivityImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivitylocalizationsimagegettoonerelationship"></a>
# **GameCenterActivityLocalizationsImageGetToOneRelationship**
> GameCenterActivityLocalizationImageLinkageResponse GameCenterActivityLocalizationsImageGetToOneRelationship (string id)



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
    public class GameCenterActivityLocalizationsImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterActivityLocalizationImageLinkageResponse result = apiInstance.GameCenterActivityLocalizationsImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityLocalizationImageLinkageResponse> response = apiInstance.GameCenterActivityLocalizationsImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterActivityLocalizationImageLinkageResponse**](GameCenterActivityLocalizationImageLinkageResponse.md)

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
| **200** | Related linkage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivitylocalizationsupdateinstance"></a>
# **GameCenterActivityLocalizationsUpdateInstance**
> GameCenterActivityLocalizationResponse GameCenterActivityLocalizationsUpdateInstance (string id, GameCenterActivityLocalizationUpdateRequest gameCenterActivityLocalizationUpdateRequest)



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
    public class GameCenterActivityLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterActivityLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterActivityLocalizationUpdateRequest = new GameCenterActivityLocalizationUpdateRequest(); // GameCenterActivityLocalizationUpdateRequest | GameCenterActivityLocalization representation

            try
            {
                GameCenterActivityLocalizationResponse result = apiInstance.GameCenterActivityLocalizationsUpdateInstance(id, gameCenterActivityLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityLocalizationResponse> response = apiInstance.GameCenterActivityLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterActivityLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityLocalizationsApi.GameCenterActivityLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLocalizationUpdateRequest** | [**GameCenterActivityLocalizationUpdateRequest**](GameCenterActivityLocalizationUpdateRequest.md) | GameCenterActivityLocalization representation |  |

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
| **200** | Single GameCenterActivityLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

