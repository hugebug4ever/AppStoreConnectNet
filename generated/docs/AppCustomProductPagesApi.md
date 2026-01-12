# AppStoreConnect.Net.Api.AppCustomProductPagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated**](AppCustomProductPagesApi.md#appcustomproductpagesappcustomproductpageversionsgettomanyrelated) | **GET** /v1/appCustomProductPages/{id}/appCustomProductPageVersions |  |
| [**AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship**](AppCustomProductPagesApi.md#appcustomproductpagesappcustomproductpageversionsgettomanyrelationship) | **GET** /v1/appCustomProductPages/{id}/relationships/appCustomProductPageVersions |  |
| [**AppCustomProductPagesCreateInstance**](AppCustomProductPagesApi.md#appcustomproductpagescreateinstance) | **POST** /v1/appCustomProductPages |  |
| [**AppCustomProductPagesDeleteInstance**](AppCustomProductPagesApi.md#appcustomproductpagesdeleteinstance) | **DELETE** /v1/appCustomProductPages/{id} |  |
| [**AppCustomProductPagesGetInstance**](AppCustomProductPagesApi.md#appcustomproductpagesgetinstance) | **GET** /v1/appCustomProductPages/{id} |  |
| [**AppCustomProductPagesUpdateInstance**](AppCustomProductPagesApi.md#appcustomproductpagesupdateinstance) | **PATCH** /v1/appCustomProductPages/{id} |  |

<a id="appcustomproductpagesappcustomproductpageversionsgettomanyrelated"></a>
# **AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated**
> AppCustomProductPageVersionsResponse AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated (string id, List<string>? filterState = null, List<string>? fieldsAppCustomProductPageVersions = null, List<string>? fieldsAppCustomProductPages = null, List<string>? fieldsAppCustomProductPageLocalizations = null, int? limit = null, List<string>? include = null, int? limitAppCustomProductPageLocalizations = null)



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
    public class AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelatedExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterState = new List<string>?(); // List<string>? | filter by attribute 'state' (optional) 
            var fieldsAppCustomProductPageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageVersions (optional) 
            var fieldsAppCustomProductPages = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPages (optional) 
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppCustomProductPageLocalizations = 56;  // int? | maximum number of related appCustomProductPageLocalizations returned (when they are included) (optional) 

            try
            {
                AppCustomProductPageVersionsResponse result = apiInstance.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated(id, filterState, fieldsAppCustomProductPageVersions, fieldsAppCustomProductPages, fieldsAppCustomProductPageLocalizations, limit, include, limitAppCustomProductPageLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageVersionsResponse> response = apiInstance.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelatedWithHttpInfo(id, filterState, fieldsAppCustomProductPageVersions, fieldsAppCustomProductPages, fieldsAppCustomProductPageLocalizations, limit, include, limitAppCustomProductPageLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageLocalizations** | **int?** | maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageVersionsResponse**](AppCustomProductPageVersionsResponse.md)

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
| **200** | List of AppCustomProductPageVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpagesappcustomproductpageversionsgettomanyrelationship"></a>
# **AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship**
> AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse result = apiInstance.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse> response = apiInstance.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse**](AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.md)

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

<a id="appcustomproductpagescreateinstance"></a>
# **AppCustomProductPagesCreateInstance**
> AppCustomProductPageResponse AppCustomProductPagesCreateInstance (AppCustomProductPageCreateRequest appCustomProductPageCreateRequest)



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
    public class AppCustomProductPagesCreateInstanceExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var appCustomProductPageCreateRequest = new AppCustomProductPageCreateRequest(); // AppCustomProductPageCreateRequest | AppCustomProductPage representation

            try
            {
                AppCustomProductPageResponse result = apiInstance.AppCustomProductPagesCreateInstance(appCustomProductPageCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageResponse> response = apiInstance.AppCustomProductPagesCreateInstanceWithHttpInfo(appCustomProductPageCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageCreateRequest** | [**AppCustomProductPageCreateRequest**](AppCustomProductPageCreateRequest.md) | AppCustomProductPage representation |  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **201** | Single AppCustomProductPage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpagesdeleteinstance"></a>
# **AppCustomProductPagesDeleteInstance**
> void AppCustomProductPagesDeleteInstance (string id)



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
    public class AppCustomProductPagesDeleteInstanceExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppCustomProductPagesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppCustomProductPagesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appcustomproductpagesgetinstance"></a>
# **AppCustomProductPagesGetInstance**
> AppCustomProductPageResponse AppCustomProductPagesGetInstance (string id, List<string>? fieldsAppCustomProductPages = null, List<string>? fieldsAppCustomProductPageVersions = null, List<string>? include = null, int? limitAppCustomProductPageVersions = null)



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
    public class AppCustomProductPagesGetInstanceExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCustomProductPages = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPages (optional) 
            var fieldsAppCustomProductPageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppCustomProductPageVersions = 56;  // int? | maximum number of related appCustomProductPageVersions returned (when they are included) (optional) 

            try
            {
                AppCustomProductPageResponse result = apiInstance.AppCustomProductPagesGetInstance(id, fieldsAppCustomProductPages, fieldsAppCustomProductPageVersions, include, limitAppCustomProductPageVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageResponse> response = apiInstance.AppCustomProductPagesGetInstanceWithHttpInfo(id, fieldsAppCustomProductPages, fieldsAppCustomProductPageVersions, include, limitAppCustomProductPageVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageVersions** | **int?** | maximum number of related appCustomProductPageVersions returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **200** | Single AppCustomProductPage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpagesupdateinstance"></a>
# **AppCustomProductPagesUpdateInstance**
> AppCustomProductPageResponse AppCustomProductPagesUpdateInstance (string id, AppCustomProductPageUpdateRequest appCustomProductPageUpdateRequest)



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
    public class AppCustomProductPagesUpdateInstanceExample
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
            var apiInstance = new AppCustomProductPagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appCustomProductPageUpdateRequest = new AppCustomProductPageUpdateRequest(); // AppCustomProductPageUpdateRequest | AppCustomProductPage representation

            try
            {
                AppCustomProductPageResponse result = apiInstance.AppCustomProductPagesUpdateInstance(id, appCustomProductPageUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPagesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageResponse> response = apiInstance.AppCustomProductPagesUpdateInstanceWithHttpInfo(id, appCustomProductPageUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPagesApi.AppCustomProductPagesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageUpdateRequest** | [**AppCustomProductPageUpdateRequest**](AppCustomProductPageUpdateRequest.md) | AppCustomProductPage representation |  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **200** | Single AppCustomProductPage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

