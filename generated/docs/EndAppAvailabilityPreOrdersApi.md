# AppStoreConnect.Net.Api.EndAppAvailabilityPreOrdersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**EndAppAvailabilityPreOrdersCreateInstance**](EndAppAvailabilityPreOrdersApi.md#endappavailabilitypreorderscreateinstance) | **POST** /v1/endAppAvailabilityPreOrders |  |

<a id="endappavailabilitypreorderscreateinstance"></a>
# **EndAppAvailabilityPreOrdersCreateInstance**
> EndAppAvailabilityPreOrderResponse EndAppAvailabilityPreOrdersCreateInstance (EndAppAvailabilityPreOrderCreateRequest endAppAvailabilityPreOrderCreateRequest)



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
    public class EndAppAvailabilityPreOrdersCreateInstanceExample
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
            var apiInstance = new EndAppAvailabilityPreOrdersApi(httpClient, config, httpClientHandler);
            var endAppAvailabilityPreOrderCreateRequest = new EndAppAvailabilityPreOrderCreateRequest(); // EndAppAvailabilityPreOrderCreateRequest | EndAppAvailabilityPreOrder representation

            try
            {
                EndAppAvailabilityPreOrderResponse result = apiInstance.EndAppAvailabilityPreOrdersCreateInstance(endAppAvailabilityPreOrderCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndAppAvailabilityPreOrdersApi.EndAppAvailabilityPreOrdersCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndAppAvailabilityPreOrdersCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EndAppAvailabilityPreOrderResponse> response = apiInstance.EndAppAvailabilityPreOrdersCreateInstanceWithHttpInfo(endAppAvailabilityPreOrderCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndAppAvailabilityPreOrdersApi.EndAppAvailabilityPreOrdersCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **endAppAvailabilityPreOrderCreateRequest** | [**EndAppAvailabilityPreOrderCreateRequest**](EndAppAvailabilityPreOrderCreateRequest.md) | EndAppAvailabilityPreOrder representation |  |

### Return type

[**EndAppAvailabilityPreOrderResponse**](EndAppAvailabilityPreOrderResponse.md)

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
| **201** | Single EndAppAvailabilityPreOrder |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

