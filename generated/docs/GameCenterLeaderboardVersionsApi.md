# AppStoreConnect.Net.Api.GameCenterLeaderboardVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardVersionsV2CreateInstance**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2createinstance) | **POST** /v2/gameCenterLeaderboardVersions |  |
| [**GameCenterLeaderboardVersionsV2GetInstance**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2getinstance) | **GET** /v2/gameCenterLeaderboardVersions/{id} |  |
| [**GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2localizationsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardVersions/{id}/localizations |  |
| [**GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship**](GameCenterLeaderboardVersionsApi.md#gamecenterleaderboardversionsv2localizationsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardVersions/{id}/relationships/localizations |  |

<a id="gamecenterleaderboardversionsv2createinstance"></a>
# **GameCenterLeaderboardVersionsV2CreateInstance**
> GameCenterLeaderboardVersionV2Response GameCenterLeaderboardVersionsV2CreateInstance (GameCenterLeaderboardVersionV2CreateRequest gameCenterLeaderboardVersionV2CreateRequest)



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
    public class GameCenterLeaderboardVersionsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardVersionV2CreateRequest = new GameCenterLeaderboardVersionV2CreateRequest(); // GameCenterLeaderboardVersionV2CreateRequest | GameCenterLeaderboardVersion representation

            try
            {
                GameCenterLeaderboardVersionV2Response result = apiInstance.GameCenterLeaderboardVersionsV2CreateInstance(gameCenterLeaderboardVersionV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardVersionsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardVersionV2Response> response = apiInstance.GameCenterLeaderboardVersionsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardVersionV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardVersionV2CreateRequest** | [**GameCenterLeaderboardVersionV2CreateRequest**](GameCenterLeaderboardVersionV2CreateRequest.md) | GameCenterLeaderboardVersion representation |  |

### Return type

[**GameCenterLeaderboardVersionV2Response**](GameCenterLeaderboardVersionV2Response.md)

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
| **201** | Single GameCenterLeaderboardVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardversionsv2getinstance"></a>
# **GameCenterLeaderboardVersionsV2GetInstance**
> GameCenterLeaderboardVersionV2Response GameCenterLeaderboardVersionsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardVersions = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class GameCenterLeaderboardVersionsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardVersions (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardVersionV2Response result = apiInstance.GameCenterLeaderboardVersionsV2GetInstance(id, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboardLocalizations, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardVersionsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardVersionV2Response> response = apiInstance.GameCenterLeaderboardVersionsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboardLocalizations, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardVersionV2Response**](GameCenterLeaderboardVersionV2Response.md)

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
| **200** | Single GameCenterLeaderboardVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardversionsv2localizationsgettomanyrelated"></a>
# **GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated**
> GameCenterLeaderboardLocalizationsV2Response GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardVersions = null, List<string>? fieldsGameCenterLeaderboardImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardVersions (optional) 
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardLocalizationsV2Response result = apiInstance.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboardImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationsV2Response> response = apiInstance.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboardImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationsV2Response**](GameCenterLeaderboardLocalizationsV2Response.md)

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
| **200** | List of GameCenterLeaderboardLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardversionsv2localizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship**
> GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse result = apiInstance.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse> response = apiInstance.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardVersionsApi.GameCenterLeaderboardVersionsV2LocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse**](GameCenterLeaderboardVersionV2LocalizationsLinkagesResponse.md)

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

