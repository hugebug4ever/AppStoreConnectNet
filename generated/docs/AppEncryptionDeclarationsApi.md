# AppStoreConnect.Net.Api.AppEncryptionDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelated) | **GET** /v1/appEncryptionDeclarations/{id}/appEncryptionDeclarationDocument |  |
| [**AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/appEncryptionDeclarationDocument |  |
| [**AppEncryptionDeclarationsAppGetToOneRelated**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappgettoonerelated) | **GET** /v1/appEncryptionDeclarations/{id}/app |  |
| [**AppEncryptionDeclarationsAppGetToOneRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappgettoonerelationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/app |  |
| [**AppEncryptionDeclarationsBuildsCreateToManyRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsbuildscreatetomanyrelationship) | **POST** /v1/appEncryptionDeclarations/{id}/relationships/builds |  |
| [**AppEncryptionDeclarationsCreateInstance**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationscreateinstance) | **POST** /v1/appEncryptionDeclarations |  |
| [**AppEncryptionDeclarationsGetCollection**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsgetcollection) | **GET** /v1/appEncryptionDeclarations |  |
| [**AppEncryptionDeclarationsGetInstance**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsgetinstance) | **GET** /v1/appEncryptionDeclarations/{id} |  |

<a id="appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelated"></a>
# **AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated**
> AppEncryptionDeclarationDocumentResponse AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated (string id, List<string>? fieldsAppEncryptionDeclarationDocuments = null)



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
    public class AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelatedExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppEncryptionDeclarationDocuments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional) 

            try
            {
                AppEncryptionDeclarationDocumentResponse result = apiInstance.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated(id, fieldsAppEncryptionDeclarationDocuments);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationDocumentResponse> response = apiInstance.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelatedWithHttpInfo(id, fieldsAppEncryptionDeclarationDocuments);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |

### Return type

[**AppEncryptionDeclarationDocumentResponse**](AppEncryptionDeclarationDocumentResponse.md)

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
| **200** | Single AppEncryptionDeclarationDocument |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelationship"></a>
# **AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship**
> AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship (string id)



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
    public class AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationshipExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse result = apiInstance.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse> response = apiInstance.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse**](AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse.md)

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

<a id="appencryptiondeclarationsappgettoonerelated"></a>
# **AppEncryptionDeclarationsAppGetToOneRelated**
> AppWithoutIncludesResponse AppEncryptionDeclarationsAppGetToOneRelated (string id, List<string>? fieldsApps = null)



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
    public class AppEncryptionDeclarationsAppGetToOneRelatedExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 

            try
            {
                AppWithoutIncludesResponse result = apiInstance.AppEncryptionDeclarationsAppGetToOneRelated(id, fieldsApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppWithoutIncludesResponse> response = apiInstance.AppEncryptionDeclarationsAppGetToOneRelatedWithHttpInfo(id, fieldsApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appencryptiondeclarationsappgettoonerelationship"></a>
# **AppEncryptionDeclarationsAppGetToOneRelationship**
> AppEncryptionDeclarationAppLinkageResponse AppEncryptionDeclarationsAppGetToOneRelationship (string id)



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
    public class AppEncryptionDeclarationsAppGetToOneRelationshipExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppEncryptionDeclarationAppLinkageResponse result = apiInstance.AppEncryptionDeclarationsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationAppLinkageResponse> response = apiInstance.AppEncryptionDeclarationsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppEncryptionDeclarationAppLinkageResponse**](AppEncryptionDeclarationAppLinkageResponse.md)

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

<a id="appencryptiondeclarationsbuildscreatetomanyrelationship"></a>
# **AppEncryptionDeclarationsBuildsCreateToManyRelationship**
> void AppEncryptionDeclarationsBuildsCreateToManyRelationship (string id, AppEncryptionDeclarationBuildsLinkagesRequest appEncryptionDeclarationBuildsLinkagesRequest)



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
    public class AppEncryptionDeclarationsBuildsCreateToManyRelationshipExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appEncryptionDeclarationBuildsLinkagesRequest = new AppEncryptionDeclarationBuildsLinkagesRequest(); // AppEncryptionDeclarationBuildsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.AppEncryptionDeclarationsBuildsCreateToManyRelationship(id, appEncryptionDeclarationBuildsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsBuildsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsBuildsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppEncryptionDeclarationsBuildsCreateToManyRelationshipWithHttpInfo(id, appEncryptionDeclarationBuildsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsBuildsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEncryptionDeclarationBuildsLinkagesRequest** | [**AppEncryptionDeclarationBuildsLinkagesRequest**](AppEncryptionDeclarationBuildsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appencryptiondeclarationscreateinstance"></a>
# **AppEncryptionDeclarationsCreateInstance**
> AppEncryptionDeclarationResponse AppEncryptionDeclarationsCreateInstance (AppEncryptionDeclarationCreateRequest appEncryptionDeclarationCreateRequest)



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
    public class AppEncryptionDeclarationsCreateInstanceExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var appEncryptionDeclarationCreateRequest = new AppEncryptionDeclarationCreateRequest(); // AppEncryptionDeclarationCreateRequest | AppEncryptionDeclaration representation

            try
            {
                AppEncryptionDeclarationResponse result = apiInstance.AppEncryptionDeclarationsCreateInstance(appEncryptionDeclarationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationResponse> response = apiInstance.AppEncryptionDeclarationsCreateInstanceWithHttpInfo(appEncryptionDeclarationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEncryptionDeclarationCreateRequest** | [**AppEncryptionDeclarationCreateRequest**](AppEncryptionDeclarationCreateRequest.md) | AppEncryptionDeclaration representation |  |

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
| **201** | Single AppEncryptionDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appencryptiondeclarationsgetcollection"></a>
# **AppEncryptionDeclarationsGetCollection**
> AppEncryptionDeclarationsResponse AppEncryptionDeclarationsGetCollection (List<string>? filterPlatform = null, List<string>? filterApp = null, List<string>? filterBuilds = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsApps = null, List<string>? fieldsAppEncryptionDeclarationDocuments = null, int? limit = null, List<string>? include = null, int? limitBuilds = null)



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
    public class AppEncryptionDeclarationsGetCollectionExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var filterPlatform = new List<string>?(); // List<string>? | filter by attribute 'platform' (optional) 
            var filterApp = new List<string>?(); // List<string>? | filter by id(s) of related 'app' (optional) 
            var filterBuilds = new List<string>?(); // List<string>? | filter by id(s) of related 'builds' (optional) 
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsAppEncryptionDeclarationDocuments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                AppEncryptionDeclarationsResponse result = apiInstance.AppEncryptionDeclarationsGetCollection(filterPlatform, filterApp, filterBuilds, fieldsAppEncryptionDeclarations, fieldsApps, fieldsAppEncryptionDeclarationDocuments, limit, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationsResponse> response = apiInstance.AppEncryptionDeclarationsGetCollectionWithHttpInfo(filterPlatform, filterApp, filterBuilds, fieldsAppEncryptionDeclarations, fieldsApps, fieldsAppEncryptionDeclarationDocuments, limit, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterPlatform** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**AppEncryptionDeclarationsResponse**](AppEncryptionDeclarationsResponse.md)

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
| **200** | List of AppEncryptionDeclarations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appencryptiondeclarationsgetinstance"></a>
# **AppEncryptionDeclarationsGetInstance**
> AppEncryptionDeclarationResponse AppEncryptionDeclarationsGetInstance (string id, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsApps = null, List<string>? fieldsAppEncryptionDeclarationDocuments = null, List<string>? include = null, int? limitBuilds = null)



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
    public class AppEncryptionDeclarationsGetInstanceExample
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
            var apiInstance = new AppEncryptionDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsAppEncryptionDeclarationDocuments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                AppEncryptionDeclarationResponse result = apiInstance.AppEncryptionDeclarationsGetInstance(id, fieldsAppEncryptionDeclarations, fieldsApps, fieldsAppEncryptionDeclarationDocuments, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppEncryptionDeclarationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationResponse> response = apiInstance.AppEncryptionDeclarationsGetInstanceWithHttpInfo(id, fieldsAppEncryptionDeclarations, fieldsApps, fieldsAppEncryptionDeclarationDocuments, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppEncryptionDeclarationsApi.AppEncryptionDeclarationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
| **200** | Single AppEncryptionDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

