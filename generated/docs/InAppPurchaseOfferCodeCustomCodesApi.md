# AppStoreConnect.Net.Api.InAppPurchaseOfferCodeCustomCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodeCustomCodesCreateInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodeCustomCodes |  |
| [**InAppPurchaseOfferCodeCustomCodesGetInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodeCustomCodes/{id} |  |
| [**InAppPurchaseOfferCodeCustomCodesUpdateInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodeCustomCodes/{id} |  |

<a id="inapppurchaseoffercodecustomcodescreateinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesCreateInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesCreateInstance (InAppPurchaseOfferCodeCustomCodeCreateRequest inAppPurchaseOfferCodeCustomCodeCreateRequest)



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
    public class InAppPurchaseOfferCodeCustomCodesCreateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeCustomCodesApi(httpClient, config, httpClientHandler);
            var inAppPurchaseOfferCodeCustomCodeCreateRequest = new InAppPurchaseOfferCodeCustomCodeCreateRequest(); // InAppPurchaseOfferCodeCustomCodeCreateRequest | InAppPurchaseOfferCodeCustomCode representation

            try
            {
                InAppPurchaseOfferCodeCustomCodeResponse result = apiInstance.InAppPurchaseOfferCodeCustomCodesCreateInstance(inAppPurchaseOfferCodeCustomCodeCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeCustomCodesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeCustomCodeResponse> response = apiInstance.InAppPurchaseOfferCodeCustomCodesCreateInstanceWithHttpInfo(inAppPurchaseOfferCodeCustomCodeCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeCustomCodeCreateRequest** | [**InAppPurchaseOfferCodeCustomCodeCreateRequest**](InAppPurchaseOfferCodeCustomCodeCreateRequest.md) | InAppPurchaseOfferCodeCustomCode representation |  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodecustomcodesgetinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesGetInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesGetInstance (string id, List<string>? fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string>? include = null)



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
    public class InAppPurchaseOfferCodeCustomCodesGetInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeCustomCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsInAppPurchaseOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                InAppPurchaseOfferCodeCustomCodeResponse result = apiInstance.InAppPurchaseOfferCodeCustomCodesGetInstance(id, fieldsInAppPurchaseOfferCodeCustomCodes, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeCustomCodesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeCustomCodeResponse> response = apiInstance.InAppPurchaseOfferCodeCustomCodesGetInstanceWithHttpInfo(id, fieldsInAppPurchaseOfferCodeCustomCodes, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodecustomcodesupdateinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesUpdateInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesUpdateInstance (string id, InAppPurchaseOfferCodeCustomCodeUpdateRequest inAppPurchaseOfferCodeCustomCodeUpdateRequest)



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
    public class InAppPurchaseOfferCodeCustomCodesUpdateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeCustomCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var inAppPurchaseOfferCodeCustomCodeUpdateRequest = new InAppPurchaseOfferCodeCustomCodeUpdateRequest(); // InAppPurchaseOfferCodeCustomCodeUpdateRequest | InAppPurchaseOfferCodeCustomCode representation

            try
            {
                InAppPurchaseOfferCodeCustomCodeResponse result = apiInstance.InAppPurchaseOfferCodeCustomCodesUpdateInstance(id, inAppPurchaseOfferCodeCustomCodeUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeCustomCodesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeCustomCodeResponse> response = apiInstance.InAppPurchaseOfferCodeCustomCodesUpdateInstanceWithHttpInfo(id, inAppPurchaseOfferCodeCustomCodeUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeCustomCodesApi.InAppPurchaseOfferCodeCustomCodesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeCustomCodeUpdateRequest** | [**InAppPurchaseOfferCodeCustomCodeUpdateRequest**](InAppPurchaseOfferCodeCustomCodeUpdateRequest.md) | InAppPurchaseOfferCodeCustomCode representation |  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

