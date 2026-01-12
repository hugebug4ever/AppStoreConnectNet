# AppStoreConnect.Net.Api.AnalyticsReportsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportsGetInstance**](AnalyticsReportsApi.md#analyticsreportsgetinstance) | **GET** /v1/analyticsReports/{id} |  |
| [**AnalyticsReportsInstancesGetToManyRelated**](AnalyticsReportsApi.md#analyticsreportsinstancesgettomanyrelated) | **GET** /v1/analyticsReports/{id}/instances |  |
| [**AnalyticsReportsInstancesGetToManyRelationship**](AnalyticsReportsApi.md#analyticsreportsinstancesgettomanyrelationship) | **GET** /v1/analyticsReports/{id}/relationships/instances |  |

<a id="analyticsreportsgetinstance"></a>
# **AnalyticsReportsGetInstance**
> AnalyticsReportResponse AnalyticsReportsGetInstance (string id, List<string>? fieldsAnalyticsReports = null)



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
    public class AnalyticsReportsGetInstanceExample
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
            var apiInstance = new AnalyticsReportsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAnalyticsReports = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReports (optional) 

            try
            {
                AnalyticsReportResponse result = apiInstance.AnalyticsReportsGetInstance(id, fieldsAnalyticsReports);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportResponse> response = apiInstance.AnalyticsReportsGetInstanceWithHttpInfo(id, fieldsAnalyticsReports);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |

### Return type

[**AnalyticsReportResponse**](AnalyticsReportResponse.md)

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
| **200** | Single AnalyticsReport |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportsinstancesgettomanyrelated"></a>
# **AnalyticsReportsInstancesGetToManyRelated**
> AnalyticsReportInstancesResponse AnalyticsReportsInstancesGetToManyRelated (string id, List<string>? filterGranularity = null, List<string>? filterProcessingDate = null, List<string>? fieldsAnalyticsReportInstances = null, int? limit = null)



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
    public class AnalyticsReportsInstancesGetToManyRelatedExample
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
            var apiInstance = new AnalyticsReportsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterGranularity = new List<string>?(); // List<string>? | filter by attribute 'granularity' (optional) 
            var filterProcessingDate = new List<string>?(); // List<string>? | filter by attribute 'processingDate' (optional) 
            var fieldsAnalyticsReportInstances = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReportInstances (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportInstancesResponse result = apiInstance.AnalyticsReportsInstancesGetToManyRelated(id, filterGranularity, filterProcessingDate, fieldsAnalyticsReportInstances, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsInstancesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportsInstancesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportInstancesResponse> response = apiInstance.AnalyticsReportsInstancesGetToManyRelatedWithHttpInfo(id, filterGranularity, filterProcessingDate, fieldsAnalyticsReportInstances, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsInstancesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterGranularity** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;granularity&#39; | [optional]  |
| **filterProcessingDate** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;processingDate&#39; | [optional]  |
| **fieldsAnalyticsReportInstances** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReportInstances | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportInstancesResponse**](AnalyticsReportInstancesResponse.md)

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
| **200** | List of AnalyticsReportInstances |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportsinstancesgettomanyrelationship"></a>
# **AnalyticsReportsInstancesGetToManyRelationship**
> AnalyticsReportInstancesLinkagesResponse AnalyticsReportsInstancesGetToManyRelationship (string id, int? limit = null)



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
    public class AnalyticsReportsInstancesGetToManyRelationshipExample
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
            var apiInstance = new AnalyticsReportsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportInstancesLinkagesResponse result = apiInstance.AnalyticsReportsInstancesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsInstancesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportsInstancesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportInstancesLinkagesResponse> response = apiInstance.AnalyticsReportsInstancesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportsApi.AnalyticsReportsInstancesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AnalyticsReportInstancesLinkagesResponse**](AnalyticsReportInstancesLinkagesResponse.md)

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

