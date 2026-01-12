# AppStoreConnect.Net.Api.GameCenterChallengeLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeLocalizationsCreateInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationscreateinstance) | **POST** /v1/gameCenterChallengeLocalizations |  |
| [**GameCenterChallengeLocalizationsDeleteInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsdeleteinstance) | **DELETE** /v1/gameCenterChallengeLocalizations/{id} |  |
| [**GameCenterChallengeLocalizationsGetInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsgetinstance) | **GET** /v1/gameCenterChallengeLocalizations/{id} |  |
| [**GameCenterChallengeLocalizationsImageGetToOneRelated**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsimagegettoonerelated) | **GET** /v1/gameCenterChallengeLocalizations/{id}/image |  |
| [**GameCenterChallengeLocalizationsImageGetToOneRelationship**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsimagegettoonerelationship) | **GET** /v1/gameCenterChallengeLocalizations/{id}/relationships/image |  |
| [**GameCenterChallengeLocalizationsUpdateInstance**](GameCenterChallengeLocalizationsApi.md#gamecenterchallengelocalizationsupdateinstance) | **PATCH** /v1/gameCenterChallengeLocalizations/{id} |  |

<a id="gamecenterchallengelocalizationscreateinstance"></a>
# **GameCenterChallengeLocalizationsCreateInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsCreateInstance (GameCenterChallengeLocalizationCreateRequest gameCenterChallengeLocalizationCreateRequest)



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
    public class GameCenterChallengeLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterChallengeLocalizationCreateRequest = new GameCenterChallengeLocalizationCreateRequest(); // GameCenterChallengeLocalizationCreateRequest | GameCenterChallengeLocalization representation

            try
            {
                GameCenterChallengeLocalizationResponse result = apiInstance.GameCenterChallengeLocalizationsCreateInstance(gameCenterChallengeLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeLocalizationResponse> response = apiInstance.GameCenterChallengeLocalizationsCreateInstanceWithHttpInfo(gameCenterChallengeLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeLocalizationCreateRequest** | [**GameCenterChallengeLocalizationCreateRequest**](GameCenterChallengeLocalizationCreateRequest.md) | GameCenterChallengeLocalization representation |  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **201** | Single GameCenterChallengeLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengelocalizationsdeleteinstance"></a>
# **GameCenterChallengeLocalizationsDeleteInstance**
> void GameCenterChallengeLocalizationsDeleteInstance (string id)



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
    public class GameCenterChallengeLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterChallengeLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterChallengeLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterchallengelocalizationsgetinstance"></a>
# **GameCenterChallengeLocalizationsGetInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsGetInstance (string id, List<string>? fieldsGameCenterChallengeLocalizations = null, List<string>? fieldsGameCenterChallengeImages = null, List<string>? include = null)



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
    public class GameCenterChallengeLocalizationsGetInstanceExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional) 
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterChallengeLocalizationResponse result = apiInstance.GameCenterChallengeLocalizationsGetInstance(id, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeLocalizationResponse> response = apiInstance.GameCenterChallengeLocalizationsGetInstanceWithHttpInfo(id, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **200** | Single GameCenterChallengeLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengelocalizationsimagegettoonerelated"></a>
# **GameCenterChallengeLocalizationsImageGetToOneRelated**
> GameCenterChallengeImageResponse GameCenterChallengeLocalizationsImageGetToOneRelated (string id, List<string>? fieldsGameCenterChallengeImages = null)



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
    public class GameCenterChallengeLocalizationsImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 

            try
            {
                GameCenterChallengeImageResponse result = apiInstance.GameCenterChallengeLocalizationsImageGetToOneRelated(id, fieldsGameCenterChallengeImages);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeImageResponse> response = apiInstance.GameCenterChallengeLocalizationsImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterChallengeImages);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |

### Return type

[**GameCenterChallengeImageResponse**](GameCenterChallengeImageResponse.md)

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
| **200** | Single GameCenterChallengeImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengelocalizationsimagegettoonerelationship"></a>
# **GameCenterChallengeLocalizationsImageGetToOneRelationship**
> GameCenterChallengeLocalizationImageLinkageResponse GameCenterChallengeLocalizationsImageGetToOneRelationship (string id)



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
    public class GameCenterChallengeLocalizationsImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterChallengeLocalizationImageLinkageResponse result = apiInstance.GameCenterChallengeLocalizationsImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeLocalizationImageLinkageResponse> response = apiInstance.GameCenterChallengeLocalizationsImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterChallengeLocalizationImageLinkageResponse**](GameCenterChallengeLocalizationImageLinkageResponse.md)

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

<a id="gamecenterchallengelocalizationsupdateinstance"></a>
# **GameCenterChallengeLocalizationsUpdateInstance**
> GameCenterChallengeLocalizationResponse GameCenterChallengeLocalizationsUpdateInstance (string id, GameCenterChallengeLocalizationUpdateRequest gameCenterChallengeLocalizationUpdateRequest)



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
    public class GameCenterChallengeLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterChallengeLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterChallengeLocalizationUpdateRequest = new GameCenterChallengeLocalizationUpdateRequest(); // GameCenterChallengeLocalizationUpdateRequest | GameCenterChallengeLocalization representation

            try
            {
                GameCenterChallengeLocalizationResponse result = apiInstance.GameCenterChallengeLocalizationsUpdateInstance(id, gameCenterChallengeLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeLocalizationResponse> response = apiInstance.GameCenterChallengeLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterChallengeLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeLocalizationsApi.GameCenterChallengeLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeLocalizationUpdateRequest** | [**GameCenterChallengeLocalizationUpdateRequest**](GameCenterChallengeLocalizationUpdateRequest.md) | GameCenterChallengeLocalization representation |  |

### Return type

[**GameCenterChallengeLocalizationResponse**](GameCenterChallengeLocalizationResponse.md)

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
| **200** | Single GameCenterChallengeLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

