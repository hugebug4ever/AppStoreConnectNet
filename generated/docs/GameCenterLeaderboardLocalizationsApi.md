# AppStoreConnect.Net.Api.GameCenterLeaderboardLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardLocalizationsCreateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationscreateinstance) | **POST** /v1/gameCenterLeaderboardLocalizations |  |
| [**GameCenterLeaderboardLocalizationsDeleteInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelated) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/gameCenterLeaderboardImage |  |
| [**GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelationship) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/relationships/gameCenterLeaderboardImage |  |
| [**GameCenterLeaderboardLocalizationsGetInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsgetinstance) | **GET** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsUpdateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2CreateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2createinstance) | **POST** /v2/gameCenterLeaderboardLocalizations |  |
| [**GameCenterLeaderboardLocalizationsV2DeleteInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2GetInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2getinstance) | **GET** /v2/gameCenterLeaderboardLocalizations/{id} |  |
| [**GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterLeaderboardLocalizations/{id}/image |  |
| [**GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterLeaderboardLocalizations/{id}/relationships/image |  |
| [**GameCenterLeaderboardLocalizationsV2UpdateInstance**](GameCenterLeaderboardLocalizationsApi.md#gamecenterleaderboardlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardLocalizations/{id} |  |

<a id="gamecenterleaderboardlocalizationscreateinstance"></a>
# **GameCenterLeaderboardLocalizationsCreateInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsCreateInstance (GameCenterLeaderboardLocalizationCreateRequest gameCenterLeaderboardLocalizationCreateRequest)



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
    public class GameCenterLeaderboardLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardLocalizationCreateRequest = new GameCenterLeaderboardLocalizationCreateRequest(); // GameCenterLeaderboardLocalizationCreateRequest | GameCenterLeaderboardLocalization representation

            try
            {
                GameCenterLeaderboardLocalizationResponse result = apiInstance.GameCenterLeaderboardLocalizationsCreateInstance(gameCenterLeaderboardLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationResponse> response = apiInstance.GameCenterLeaderboardLocalizationsCreateInstanceWithHttpInfo(gameCenterLeaderboardLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardLocalizationCreateRequest** | [**GameCenterLeaderboardLocalizationCreateRequest**](GameCenterLeaderboardLocalizationCreateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **201** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsdeleteinstance"></a>
# **GameCenterLeaderboardLocalizationsDeleteInstance**
> void GameCenterLeaderboardLocalizationsDeleteInstance (string id)



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
    public class GameCenterLeaderboardLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelated"></a>
# **GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated**
> GameCenterLeaderboardImageResponse GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardImages = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? include = null)



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
    public class GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardImageResponse result = apiInstance.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated(id, fieldsGameCenterLeaderboardImages, fieldsGameCenterLeaderboardLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardImageResponse> response = apiInstance.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardImages, fieldsGameCenterLeaderboardLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardImageResponse**](GameCenterLeaderboardImageResponse.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsgamecenterleaderboardimagegettoonerelationship"></a>
# **GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship**
> GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse result = apiInstance.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse> response = apiInstance.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGameCenterLeaderboardImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse**](GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse.md)

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

<a id="gamecenterleaderboardlocalizationsgetinstance"></a>
# **GameCenterLeaderboardLocalizationsGetInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsGetInstance (string id, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardLocalizationsGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardLocalizationResponse result = apiInstance.GameCenterLeaderboardLocalizationsGetInstance(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationResponse> response = apiInstance.GameCenterLeaderboardLocalizationsGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsupdateinstance"></a>
# **GameCenterLeaderboardLocalizationsUpdateInstance**
> GameCenterLeaderboardLocalizationResponse GameCenterLeaderboardLocalizationsUpdateInstance (string id, GameCenterLeaderboardLocalizationUpdateRequest gameCenterLeaderboardLocalizationUpdateRequest)



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
    public class GameCenterLeaderboardLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardLocalizationUpdateRequest = new GameCenterLeaderboardLocalizationUpdateRequest(); // GameCenterLeaderboardLocalizationUpdateRequest | GameCenterLeaderboardLocalization representation

            try
            {
                GameCenterLeaderboardLocalizationResponse result = apiInstance.GameCenterLeaderboardLocalizationsUpdateInstance(id, gameCenterLeaderboardLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationResponse> response = apiInstance.GameCenterLeaderboardLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardLocalizationUpdateRequest** | [**GameCenterLeaderboardLocalizationUpdateRequest**](GameCenterLeaderboardLocalizationUpdateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsv2createinstance"></a>
# **GameCenterLeaderboardLocalizationsV2CreateInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2CreateInstance (GameCenterLeaderboardLocalizationV2CreateRequest gameCenterLeaderboardLocalizationV2CreateRequest)



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
    public class GameCenterLeaderboardLocalizationsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardLocalizationV2CreateRequest = new GameCenterLeaderboardLocalizationV2CreateRequest(); // GameCenterLeaderboardLocalizationV2CreateRequest | GameCenterLeaderboardLocalization representation

            try
            {
                GameCenterLeaderboardLocalizationV2Response result = apiInstance.GameCenterLeaderboardLocalizationsV2CreateInstance(gameCenterLeaderboardLocalizationV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationV2Response> response = apiInstance.GameCenterLeaderboardLocalizationsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardLocalizationV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardLocalizationV2CreateRequest** | [**GameCenterLeaderboardLocalizationV2CreateRequest**](GameCenterLeaderboardLocalizationV2CreateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **201** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsv2deleteinstance"></a>
# **GameCenterLeaderboardLocalizationsV2DeleteInstance**
> void GameCenterLeaderboardLocalizationsV2DeleteInstance (string id)



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
    public class GameCenterLeaderboardLocalizationsV2DeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardLocalizationsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardLocalizationsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardlocalizationsv2getinstance"></a>
# **GameCenterLeaderboardLocalizationsV2GetInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardImages = null, List<string>? include = null)



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
    public class GameCenterLeaderboardLocalizationsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardLocalizationV2Response result = apiInstance.GameCenterLeaderboardLocalizationsV2GetInstance(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationV2Response> response = apiInstance.GameCenterLeaderboardLocalizationsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsv2imagegettoonerelated"></a>
# **GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated**
> GameCenterLeaderboardImageV2Response GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardImages = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? include = null)



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
    public class GameCenterLeaderboardLocalizationsV2ImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardImageV2Response result = apiInstance.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated(id, fieldsGameCenterLeaderboardImages, fieldsGameCenterLeaderboardLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2ImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardImageV2Response> response = apiInstance.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardImages, fieldsGameCenterLeaderboardLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardImageV2Response**](GameCenterLeaderboardImageV2Response.md)

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
| **200** | Single GameCenterLeaderboardImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship**
> GameCenterLeaderboardLocalizationV2ImageLinkageResponse GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardLocalizationV2ImageLinkageResponse result = apiInstance.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationV2ImageLinkageResponse> response = apiInstance.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2ImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardLocalizationV2ImageLinkageResponse**](GameCenterLeaderboardLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterleaderboardlocalizationsv2updateinstance"></a>
# **GameCenterLeaderboardLocalizationsV2UpdateInstance**
> GameCenterLeaderboardLocalizationV2Response GameCenterLeaderboardLocalizationsV2UpdateInstance (string id, GameCenterLeaderboardLocalizationV2UpdateRequest gameCenterLeaderboardLocalizationV2UpdateRequest)



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
    public class GameCenterLeaderboardLocalizationsV2UpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardLocalizationV2UpdateRequest = new GameCenterLeaderboardLocalizationV2UpdateRequest(); // GameCenterLeaderboardLocalizationV2UpdateRequest | GameCenterLeaderboardLocalization representation

            try
            {
                GameCenterLeaderboardLocalizationV2Response result = apiInstance.GameCenterLeaderboardLocalizationsV2UpdateInstance(id, gameCenterLeaderboardLocalizationV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardLocalizationsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationV2Response> response = apiInstance.GameCenterLeaderboardLocalizationsV2UpdateInstanceWithHttpInfo(id, gameCenterLeaderboardLocalizationV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardLocalizationsApi.GameCenterLeaderboardLocalizationsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardLocalizationV2UpdateRequest** | [**GameCenterLeaderboardLocalizationV2UpdateRequest**](GameCenterLeaderboardLocalizationV2UpdateRequest.md) | GameCenterLeaderboardLocalization representation |  |

### Return type

[**GameCenterLeaderboardLocalizationV2Response**](GameCenterLeaderboardLocalizationV2Response.md)

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
| **200** | Single GameCenterLeaderboardLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

