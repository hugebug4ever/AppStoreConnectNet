# AppStoreConnect.Net.Api.GameCenterAchievementLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementLocalizationsCreateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationscreateinstance) | **POST** /v1/gameCenterAchievementLocalizations |  |
| [**GameCenterAchievementLocalizationsDeleteInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementgettoonerelated) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievement |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementgettoonerelationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievement |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelated) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievementImage |  |
| [**GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievementImage |  |
| [**GameCenterAchievementLocalizationsGetInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsgetinstance) | **GET** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsUpdateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsupdateinstance) | **PATCH** /v1/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2CreateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2createinstance) | **POST** /v2/gameCenterAchievementLocalizations |  |
| [**GameCenterAchievementLocalizationsV2DeleteInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2deleteinstance) | **DELETE** /v2/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2GetInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2getinstance) | **GET** /v2/gameCenterAchievementLocalizations/{id} |  |
| [**GameCenterAchievementLocalizationsV2ImageGetToOneRelated**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2imagegettoonerelated) | **GET** /v2/gameCenterAchievementLocalizations/{id}/image |  |
| [**GameCenterAchievementLocalizationsV2ImageGetToOneRelationship**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2imagegettoonerelationship) | **GET** /v2/gameCenterAchievementLocalizations/{id}/relationships/image |  |
| [**GameCenterAchievementLocalizationsV2UpdateInstance**](GameCenterAchievementLocalizationsApi.md#gamecenterachievementlocalizationsv2updateinstance) | **PATCH** /v2/gameCenterAchievementLocalizations/{id} |  |

<a id="gamecenterachievementlocalizationscreateinstance"></a>
# **GameCenterAchievementLocalizationsCreateInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsCreateInstance (GameCenterAchievementLocalizationCreateRequest gameCenterAchievementLocalizationCreateRequest)



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
    public class GameCenterAchievementLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterAchievementLocalizationCreateRequest = new GameCenterAchievementLocalizationCreateRequest(); // GameCenterAchievementLocalizationCreateRequest | GameCenterAchievementLocalization representation

            try
            {
                GameCenterAchievementLocalizationResponse result = apiInstance.GameCenterAchievementLocalizationsCreateInstance(gameCenterAchievementLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationResponse> response = apiInstance.GameCenterAchievementLocalizationsCreateInstanceWithHttpInfo(gameCenterAchievementLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementLocalizationCreateRequest** | [**GameCenterAchievementLocalizationCreateRequest**](GameCenterAchievementLocalizationCreateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **201** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsdeleteinstance"></a>
# **GameCenterAchievementLocalizationsDeleteInstance**
> void GameCenterAchievementLocalizationsDeleteInstance (string id)



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
    public class GameCenterAchievementLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterAchievementLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterAchievementLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterachievementlocalizationsgamecenterachievementgettoonerelated"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated**
> GameCenterAchievementResponse GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated (string id, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? fieldsGameCenterAchievementReleases = null, List<string>? fieldsGameCenterActivities = null, List<string>? include = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelatedExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var fieldsGameCenterAchievementReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementReleases (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterAchievementResponse result = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated(id, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementReleases, fieldsGameCenterActivities, include, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementResponse> response = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelatedWithHttpInfo(id, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementReleases, fieldsGameCenterActivities, include, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsgamecenterachievementgettoonerelationship"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship**
> GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship (string id)



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
    public class GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationshipExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse result = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse> response = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelated"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated**
> GameCenterAchievementImageResponse GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated (string id, List<string>? fieldsGameCenterAchievementImages = null, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? include = null)



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
    public class GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementImages (optional) 
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterAchievementImageResponse result = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated(id, fieldsGameCenterAchievementImages, fieldsGameCenterAchievementLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementImageResponse> response = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterAchievementImages, fieldsGameCenterAchievementLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementImageResponse**](GameCenterAchievementImageResponse.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsgamecenterachievementimagegettoonerelationship"></a>
# **GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship**
> GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship (string id)



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
    public class GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse result = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse> response = apiInstance.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGameCenterAchievementImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsgetinstance"></a>
# **GameCenterAchievementLocalizationsGetInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsGetInstance (string id, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterAchievementImages = null, List<string>? include = null)



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
    public class GameCenterAchievementLocalizationsGetInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterAchievementImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterAchievementLocalizationResponse result = apiInstance.GameCenterAchievementLocalizationsGetInstance(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievements, fieldsGameCenterAchievementImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationResponse> response = apiInstance.GameCenterAchievementLocalizationsGetInstanceWithHttpInfo(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievements, fieldsGameCenterAchievementImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsupdateinstance"></a>
# **GameCenterAchievementLocalizationsUpdateInstance**
> GameCenterAchievementLocalizationResponse GameCenterAchievementLocalizationsUpdateInstance (string id, GameCenterAchievementLocalizationUpdateRequest gameCenterAchievementLocalizationUpdateRequest)



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
    public class GameCenterAchievementLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterAchievementLocalizationUpdateRequest = new GameCenterAchievementLocalizationUpdateRequest(); // GameCenterAchievementLocalizationUpdateRequest | GameCenterAchievementLocalization representation

            try
            {
                GameCenterAchievementLocalizationResponse result = apiInstance.GameCenterAchievementLocalizationsUpdateInstance(id, gameCenterAchievementLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationResponse> response = apiInstance.GameCenterAchievementLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterAchievementLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementLocalizationUpdateRequest** | [**GameCenterAchievementLocalizationUpdateRequest**](GameCenterAchievementLocalizationUpdateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsv2createinstance"></a>
# **GameCenterAchievementLocalizationsV2CreateInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2CreateInstance (GameCenterAchievementLocalizationV2CreateRequest gameCenterAchievementLocalizationV2CreateRequest)



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
    public class GameCenterAchievementLocalizationsV2CreateInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterAchievementLocalizationV2CreateRequest = new GameCenterAchievementLocalizationV2CreateRequest(); // GameCenterAchievementLocalizationV2CreateRequest | GameCenterAchievementLocalization representation

            try
            {
                GameCenterAchievementLocalizationV2Response result = apiInstance.GameCenterAchievementLocalizationsV2CreateInstance(gameCenterAchievementLocalizationV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationV2Response> response = apiInstance.GameCenterAchievementLocalizationsV2CreateInstanceWithHttpInfo(gameCenterAchievementLocalizationV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementLocalizationV2CreateRequest** | [**GameCenterAchievementLocalizationV2CreateRequest**](GameCenterAchievementLocalizationV2CreateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **201** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsv2deleteinstance"></a>
# **GameCenterAchievementLocalizationsV2DeleteInstance**
> void GameCenterAchievementLocalizationsV2DeleteInstance (string id)



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
    public class GameCenterAchievementLocalizationsV2DeleteInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterAchievementLocalizationsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterAchievementLocalizationsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterachievementlocalizationsv2getinstance"></a>
# **GameCenterAchievementLocalizationsV2GetInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2GetInstance (string id, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? fieldsGameCenterAchievementImages = null, List<string>? include = null)



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
    public class GameCenterAchievementLocalizationsV2GetInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var fieldsGameCenterAchievementImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterAchievementLocalizationV2Response result = apiInstance.GameCenterAchievementLocalizationsV2GetInstance(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementImages, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationV2Response> response = apiInstance.GameCenterAchievementLocalizationsV2GetInstanceWithHttpInfo(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementImages, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsv2imagegettoonerelated"></a>
# **GameCenterAchievementLocalizationsV2ImageGetToOneRelated**
> GameCenterAchievementImageV2Response GameCenterAchievementLocalizationsV2ImageGetToOneRelated (string id, List<string>? fieldsGameCenterAchievementImages = null, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? include = null)



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
    public class GameCenterAchievementLocalizationsV2ImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementImages (optional) 
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterAchievementImageV2Response result = apiInstance.GameCenterAchievementLocalizationsV2ImageGetToOneRelated(id, fieldsGameCenterAchievementImages, fieldsGameCenterAchievementLocalizations, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2ImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2ImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementImageV2Response> response = apiInstance.GameCenterAchievementLocalizationsV2ImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterAchievementImages, fieldsGameCenterAchievementLocalizations, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2ImageGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementImageV2Response**](GameCenterAchievementImageV2Response.md)

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
| **200** | Single GameCenterAchievementImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementlocalizationsv2imagegettoonerelationship"></a>
# **GameCenterAchievementLocalizationsV2ImageGetToOneRelationship**
> GameCenterAchievementLocalizationV2ImageLinkageResponse GameCenterAchievementLocalizationsV2ImageGetToOneRelationship (string id)



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
    public class GameCenterAchievementLocalizationsV2ImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterAchievementLocalizationV2ImageLinkageResponse result = apiInstance.GameCenterAchievementLocalizationsV2ImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2ImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2ImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationV2ImageLinkageResponse> response = apiInstance.GameCenterAchievementLocalizationsV2ImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2ImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementLocalizationV2ImageLinkageResponse**](GameCenterAchievementLocalizationV2ImageLinkageResponse.md)

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

<a id="gamecenterachievementlocalizationsv2updateinstance"></a>
# **GameCenterAchievementLocalizationsV2UpdateInstance**
> GameCenterAchievementLocalizationV2Response GameCenterAchievementLocalizationsV2UpdateInstance (string id, GameCenterAchievementLocalizationV2UpdateRequest gameCenterAchievementLocalizationV2UpdateRequest)



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
    public class GameCenterAchievementLocalizationsV2UpdateInstanceExample
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
            var apiInstance = new GameCenterAchievementLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterAchievementLocalizationV2UpdateRequest = new GameCenterAchievementLocalizationV2UpdateRequest(); // GameCenterAchievementLocalizationV2UpdateRequest | GameCenterAchievementLocalization representation

            try
            {
                GameCenterAchievementLocalizationV2Response result = apiInstance.GameCenterAchievementLocalizationsV2UpdateInstance(id, gameCenterAchievementLocalizationV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementLocalizationsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationV2Response> response = apiInstance.GameCenterAchievementLocalizationsV2UpdateInstanceWithHttpInfo(id, gameCenterAchievementLocalizationV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementLocalizationsApi.GameCenterAchievementLocalizationsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementLocalizationV2UpdateRequest** | [**GameCenterAchievementLocalizationV2UpdateRequest**](GameCenterAchievementLocalizationV2UpdateRequest.md) | GameCenterAchievementLocalization representation |  |

### Return type

[**GameCenterAchievementLocalizationV2Response**](GameCenterAchievementLocalizationV2Response.md)

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
| **200** | Single GameCenterAchievementLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

