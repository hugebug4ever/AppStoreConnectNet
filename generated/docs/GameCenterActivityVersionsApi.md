# AppStoreConnect.Net.Api.GameCenterActivityVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivityVersionsCreateInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionscreateinstance) | **POST** /v1/gameCenterActivityVersions |  |
| [**GameCenterActivityVersionsDefaultImageGetToOneRelated**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsdefaultimagegettoonerelated) | **GET** /v1/gameCenterActivityVersions/{id}/defaultImage |  |
| [**GameCenterActivityVersionsDefaultImageGetToOneRelationship**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsdefaultimagegettoonerelationship) | **GET** /v1/gameCenterActivityVersions/{id}/relationships/defaultImage |  |
| [**GameCenterActivityVersionsGetInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsgetinstance) | **GET** /v1/gameCenterActivityVersions/{id} |  |
| [**GameCenterActivityVersionsLocalizationsGetToManyRelated**](GameCenterActivityVersionsApi.md#gamecenteractivityversionslocalizationsgettomanyrelated) | **GET** /v1/gameCenterActivityVersions/{id}/localizations |  |
| [**GameCenterActivityVersionsLocalizationsGetToManyRelationship**](GameCenterActivityVersionsApi.md#gamecenteractivityversionslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterActivityVersions/{id}/relationships/localizations |  |
| [**GameCenterActivityVersionsUpdateInstance**](GameCenterActivityVersionsApi.md#gamecenteractivityversionsupdateinstance) | **PATCH** /v1/gameCenterActivityVersions/{id} |  |

<a id="gamecenteractivityversionscreateinstance"></a>
# **GameCenterActivityVersionsCreateInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsCreateInstance (GameCenterActivityVersionCreateRequest gameCenterActivityVersionCreateRequest)



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
    public class GameCenterActivityVersionsCreateInstanceExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterActivityVersionCreateRequest = new GameCenterActivityVersionCreateRequest(); // GameCenterActivityVersionCreateRequest | GameCenterActivityVersion representation

            try
            {
                GameCenterActivityVersionResponse result = apiInstance.GameCenterActivityVersionsCreateInstance(gameCenterActivityVersionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionResponse> response = apiInstance.GameCenterActivityVersionsCreateInstanceWithHttpInfo(gameCenterActivityVersionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityVersionCreateRequest** | [**GameCenterActivityVersionCreateRequest**](GameCenterActivityVersionCreateRequest.md) | GameCenterActivityVersion representation |  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **201** | Single GameCenterActivityVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivityversionsdefaultimagegettoonerelated"></a>
# **GameCenterActivityVersionsDefaultImageGetToOneRelated**
> GameCenterActivityImageResponse GameCenterActivityVersionsDefaultImageGetToOneRelated (string id, List<string>? fieldsGameCenterActivityImages = null)



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
    public class GameCenterActivityVersionsDefaultImageGetToOneRelatedExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityImages (optional) 

            try
            {
                GameCenterActivityImageResponse result = apiInstance.GameCenterActivityVersionsDefaultImageGetToOneRelated(id, fieldsGameCenterActivityImages);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsDefaultImageGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsDefaultImageGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityImageResponse> response = apiInstance.GameCenterActivityVersionsDefaultImageGetToOneRelatedWithHttpInfo(id, fieldsGameCenterActivityImages);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsDefaultImageGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenteractivityversionsdefaultimagegettoonerelationship"></a>
# **GameCenterActivityVersionsDefaultImageGetToOneRelationship**
> GameCenterActivityVersionDefaultImageLinkageResponse GameCenterActivityVersionsDefaultImageGetToOneRelationship (string id)



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
    public class GameCenterActivityVersionsDefaultImageGetToOneRelationshipExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterActivityVersionDefaultImageLinkageResponse result = apiInstance.GameCenterActivityVersionsDefaultImageGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsDefaultImageGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsDefaultImageGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionDefaultImageLinkageResponse> response = apiInstance.GameCenterActivityVersionsDefaultImageGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsDefaultImageGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterActivityVersionDefaultImageLinkageResponse**](GameCenterActivityVersionDefaultImageLinkageResponse.md)

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

<a id="gamecenteractivityversionsgetinstance"></a>
# **GameCenterActivityVersionsGetInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsGetInstance (string id, List<string>? fieldsGameCenterActivityVersions = null, List<string>? fieldsGameCenterActivityLocalizations = null, List<string>? fieldsGameCenterActivityImages = null, List<string>? include = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterActivityVersionsGetInstanceExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityVersions (optional) 
            var fieldsGameCenterActivityLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityLocalizations (optional) 
            var fieldsGameCenterActivityImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterActivityVersionResponse result = apiInstance.GameCenterActivityVersionsGetInstance(id, fieldsGameCenterActivityVersions, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityImages, include, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionResponse> response = apiInstance.GameCenterActivityVersionsGetInstanceWithHttpInfo(id, fieldsGameCenterActivityVersions, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityImages, include, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **200** | Single GameCenterActivityVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivityversionslocalizationsgettomanyrelated"></a>
# **GameCenterActivityVersionsLocalizationsGetToManyRelated**
> GameCenterActivityLocalizationsResponse GameCenterActivityVersionsLocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterActivityLocalizations = null, List<string>? fieldsGameCenterActivityVersions = null, List<string>? fieldsGameCenterActivityImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterActivityVersionsLocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivityLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityLocalizations (optional) 
            var fieldsGameCenterActivityVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityVersions (optional) 
            var fieldsGameCenterActivityImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterActivityLocalizationsResponse result = apiInstance.GameCenterActivityVersionsLocalizationsGetToManyRelated(id, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityVersions, fieldsGameCenterActivityImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityLocalizationsResponse> response = apiInstance.GameCenterActivityVersionsLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterActivityLocalizations, fieldsGameCenterActivityVersions, fieldsGameCenterActivityImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterActivityLocalizationsResponse**](GameCenterActivityLocalizationsResponse.md)

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
| **200** | List of GameCenterActivityLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenteractivityversionslocalizationsgettomanyrelationship"></a>
# **GameCenterActivityVersionsLocalizationsGetToManyRelationship**
> GameCenterActivityVersionLocalizationsLinkagesResponse GameCenterActivityVersionsLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterActivityVersionsLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterActivityVersionLocalizationsLinkagesResponse result = apiInstance.GameCenterActivityVersionsLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionLocalizationsLinkagesResponse> response = apiInstance.GameCenterActivityVersionsLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**GameCenterActivityVersionLocalizationsLinkagesResponse**](GameCenterActivityVersionLocalizationsLinkagesResponse.md)

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

<a id="gamecenteractivityversionsupdateinstance"></a>
# **GameCenterActivityVersionsUpdateInstance**
> GameCenterActivityVersionResponse GameCenterActivityVersionsUpdateInstance (string id, GameCenterActivityVersionUpdateRequest gameCenterActivityVersionUpdateRequest)



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
    public class GameCenterActivityVersionsUpdateInstanceExample
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
            var apiInstance = new GameCenterActivityVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterActivityVersionUpdateRequest = new GameCenterActivityVersionUpdateRequest(); // GameCenterActivityVersionUpdateRequest | GameCenterActivityVersion representation

            try
            {
                GameCenterActivityVersionResponse result = apiInstance.GameCenterActivityVersionsUpdateInstance(id, gameCenterActivityVersionUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterActivityVersionsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivityVersionResponse> response = apiInstance.GameCenterActivityVersionsUpdateInstanceWithHttpInfo(id, gameCenterActivityVersionUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterActivityVersionsApi.GameCenterActivityVersionsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityVersionUpdateRequest** | [**GameCenterActivityVersionUpdateRequest**](GameCenterActivityVersionUpdateRequest.md) | GameCenterActivityVersion representation |  |

### Return type

[**GameCenterActivityVersionResponse**](GameCenterActivityVersionResponse.md)

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
| **200** | Single GameCenterActivityVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

