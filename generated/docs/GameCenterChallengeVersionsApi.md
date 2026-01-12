# AppStoreConnect.Net.Api.GameCenterChallengeVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengeVersionsCreateInstance**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionscreateinstance) | **POST** /v1/gameCenterChallengeVersions |  |
| [**GameCenterChallengeVersionsDefaultImageGetToOneRelated**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsdefaultimagegettoonerelated) | **GET** /v1/gameCenterChallengeVersions/{id}/defaultImage |  |
| [**GameCenterChallengeVersionsDefaultImageGetToOneRelationship**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsdefaultimagegettoonerelationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/defaultImage |  |
| [**GameCenterChallengeVersionsGetInstance**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionsgetinstance) | **GET** /v1/gameCenterChallengeVersions/{id} |  |
| [**GameCenterChallengeVersionsLocalizationsGetToManyRelated**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionslocalizationsgettomanyrelated) | **GET** /v1/gameCenterChallengeVersions/{id}/localizations |  |
| [**GameCenterChallengeVersionsLocalizationsGetToManyRelationship**](GameCenterChallengeVersionsApi.md#gamecenterchallengeversionslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/localizations |  |

<a id="gamecenterchallengeversionscreateinstance"></a>
# **GameCenterChallengeVersionsCreateInstance**
> GameCenterChallengeVersionResponse GameCenterChallengeVersionsCreateInstance (GameCenterChallengeVersionCreateRequest gameCenterChallengeVersionCreateRequest)



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
    public class GameCenterChallengeVersionsCreateInstanceExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterChallengeVersionCreateRequest = new GameCenterChallengeVersionCreateRequest(); // GameCenterChallengeVersionCreateRequest | GameCenterChallengeVersion representation

            try
            {
                GameCenterChallengeVersionResponse result = apiInstance.GameCenterChallengeVersionsCreateInstance(gameCenterChallengeVersionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionResponse> response = apiInstance.GameCenterChallengeVersionsCreateInstanceWithHttpInfo(gameCenterChallengeVersionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeVersionCreateRequest** | [**GameCenterChallengeVersionCreateRequest**](GameCenterChallengeVersionCreateRequest.md) | GameCenterChallengeVersion representation |  |

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
| **201** | Single GameCenterChallengeVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengeversionsdefaultimagegettoonerelated"></a>
# **GameCenterChallengeVersionsDefaultImageGetToOneRelated**
> GameCenterChallengeImageResponse GameCenterChallengeVersionsDefaultImageGetToOneRelated (string id, List<string>? fieldsGameCenterChallengeImages = null)



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
    public class GameCenterChallengeVersionsDefaultImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 

            try
            {
                GameCenterChallengeImageResponse result = apiInstance.GameCenterChallengeVersionsDefaultImageGetToOneRelated(id, fieldsGameCenterChallengeImages);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsDefaultImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsDefaultImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeImageResponse> response = apiInstance.GameCenterChallengeVersionsDefaultImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterChallengeImages);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsDefaultImageGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenterchallengeversionsdefaultimagegettoonerelationship"></a>
# **GameCenterChallengeVersionsDefaultImageGetToOneRelationship**
> GameCenterChallengeVersionDefaultImageLinkageResponse GameCenterChallengeVersionsDefaultImageGetToOneRelationship (string id)



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
    public class GameCenterChallengeVersionsDefaultImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterChallengeVersionDefaultImageLinkageResponse result = apiInstance.GameCenterChallengeVersionsDefaultImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsDefaultImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsDefaultImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionDefaultImageLinkageResponse> response = apiInstance.GameCenterChallengeVersionsDefaultImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsDefaultImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterChallengeVersionDefaultImageLinkageResponse**](GameCenterChallengeVersionDefaultImageLinkageResponse.md)

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

<a id="gamecenterchallengeversionsgetinstance"></a>
# **GameCenterChallengeVersionsGetInstance**
> GameCenterChallengeVersionResponse GameCenterChallengeVersionsGetInstance (string id, List<string>? fieldsGameCenterChallengeVersions = null, List<string>? fieldsGameCenterChallengeLocalizations = null, List<string>? fieldsGameCenterChallengeImages = null, List<string>? include = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterChallengeVersionsGetInstanceExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersions (optional) 
            var fieldsGameCenterChallengeLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional) 
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterChallengeVersionResponse result = apiInstance.GameCenterChallengeVersionsGetInstance(id, fieldsGameCenterChallengeVersions, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeImages, include, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionResponse> response = apiInstance.GameCenterChallengeVersionsGetInstanceWithHttpInfo(id, fieldsGameCenterChallengeVersions, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeImages, include, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
| **200** | Single GameCenterChallengeVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengeversionslocalizationsgettomanyrelated"></a>
# **GameCenterChallengeVersionsLocalizationsGetToManyRelated**
> GameCenterChallengeLocalizationsResponse GameCenterChallengeVersionsLocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterChallengeLocalizations = null, List<string>? fieldsGameCenterChallengeVersions = null, List<string>? fieldsGameCenterChallengeImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterChallengeVersionsLocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional) 
            var fieldsGameCenterChallengeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersions (optional) 
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterChallengeLocalizationsResponse result = apiInstance.GameCenterChallengeVersionsLocalizationsGetToManyRelated(id, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeVersions, fieldsGameCenterChallengeImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeLocalizationsResponse> response = apiInstance.GameCenterChallengeVersionsLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeVersions, fieldsGameCenterChallengeImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterChallengeLocalizationsResponse**](GameCenterChallengeLocalizationsResponse.md)

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
| **200** | List of GameCenterChallengeLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengeversionslocalizationsgettomanyrelationship"></a>
# **GameCenterChallengeVersionsLocalizationsGetToManyRelationship**
> GameCenterChallengeVersionLocalizationsLinkagesResponse GameCenterChallengeVersionsLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterChallengeVersionsLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterChallengeVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterChallengeVersionLocalizationsLinkagesResponse result = apiInstance.GameCenterChallengeVersionsLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengeVersionsLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionLocalizationsLinkagesResponse> response = apiInstance.GameCenterChallengeVersionsLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengeVersionsApi.GameCenterChallengeVersionsLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**GameCenterChallengeVersionLocalizationsLinkagesResponse**](GameCenterChallengeVersionLocalizationsLinkagesResponse.md)

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

