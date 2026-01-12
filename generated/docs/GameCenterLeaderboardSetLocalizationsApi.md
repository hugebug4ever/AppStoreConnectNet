# AppStoreConnect.Net.Api.GameCenterLeaderboardSetLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetLocalizationsCreateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationscreateinstance) | **POST** /v1/gameCenterLeaderboardSetLocalizations |  |
| [**GameCenterLeaderboardSetLocalizationsDeleteInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelated) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id}/gameCenterLeaderboardSetImage |  |
| [**GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelationship) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id}/relationships/gameCenterLeaderboardSetImage |  |
| [**GameCenterLeaderboardSetLocalizationsGetInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsgetinstance) | **GET** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsUpdateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2CreateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2createinstance) | **POST** /v2/gameCenterLeaderboardSetLocalizations |  |
| [**GameCenterLeaderboardSetLocalizationsV2DeleteInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2GetInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2getinstance) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |
| [**GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id}/image |  |
| [**GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterLeaderboardSetLocalizations/{id}/relationships/image |  |
| [**GameCenterLeaderboardSetLocalizationsV2UpdateInstance**](GameCenterLeaderboardSetLocalizationsApi.md#gamecenterleaderboardsetlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardSetLocalizations/{id} |  |

<a id="gamecenterleaderboardsetlocalizationscreateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsCreateInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsCreateInstance (GameCenterLeaderboardSetLocalizationCreateRequest gameCenterLeaderboardSetLocalizationCreateRequest)



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
    public class GameCenterLeaderboardSetLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetLocalizationCreateRequest = new GameCenterLeaderboardSetLocalizationCreateRequest(); // GameCenterLeaderboardSetLocalizationCreateRequest | GameCenterLeaderboardSetLocalization representation

            try
            {
                GameCenterLeaderboardSetLocalizationResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsCreateInstance(gameCenterLeaderboardSetLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsCreateInstanceWithHttpInfo(gameCenterLeaderboardSetLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetLocalizationCreateRequest** | [**GameCenterLeaderboardSetLocalizationCreateRequest**](GameCenterLeaderboardSetLocalizationCreateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **201** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetlocalizationsdeleteinstance"></a>
# **GameCenterLeaderboardSetLocalizationsDeleteInstance**
> void GameCenterLeaderboardSetLocalizationsDeleteInstance (string id)



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
    public class GameCenterLeaderboardSetLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelated"></a>
# **GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated**
> GameCenterLeaderboardSetImageResponse GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetImageResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated(id, fieldsGameCenterLeaderboardSetImages, fieldsGameCenterLeaderboardSetLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSetImages, fieldsGameCenterLeaderboardSetLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
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

<a id="gamecenterleaderboardsetlocalizationsgamecenterleaderboardsetimagegettoonerelationship"></a>
# **GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship**
> GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGameCenterLeaderboardSetImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse**](GameCenterLeaderboardSetLocalizationGameCenterLeaderboardSetImageLinkageResponse.md)

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

<a id="gamecenterleaderboardsetlocalizationsgetinstance"></a>
# **GameCenterLeaderboardSetLocalizationsGetInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsGetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetLocalizationsGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetLocalizationResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsGetInstance(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetlocalizationsupdateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsUpdateInstance**
> GameCenterLeaderboardSetLocalizationResponse GameCenterLeaderboardSetLocalizationsUpdateInstance (string id, GameCenterLeaderboardSetLocalizationUpdateRequest gameCenterLeaderboardSetLocalizationUpdateRequest)



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
    public class GameCenterLeaderboardSetLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetLocalizationUpdateRequest = new GameCenterLeaderboardSetLocalizationUpdateRequest(); // GameCenterLeaderboardSetLocalizationUpdateRequest | GameCenterLeaderboardSetLocalization representation

            try
            {
                GameCenterLeaderboardSetLocalizationResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsUpdateInstance(id, gameCenterLeaderboardSetLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetLocalizationUpdateRequest** | [**GameCenterLeaderboardSetLocalizationUpdateRequest**](GameCenterLeaderboardSetLocalizationUpdateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationResponse**](GameCenterLeaderboardSetLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2createinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2CreateInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2CreateInstance (GameCenterLeaderboardSetLocalizationV2CreateRequest gameCenterLeaderboardSetLocalizationV2CreateRequest)



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
    public class GameCenterLeaderboardSetLocalizationsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetLocalizationV2CreateRequest = new GameCenterLeaderboardSetLocalizationV2CreateRequest(); // GameCenterLeaderboardSetLocalizationV2CreateRequest | GameCenterLeaderboardSetLocalization representation

            try
            {
                GameCenterLeaderboardSetLocalizationV2Response result = apiInstance.GameCenterLeaderboardSetLocalizationsV2CreateInstance(gameCenterLeaderboardSetLocalizationV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationV2Response> response = apiInstance.GameCenterLeaderboardSetLocalizationsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardSetLocalizationV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetLocalizationV2CreateRequest** | [**GameCenterLeaderboardSetLocalizationV2CreateRequest**](GameCenterLeaderboardSetLocalizationV2CreateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2deleteinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2DeleteInstance**
> void GameCenterLeaderboardSetLocalizationsV2DeleteInstance (string id)



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
    public class GameCenterLeaderboardSetLocalizationsV2DeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetLocalizationsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetLocalizationsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetlocalizationsv2getinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2GetInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetLocalizationsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetLocalizationV2Response result = apiInstance.GameCenterLeaderboardSetLocalizationsV2GetInstance(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationV2Response> response = apiInstance.GameCenterLeaderboardSetLocalizationsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetlocalizationsv2imagegettoonerelated"></a>
# **GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated**
> GameCenterLeaderboardSetImageV2Response GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardSetImages = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetImageV2Response result = apiInstance.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated(id, fieldsGameCenterLeaderboardSetImages, fieldsGameCenterLeaderboardSetLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetImageV2Response> response = apiInstance.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSetImages, fieldsGameCenterLeaderboardSetLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
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

<a id="gamecenterleaderboardsetlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship**
> GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse result = apiInstance.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse> response = apiInstance.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2ImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse**](GameCenterLeaderboardSetLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterleaderboardsetlocalizationsv2updateinstance"></a>
# **GameCenterLeaderboardSetLocalizationsV2UpdateInstance**
> GameCenterLeaderboardSetLocalizationV2Response GameCenterLeaderboardSetLocalizationsV2UpdateInstance (string id, GameCenterLeaderboardSetLocalizationV2UpdateRequest gameCenterLeaderboardSetLocalizationV2UpdateRequest)



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
    public class GameCenterLeaderboardSetLocalizationsV2UpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetLocalizationV2UpdateRequest = new GameCenterLeaderboardSetLocalizationV2UpdateRequest(); // GameCenterLeaderboardSetLocalizationV2UpdateRequest | GameCenterLeaderboardSetLocalization representation

            try
            {
                GameCenterLeaderboardSetLocalizationV2Response result = apiInstance.GameCenterLeaderboardSetLocalizationsV2UpdateInstance(id, gameCenterLeaderboardSetLocalizationV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetLocalizationsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationV2Response> response = apiInstance.GameCenterLeaderboardSetLocalizationsV2UpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetLocalizationV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetLocalizationsApi.GameCenterLeaderboardSetLocalizationsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetLocalizationV2UpdateRequest** | [**GameCenterLeaderboardSetLocalizationV2UpdateRequest**](GameCenterLeaderboardSetLocalizationV2UpdateRequest.md) | GameCenterLeaderboardSetLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetLocalizationV2Response**](GameCenterLeaderboardSetLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

