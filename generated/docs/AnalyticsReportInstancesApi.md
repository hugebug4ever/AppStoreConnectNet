# AppStoreConnect.Net.Api.AnalyticsReportInstancesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportInstancesGetInstance**](AnalyticsReportInstancesApi.md#analyticsreportinstancesgetinstance) | **GET** /v1/analyticsReportInstances/{id} |  |
| [**AnalyticsReportInstancesSegmentsGetToManyRelated**](AnalyticsReportInstancesApi.md#analyticsreportinstancessegmentsgettomanyrelated) | **GET** /v1/analyticsReportInstances/{id}/segments |  |
| [**AnalyticsReportInstancesSegmentsGetToManyRelationship**](AnalyticsReportInstancesApi.md#analyticsreportinstancessegmentsgettomanyrelationship) | **GET** /v1/analyticsReportInstances/{id}/relationships/segments |  |

<a id="analyticsreportinstancesgetinstance"></a>
# **AnalyticsReportInstancesGetInstance**
> AnalyticsReportInstanceResponse AnalyticsReportInstancesGetInstance (string id, List<string>? fieldsAnalyticsReportInstances = null)



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
    public class AnalyticsReportInstancesGetInstanceExample
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
            var apiInstance = new AnalyticsReportInstancesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAnalyticsReportInstances = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReportInstances (optional) 

            try
            {
                AnalyticsReportInstanceResponse result = apiInstance.AnalyticsReportInstancesGetInstance(id, fieldsAnalyticsReportInstances);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportInstancesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportInstanceResponse> response = apiInstance.AnalyticsReportInstancesGetInstanceWithHttpInfo(id, fieldsAnalyticsReportInstances);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportInstances** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReportInstances | [optional]  |

### Return type

[**AnalyticsReportInstanceResponse**](AnalyticsReportInstanceResponse.md)

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
| **200** | Single AnalyticsReportInstance |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportinstancessegmentsgettomanyrelated"></a>
# **AnalyticsReportInstancesSegmentsGetToManyRelated**
> AnalyticsReportSegmentsResponse AnalyticsReportInstancesSegmentsGetToManyRelated (string id, List<string>? fieldsAnalyticsReportSegments = null, int? limit = null)



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
    public class AnalyticsReportInstancesSegmentsGetToManyRelatedExample
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
            var apiInstance = new AnalyticsReportInstancesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAnalyticsReportSegments = new List<string>?(); // List<string>? | the fields to include for returned resources of type analyticsReportSegments (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportSegmentsResponse result = apiInstance.AnalyticsReportInstancesSegmentsGetToManyRelated(id, fieldsAnalyticsReportSegments, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesSegmentsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportInstancesSegmentsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportSegmentsResponse> response = apiInstance.AnalyticsReportInstancesSegmentsGetToManyRelatedWithHttpInfo(id, fieldsAnalyticsReportSegments, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesSegmentsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportSegments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type analyticsReportSegments | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportSegmentsResponse**](AnalyticsReportSegmentsResponse.md)

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
| **200** | List of AnalyticsReportSegments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="analyticsreportinstancessegmentsgettomanyrelationship"></a>
# **AnalyticsReportInstancesSegmentsGetToManyRelationship**
> AnalyticsReportInstanceSegmentsLinkagesResponse AnalyticsReportInstancesSegmentsGetToManyRelationship (string id, int? limit = null)



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
    public class AnalyticsReportInstancesSegmentsGetToManyRelationshipExample
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
            var apiInstance = new AnalyticsReportInstancesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AnalyticsReportInstanceSegmentsLinkagesResponse result = apiInstance.AnalyticsReportInstancesSegmentsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesSegmentsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AnalyticsReportInstancesSegmentsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AnalyticsReportInstanceSegmentsLinkagesResponse> response = apiInstance.AnalyticsReportInstancesSegmentsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AnalyticsReportInstancesApi.AnalyticsReportInstancesSegmentsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AnalyticsReportInstanceSegmentsLinkagesResponse**](AnalyticsReportInstanceSegmentsLinkagesResponse.md)

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

