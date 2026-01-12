# AppStoreConnect.Net.Api.GameCenterLeaderboardSetVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetVersionsV2CreateInstance**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2createinstance) | **POST** /v2/gameCenterLeaderboardSetVersions |  |
| [**GameCenterLeaderboardSetVersionsV2GetInstance**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2getinstance) | **GET** /v2/gameCenterLeaderboardSetVersions/{id} |  |
| [**GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardSetVersions/{id}/localizations |  |
| [**GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship**](GameCenterLeaderboardSetVersionsApi.md#gamecenterleaderboardsetversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardSetVersions/{id}/relationships/localizations |  |

<a id="gamecenterleaderboardsetversionsv2createinstance"></a>
# **GameCenterLeaderboardSetVersionsV2CreateInstance**
> GameCenterLeaderboardSetVersionV2Response GameCenterLeaderboardSetVersionsV2CreateInstance (GameCenterLeaderboardSetVersionV2CreateRequest gameCenterLeaderboardSetVersionV2CreateRequest)



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
    public class GameCenterLeaderboardSetVersionsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetVersionV2CreateRequest = new GameCenterLeaderboardSetVersionV2CreateRequest(); // GameCenterLeaderboardSetVersionV2CreateRequest | GameCenterLeaderboardSetVersion representation

            try
            {
                GameCenterLeaderboardSetVersionV2Response result = apiInstance.GameCenterLeaderboardSetVersionsV2CreateInstance(gameCenterLeaderboardSetVersionV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetVersionsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetVersionV2Response> response = apiInstance.GameCenterLeaderboardSetVersionsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardSetVersionV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetVersionV2CreateRequest** | [**GameCenterLeaderboardSetVersionV2CreateRequest**](GameCenterLeaderboardSetVersionV2CreateRequest.md) | GameCenterLeaderboardSetVersion representation |  |

### Return type

[**GameCenterLeaderboardSetVersionV2Response**](GameCenterLeaderboardSetVersionV2Response.md)

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
| **201** | Single GameCenterLeaderboardSetVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetversionsv2getinstance"></a>
# **GameCenterLeaderboardSetVersionsV2GetInstance**
> GameCenterLeaderboardSetVersionV2Response GameCenterLeaderboardSetVersionsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardSetVersions = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class GameCenterLeaderboardSetVersionsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetVersions (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetVersionV2Response result = apiInstance.GameCenterLeaderboardSetVersionsV2GetInstance(id, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSetLocalizations, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetVersionsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetVersionV2Response> response = apiInstance.GameCenterLeaderboardSetVersionsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSetLocalizations, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetVersionV2Response**](GameCenterLeaderboardSetVersionV2Response.md)

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
| **200** | Single GameCenterLeaderboardSetVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetversionsv2localizationsgettomanyrelated"></a>
# **GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated**
> GameCenterLeaderboardSetLocalizationsV2Response GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboardSetVersions = null, List<string>? fieldsGameCenterLeaderboardSetImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboardSetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetVersions (optional) 
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetLocalizationsV2Response result = apiInstance.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSetImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationsV2Response> response = apiInstance.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSetImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationsV2Response**](GameCenterLeaderboardSetLocalizationsV2Response.md)

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
| **200** | List of GameCenterLeaderboardSetLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship**
> GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse result = apiInstance.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetVersionsApi.GameCenterLeaderboardSetVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse**](GameCenterLeaderboardSetVersionV2LocalizationsLinkagesResponse.md)

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
| **200** | List of related linkages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

