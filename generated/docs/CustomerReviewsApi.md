# AppStoreConnect.Net.Api.CustomerReviewsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CustomerReviewsGetInstance**](CustomerReviewsApi.md#customerreviewsgetinstance) | **GET** /v1/customerReviews/{id} |  |
| [**CustomerReviewsResponseGetToOneRelated**](CustomerReviewsApi.md#customerreviewsresponsegettoonerelated) | **GET** /v1/customerReviews/{id}/response |  |
| [**CustomerReviewsResponseGetToOneRelationship**](CustomerReviewsApi.md#customerreviewsresponsegettoonerelationship) | **GET** /v1/customerReviews/{id}/relationships/response |  |

<a id="customerreviewsgetinstance"></a>
# **CustomerReviewsGetInstance**
> CustomerReviewResponse CustomerReviewsGetInstance (string id, List<string>? fieldsCustomerReviews = null, List<string>? fieldsCustomerReviewResponses = null, List<string>? include = null)



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
    public class CustomerReviewsGetInstanceExample
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
            var apiInstance = new CustomerReviewsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCustomerReviews = new List<string>?(); // List<string>? | the fields to include for returned resources of type customerReviews (optional) 
            var fieldsCustomerReviewResponses = new List<string>?(); // List<string>? | the fields to include for returned resources of type customerReviewResponses (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CustomerReviewResponse result = apiInstance.CustomerReviewsGetInstance(id, fieldsCustomerReviews, fieldsCustomerReviewResponses, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CustomerReviewsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CustomerReviewResponse> response = apiInstance.CustomerReviewsGetInstanceWithHttpInfo(id, fieldsCustomerReviews, fieldsCustomerReviewResponses, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCustomerReviews** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type customerReviews | [optional]  |
| **fieldsCustomerReviewResponses** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type customerReviewResponses | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CustomerReviewResponse**](CustomerReviewResponse.md)

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
| **200** | Single CustomerReview |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="customerreviewsresponsegettoonerelated"></a>
# **CustomerReviewsResponseGetToOneRelated**
> CustomerReviewResponseV1Response CustomerReviewsResponseGetToOneRelated (string id, List<string>? fieldsCustomerReviewResponses = null, List<string>? fieldsCustomerReviews = null, List<string>? include = null)



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
    public class CustomerReviewsResponseGetToOneRelatedExample
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
            var apiInstance = new CustomerReviewsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCustomerReviewResponses = new List<string>?(); // List<string>? | the fields to include for returned resources of type customerReviewResponses (optional) 
            var fieldsCustomerReviews = new List<string>?(); // List<string>? | the fields to include for returned resources of type customerReviews (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CustomerReviewResponseV1Response result = apiInstance.CustomerReviewsResponseGetToOneRelated(id, fieldsCustomerReviewResponses, fieldsCustomerReviews, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsResponseGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CustomerReviewsResponseGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CustomerReviewResponseV1Response> response = apiInstance.CustomerReviewsResponseGetToOneRelatedWithHttpInfo(id, fieldsCustomerReviewResponses, fieldsCustomerReviews, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsResponseGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCustomerReviewResponses** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type customerReviewResponses | [optional]  |
| **fieldsCustomerReviews** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type customerReviews | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CustomerReviewResponseV1Response**](CustomerReviewResponseV1Response.md)

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
| **200** | Single CustomerReviewResponse |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="customerreviewsresponsegettoonerelationship"></a>
# **CustomerReviewsResponseGetToOneRelationship**
> CustomerReviewResponseLinkageResponse CustomerReviewsResponseGetToOneRelationship (string id)



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
    public class CustomerReviewsResponseGetToOneRelationshipExample
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
            var apiInstance = new CustomerReviewsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                CustomerReviewResponseLinkageResponse result = apiInstance.CustomerReviewsResponseGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsResponseGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CustomerReviewsResponseGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CustomerReviewResponseLinkageResponse> response = apiInstance.CustomerReviewsResponseGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CustomerReviewsApi.CustomerReviewsResponseGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CustomerReviewResponseLinkageResponse**](CustomerReviewResponseLinkageResponse.md)

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

