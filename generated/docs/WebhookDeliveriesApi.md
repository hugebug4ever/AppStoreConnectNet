# AppStoreConnect.Net.Api.WebhookDeliveriesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**WebhookDeliveriesCreateInstance**](WebhookDeliveriesApi.md#webhookdeliveriescreateinstance) | **POST** /v1/webhookDeliveries |  |

<a id="webhookdeliveriescreateinstance"></a>
# **WebhookDeliveriesCreateInstance**
> WebhookDeliveryResponse WebhookDeliveriesCreateInstance (WebhookDeliveryCreateRequest webhookDeliveryCreateRequest)



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
    public class WebhookDeliveriesCreateInstanceExample
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
            var apiInstance = new WebhookDeliveriesApi(httpClient, config, httpClientHandler);
            var webhookDeliveryCreateRequest = new WebhookDeliveryCreateRequest(); // WebhookDeliveryCreateRequest | WebhookDelivery representation

            try
            {
                WebhookDeliveryResponse result = apiInstance.WebhookDeliveriesCreateInstance(webhookDeliveryCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WebhookDeliveriesApi.WebhookDeliveriesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WebhookDeliveriesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WebhookDeliveryResponse> response = apiInstance.WebhookDeliveriesCreateInstanceWithHttpInfo(webhookDeliveryCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WebhookDeliveriesApi.WebhookDeliveriesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **webhookDeliveryCreateRequest** | [**WebhookDeliveryCreateRequest**](WebhookDeliveryCreateRequest.md) | WebhookDelivery representation |  |

### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

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
| **201** | Single WebhookDelivery |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

