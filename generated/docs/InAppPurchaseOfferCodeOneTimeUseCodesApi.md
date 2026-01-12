# AppStoreConnect.Net.Api.InAppPurchaseOfferCodeOneTimeUseCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodeOneTimeUseCodes |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesGetInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id} |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id} |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesvaluesgettoonerelated) | **GET** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id}/values |  |

<a id="inapppurchaseoffercodeonetimeusecodescreateinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance (InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest)



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
    public class InAppPurchaseOfferCodeOneTimeUseCodesCreateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeOneTimeUseCodesApi(httpClient, config, httpClientHandler);
            var inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest = new InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest(); // InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest | InAppPurchaseOfferCodeOneTimeUseCode representation

            try
            {
                InAppPurchaseOfferCodeOneTimeUseCodeResponse result = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance(inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeOneTimeUseCodesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeOneTimeUseCodeResponse> response = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesCreateInstanceWithHttpInfo(inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest** | [**InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest**](InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest.md) | InAppPurchaseOfferCodeOneTimeUseCode representation |  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesgetinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesGetInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesGetInstance (string id, List<string>? fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string>? include = null)



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
    public class InAppPurchaseOfferCodeOneTimeUseCodesGetInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeOneTimeUseCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsInAppPurchaseOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                InAppPurchaseOfferCodeOneTimeUseCodeResponse result = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesGetInstance(id, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeOneTimeUseCodesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeOneTimeUseCodeResponse> response = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesGetInstanceWithHttpInfo(id, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesupdateinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance (string id, InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest)



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
    public class InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodeOneTimeUseCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest = new InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest(); // InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest | InAppPurchaseOfferCodeOneTimeUseCode representation

            try
            {
                InAppPurchaseOfferCodeOneTimeUseCodeResponse result = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance(id, inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeOneTimeUseCodeResponse> response = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstanceWithHttpInfo(id, inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest** | [**InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest**](InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest.md) | InAppPurchaseOfferCodeOneTimeUseCode representation |  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesvaluesgettoonerelated"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated**
> string InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated (string id)



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
    public class InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelatedExample
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
            var apiInstance = new InAppPurchaseOfferCodeOneTimeUseCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                string result = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<string> response = apiInstance.InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelatedWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodeOneTimeUseCodesApi.InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

**string**

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCodeValue |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

