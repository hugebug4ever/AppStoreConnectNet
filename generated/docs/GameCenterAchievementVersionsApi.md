# AppStoreConnect.Net.Api.GameCenterAchievementVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementVersionsV2CreateInstance**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2createinstance) | **POST** /v2/gameCenterAchievementVersions |  |
| [**GameCenterAchievementVersionsV2GetInstance**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2getinstance) | **GET** /v2/gameCenterAchievementVersions/{id} |  |
| [**GameCenterAchievementVersionsV2LocalizationsGetToManyRelated**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterAchievementVersions/{id}/localizations |  |
| [**GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship**](GameCenterAchievementVersionsApi.md#gamecenterachievementversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterAchievementVersions/{id}/relationships/localizations |  |

<a id="gamecenterachievementversionsv2createinstance"></a>
# **GameCenterAchievementVersionsV2CreateInstance**
> GameCenterAchievementVersionV2Response GameCenterAchievementVersionsV2CreateInstance (GameCenterAchievementVersionV2CreateRequest gameCenterAchievementVersionV2CreateRequest)



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
    public class GameCenterAchievementVersionsV2CreateInstanceExample
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
            var apiInstance = new GameCenterAchievementVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterAchievementVersionV2CreateRequest = new GameCenterAchievementVersionV2CreateRequest(); // GameCenterAchievementVersionV2CreateRequest | GameCenterAchievementVersion representation

            try
            {
                GameCenterAchievementVersionV2Response result = apiInstance.GameCenterAchievementVersionsV2CreateInstance(gameCenterAchievementVersionV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementVersionsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementVersionV2Response> response = apiInstance.GameCenterAchievementVersionsV2CreateInstanceWithHttpInfo(gameCenterAchievementVersionV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementVersionV2CreateRequest** | [**GameCenterAchievementVersionV2CreateRequest**](GameCenterAchievementVersionV2CreateRequest.md) | GameCenterAchievementVersion representation |  |

### Return type

[**GameCenterAchievementVersionV2Response**](GameCenterAchievementVersionV2Response.md)

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
| **201** | Single GameCenterAchievementVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementversionsv2getinstance"></a>
# **GameCenterAchievementVersionsV2GetInstance**
> GameCenterAchievementVersionV2Response GameCenterAchievementVersionsV2GetInstance (string id, List<string>? fieldsGameCenterAchievementVersions = null, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class GameCenterAchievementVersionsV2GetInstanceExample
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
            var apiInstance = new GameCenterAchievementVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementVersions (optional) 
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                GameCenterAchievementVersionV2Response result = apiInstance.GameCenterAchievementVersionsV2GetInstance(id, fieldsGameCenterAchievementVersions, fieldsGameCenterAchievementLocalizations, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementVersionsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementVersionV2Response> response = apiInstance.GameCenterAchievementVersionsV2GetInstanceWithHttpInfo(id, fieldsGameCenterAchievementVersions, fieldsGameCenterAchievementLocalizations, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementVersionV2Response**](GameCenterAchievementVersionV2Response.md)

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
| **200** | Single GameCenterAchievementVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementversionsv2localizationsgettomanyrelated"></a>
# **GameCenterAchievementVersionsV2LocalizationsGetToManyRelated**
> GameCenterAchievementLocalizationsV2Response GameCenterAchievementVersionsV2LocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? fieldsGameCenterAchievementVersions = null, List<string>? fieldsGameCenterAchievementImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterAchievementVersionsV2LocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterAchievementVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var fieldsGameCenterAchievementVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementVersions (optional) 
            var fieldsGameCenterAchievementImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterAchievementLocalizationsV2Response result = apiInstance.GameCenterAchievementVersionsV2LocalizationsGetToManyRelated(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementVersions, fieldsGameCenterAchievementImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2LocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementVersionsV2LocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementLocalizationsV2Response> response = apiInstance.GameCenterAchievementVersionsV2LocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementVersions, fieldsGameCenterAchievementImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2LocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationsV2Response**](GameCenterAchievementLocalizationsV2Response.md)

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
| **200** | List of GameCenterAchievementLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterachievementversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship**
> GameCenterAchievementVersionV2LocalizationsLinkagesResponse GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterAchievementVersionsV2LocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterAchievementVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterAchievementVersionV2LocalizationsLinkagesResponse result = apiInstance.GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2LocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAchievementVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementVersionV2LocalizationsLinkagesResponse> response = apiInstance.GameCenterAchievementVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAchievementVersionsApi.GameCenterAchievementVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**GameCenterAchievementVersionV2LocalizationsLinkagesResponse**](GameCenterAchievementVersionV2LocalizationsLinkagesResponse.md)

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

