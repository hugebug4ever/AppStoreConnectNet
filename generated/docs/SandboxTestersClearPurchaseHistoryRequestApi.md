# AppStoreConnect.Net.Api.SandboxTestersClearPurchaseHistoryRequestApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SandboxTestersClearPurchaseHistoryRequestV2CreateInstance**](SandboxTestersClearPurchaseHistoryRequestApi.md#sandboxtestersclearpurchasehistoryrequestv2createinstance) | **POST** /v2/sandboxTestersClearPurchaseHistoryRequest |  |

<a id="sandboxtestersclearpurchasehistoryrequestv2createinstance"></a>
# **SandboxTestersClearPurchaseHistoryRequestV2CreateInstance**
> SandboxTestersClearPurchaseHistoryRequestV2Response SandboxTestersClearPurchaseHistoryRequestV2CreateInstance (SandboxTestersClearPurchaseHistoryRequestV2CreateRequest sandboxTestersClearPurchaseHistoryRequestV2CreateRequest)



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
    public class SandboxTestersClearPurchaseHistoryRequestV2CreateInstanceExample
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
            var apiInstance = new SandboxTestersClearPurchaseHistoryRequestApi(httpClient, config, httpClientHandler);
            var sandboxTestersClearPurchaseHistoryRequestV2CreateRequest = new SandboxTestersClearPurchaseHistoryRequestV2CreateRequest(); // SandboxTestersClearPurchaseHistoryRequestV2CreateRequest | SandboxTestersClearPurchaseHistoryRequest representation

            try
            {
                SandboxTestersClearPurchaseHistoryRequestV2Response result = apiInstance.SandboxTestersClearPurchaseHistoryRequestV2CreateInstance(sandboxTestersClearPurchaseHistoryRequestV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SandboxTestersClearPurchaseHistoryRequestApi.SandboxTestersClearPurchaseHistoryRequestV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SandboxTestersClearPurchaseHistoryRequestV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SandboxTestersClearPurchaseHistoryRequestV2Response> response = apiInstance.SandboxTestersClearPurchaseHistoryRequestV2CreateInstanceWithHttpInfo(sandboxTestersClearPurchaseHistoryRequestV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SandboxTestersClearPurchaseHistoryRequestApi.SandboxTestersClearPurchaseHistoryRequestV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **sandboxTestersClearPurchaseHistoryRequestV2CreateRequest** | [**SandboxTestersClearPurchaseHistoryRequestV2CreateRequest**](SandboxTestersClearPurchaseHistoryRequestV2CreateRequest.md) | SandboxTestersClearPurchaseHistoryRequest representation |  |

### Return type

[**SandboxTestersClearPurchaseHistoryRequestV2Response**](SandboxTestersClearPurchaseHistoryRequestV2Response.md)

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
| **201** | Single SandboxTestersClearPurchaseHistoryRequest |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

