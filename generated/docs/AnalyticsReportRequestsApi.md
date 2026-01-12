# AppStoreConnect.Net.Api.AnalyticsReportRequestsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportRequestsCreateInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestscreateinstance) | **POST** /v1/analyticsReportRequests |  |
| [**AnalyticsReportRequestsDeleteInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestsdeleteinstance) | **DELETE** /v1/analyticsReportRequests/{id} |  |
| [**AnalyticsReportRequestsGetInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestsgetinstance) | **GET** /v1/analyticsReportRequests/{id} |  |
| [**AnalyticsReportRequestsReportsGetToManyRelated**](AnalyticsReportRequestsApi.md#analyticsreportrequestsreportsgettomanyrelated) | **GET** /v1/analyticsReportRequests/{id}/reports |  |
| [**AnalyticsReportRequestsReportsGetToManyRelationship**](AnalyticsReportRequestsApi.md#analyticsreportrequestsreportsgettomanyrelationship) | **GET** /v1/analyticsReportRequests/{id}/relationships/reports |  |

<a id="analyticsreportrequestscreateinstance"></a>
# **AnalyticsReportRequestsCreateInstance**
> AnalyticsReportRequestResponse AnalyticsReportRequestsCreateInstance (AnalyticsReportRequestCreateRequest analyticsReportRequestCreateRequest)



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
    public class AnalyticsReportRequestsCreateInstanceExample
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
            var apiInstance = new AnalyticsReportRequestsApi(httpClient, config, httpClientHandler);
            var analyticsReportRequestCreateRequest = new AnalyticsReportRequestCreateRequest(); // AnalyticsReportRequestCreateRequest | AnalyticsReportRequest representation

            try
            {
                AnalyticsReportRequestResponse result = apiInstance.AnalyticsReportRequestsCreateInstance(analyticsReportRequestCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportRequestsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportRequestResponse> response = apiInstance.AnalyticsReportRequestsCreateInstanceWithHttpInfo(analyticsReportRequestCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **analyticsReportRequestCreateRequest** | [**AnalyticsReportRequestCreateRequest**](AnalyticsReportRequestCreateRequest.md) | AnalyticsReportRequest representation |  |

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
| **201** | Single AnalyticsReportRequest |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportrequestsdeleteinstance"></a>
# **AnalyticsReportRequestsDeleteInstance**
> void AnalyticsReportRequestsDeleteInstance (string id)



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
    public class AnalyticsReportRequestsDeleteInstanceExample
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
            var apiInstance = new AnalyticsReportRequestsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AnalyticsReportRequestsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportRequestsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AnalyticsReportRequestsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="analyticsreportrequestsgetinstance"></a>
# **AnalyticsReportRequestsGetInstance**
> AnalyticsReportRequestResponse AnalyticsReportRequestsGetInstance (string id, List<string>? fieldsAnalyticsReportRequests = null, List<string>? fieldsAnalyticsReports = null, List<string>? include = null, int? limitReports = null)



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
    public class AnalyticsReportRequestsGetInstanceExample
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
            var apiInstance = new AnalyticsReportRequestsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAnalyticsReportRequests = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReportRequests (optional) 
            var fieldsAnalyticsReports = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReports (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitReports = 56;  // int? | maximum number of related reports returned (when they are included) (optional) 

            try
            {
                AnalyticsReportRequestResponse result = apiInstance.AnalyticsReportRequestsGetInstance(id, fieldsAnalyticsReportRequests, fieldsAnalyticsReports, include, limitReports);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportRequestsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportRequestResponse> response = apiInstance.AnalyticsReportRequestsGetInstanceWithHttpInfo(id, fieldsAnalyticsReportRequests, fieldsAnalyticsReports, include, limitReports);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportRequests** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReportRequests | [optional]  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitReports** | **int?** | maximum number of related reports returned (when they are included) | [optional]  |

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
| **200** | Single AnalyticsReportRequest |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportrequestsreportsgettomanyrelated"></a>
# **AnalyticsReportRequestsReportsGetToManyRelated**
> AnalyticsReportsResponse AnalyticsReportRequestsReportsGetToManyRelated (string id, List<string>? filterName = null, List<string>? filterCategory = null, List<string>? fieldsAnalyticsReports = null, int? limit = null)



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
    public class AnalyticsReportRequestsReportsGetToManyRelatedExample
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
            var apiInstance = new AnalyticsReportRequestsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterName = new List<string>?(); // List<string>? | filter by attribute 'name' (optional) 
            var filterCategory = new List<string>?(); // List<string>? | filter by attribute 'category' (optional) 
            var fieldsAnalyticsReports = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReports (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportsResponse result = apiInstance.AnalyticsReportRequestsReportsGetToManyRelated(id, filterName, filterCategory, fieldsAnalyticsReports, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsReportsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportRequestsReportsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportsResponse> response = apiInstance.AnalyticsReportRequestsReportsGetToManyRelatedWithHttpInfo(id, filterName, filterCategory, fieldsAnalyticsReports, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsReportsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterCategory** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;category&#39; | [optional]  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportsResponse**](AnalyticsReportsResponse.md)

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
| **200** | List of AnalyticsReports |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportrequestsreportsgettomanyrelationship"></a>
# **AnalyticsReportRequestsReportsGetToManyRelationship**
> AnalyticsReportRequestReportsLinkagesResponse AnalyticsReportRequestsReportsGetToManyRelationship (string id, int? limit = null)



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
    public class AnalyticsReportRequestsReportsGetToManyRelationshipExample
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
            var apiInstance = new AnalyticsReportRequestsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportRequestReportsLinkagesResponse result = apiInstance.AnalyticsReportRequestsReportsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsReportsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportRequestsReportsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportRequestReportsLinkagesResponse> response = apiInstance.AnalyticsReportRequestsReportsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportRequestsApi.AnalyticsReportRequestsReportsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AnalyticsReportRequestReportsLinkagesResponse**](AnalyticsReportRequestReportsLinkagesResponse.md)

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

