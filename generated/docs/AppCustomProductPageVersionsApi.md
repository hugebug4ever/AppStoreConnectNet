# AppStoreConnect.Net.Api.AppCustomProductPageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelated) | **GET** /v1/appCustomProductPageVersions/{id}/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelationship) | **GET** /v1/appCustomProductPageVersions/{id}/relationships/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageVersionsCreateInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionscreateinstance) | **POST** /v1/appCustomProductPageVersions |  |
| [**AppCustomProductPageVersionsGetInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsgetinstance) | **GET** /v1/appCustomProductPageVersions/{id} |  |
| [**AppCustomProductPageVersionsUpdateInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsupdateinstance) | **PATCH** /v1/appCustomProductPageVersions/{id} |  |

<a id="appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelated"></a>
# **AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated**
> AppCustomProductPageLocalizationsResponse AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated (string id, List<string>? filterLocale = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppCustomProductPageVersions = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppPreviewSets = null, List<string>? fieldsAppKeywords = null, int? limit = null, List<string>? include = null, int? limitAppScreenshotSets = null, int? limitAppPreviewSets = null, int? limitSearchKeywords = null)



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
    public class AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelatedExample
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
            var apiInstance = new AppCustomProductPageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterLocale = new List<string>?(); // List<string>? | filter by attribute 'locale' (optional) 
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var fieldsAppCustomProductPageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageVersions (optional) 
            var fieldsAppScreenshotSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshotSets (optional) 
            var fieldsAppPreviewSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviewSets (optional) 
            var fieldsAppKeywords = new List<string>?(); // List<string>? | the fields to include for returned resources of type appKeywords (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppScreenshotSets = 56;  // int? | maximum number of related appScreenshotSets returned (when they are included) (optional) 
            var limitAppPreviewSets = 56;  // int? | maximum number of related appPreviewSets returned (when they are included) (optional) 
            var limitSearchKeywords = 56;  // int? | maximum number of related searchKeywords returned (when they are included) (optional) 

            try
            {
                AppCustomProductPageLocalizationsResponse result = apiInstance.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated(id, filterLocale, fieldsAppCustomProductPageLocalizations, fieldsAppCustomProductPageVersions, fieldsAppScreenshotSets, fieldsAppPreviewSets, fieldsAppKeywords, limit, include, limitAppScreenshotSets, limitAppPreviewSets, limitSearchKeywords);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationsResponse> response = apiInstance.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelatedWithHttpInfo(id, filterLocale, fieldsAppCustomProductPageLocalizations, fieldsAppCustomProductPageVersions, fieldsAppScreenshotSets, fieldsAppPreviewSets, fieldsAppKeywords, limit, include, limitAppScreenshotSets, limitAppPreviewSets, limitSearchKeywords);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLocale** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **fieldsAppKeywords** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appKeywords | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppScreenshotSets** | **int?** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitAppPreviewSets** | **int?** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int?** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageLocalizationsResponse**](AppCustomProductPageLocalizationsResponse.md)

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
| **200** | List of AppCustomProductPageLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelationship"></a>
# **AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship**
> AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse result = apiInstance.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse> response = apiInstance.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse**](AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.md)

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

<a id="appcustomproductpageversionscreateinstance"></a>
# **AppCustomProductPageVersionsCreateInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsCreateInstance (AppCustomProductPageVersionCreateRequest appCustomProductPageVersionCreateRequest)



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
    public class AppCustomProductPageVersionsCreateInstanceExample
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
            var apiInstance = new AppCustomProductPageVersionsApi(httpClient, config, httpClientHandler);
            var appCustomProductPageVersionCreateRequest = new AppCustomProductPageVersionCreateRequest(); // AppCustomProductPageVersionCreateRequest | AppCustomProductPageVersion representation

            try
            {
                AppCustomProductPageVersionResponse result = apiInstance.AppCustomProductPageVersionsCreateInstance(appCustomProductPageVersionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageVersionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageVersionResponse> response = apiInstance.AppCustomProductPageVersionsCreateInstanceWithHttpInfo(appCustomProductPageVersionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageVersionCreateRequest** | [**AppCustomProductPageVersionCreateRequest**](AppCustomProductPageVersionCreateRequest.md) | AppCustomProductPageVersion representation |  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **201** | Single AppCustomProductPageVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpageversionsgetinstance"></a>
# **AppCustomProductPageVersionsGetInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsGetInstance (string id, List<string>? fieldsAppCustomProductPageVersions = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? include = null, int? limitAppCustomProductPageLocalizations = null)



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
    public class AppCustomProductPageVersionsGetInstanceExample
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
            var apiInstance = new AppCustomProductPageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCustomProductPageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageVersions (optional) 
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppCustomProductPageLocalizations = 56;  // int? | maximum number of related appCustomProductPageLocalizations returned (when they are included) (optional) 

            try
            {
                AppCustomProductPageVersionResponse result = apiInstance.AppCustomProductPageVersionsGetInstance(id, fieldsAppCustomProductPageVersions, fieldsAppCustomProductPageLocalizations, include, limitAppCustomProductPageLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageVersionResponse> response = apiInstance.AppCustomProductPageVersionsGetInstanceWithHttpInfo(id, fieldsAppCustomProductPageVersions, fieldsAppCustomProductPageLocalizations, include, limitAppCustomProductPageLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageLocalizations** | **int?** | maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **200** | Single AppCustomProductPageVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpageversionsupdateinstance"></a>
# **AppCustomProductPageVersionsUpdateInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsUpdateInstance (string id, AppCustomProductPageVersionUpdateRequest appCustomProductPageVersionUpdateRequest)



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
    public class AppCustomProductPageVersionsUpdateInstanceExample
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
            var apiInstance = new AppCustomProductPageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appCustomProductPageVersionUpdateRequest = new AppCustomProductPageVersionUpdateRequest(); // AppCustomProductPageVersionUpdateRequest | AppCustomProductPageVersion representation

            try
            {
                AppCustomProductPageVersionResponse result = apiInstance.AppCustomProductPageVersionsUpdateInstance(id, appCustomProductPageVersionUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageVersionsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageVersionResponse> response = apiInstance.AppCustomProductPageVersionsUpdateInstanceWithHttpInfo(id, appCustomProductPageVersionUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageVersionsApi.AppCustomProductPageVersionsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageVersionUpdateRequest** | [**AppCustomProductPageVersionUpdateRequest**](AppCustomProductPageVersionUpdateRequest.md) | AppCustomProductPageVersion representation |  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **200** | Single AppCustomProductPageVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

