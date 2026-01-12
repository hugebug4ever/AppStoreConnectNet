# AppStoreConnect.Net.Api.MarketplaceWebhooksApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MarketplaceWebhooksCreateInstance**](MarketplaceWebhooksApi.md#marketplacewebhookscreateinstance) | **POST** /v1/marketplaceWebhooks |  |
| [**MarketplaceWebhooksDeleteInstance**](MarketplaceWebhooksApi.md#marketplacewebhooksdeleteinstance) | **DELETE** /v1/marketplaceWebhooks/{id} |  |
| [**MarketplaceWebhooksGetCollection**](MarketplaceWebhooksApi.md#marketplacewebhooksgetcollection) | **GET** /v1/marketplaceWebhooks |  |
| [**MarketplaceWebhooksUpdateInstance**](MarketplaceWebhooksApi.md#marketplacewebhooksupdateinstance) | **PATCH** /v1/marketplaceWebhooks/{id} |  |

<a id="marketplacewebhookscreateinstance"></a>
# **MarketplaceWebhooksCreateInstance**
> MarketplaceWebhookResponse MarketplaceWebhooksCreateInstance (MarketplaceWebhookCreateRequest marketplaceWebhookCreateRequest)



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
    public class MarketplaceWebhooksCreateInstanceExample
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
            var apiInstance = new MarketplaceWebhooksApi(httpClient, config, httpClientHandler);
            var marketplaceWebhookCreateRequest = new MarketplaceWebhookCreateRequest(); // MarketplaceWebhookCreateRequest | MarketplaceWebhook representation

            try
            {
                MarketplaceWebhookResponse result = apiInstance.MarketplaceWebhooksCreateInstance(marketplaceWebhookCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceWebhooksCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MarketplaceWebhookResponse> response = apiInstance.MarketplaceWebhooksCreateInstanceWithHttpInfo(marketplaceWebhookCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **marketplaceWebhookCreateRequest** | [**MarketplaceWebhookCreateRequest**](MarketplaceWebhookCreateRequest.md) | MarketplaceWebhook representation |  |

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
| **201** | Single MarketplaceWebhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="marketplacewebhooksdeleteinstance"></a>
# **MarketplaceWebhooksDeleteInstance**
> void MarketplaceWebhooksDeleteInstance (string id)



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
    public class MarketplaceWebhooksDeleteInstanceExample
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
            var apiInstance = new MarketplaceWebhooksApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.MarketplaceWebhooksDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceWebhooksDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.MarketplaceWebhooksDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="marketplacewebhooksgetcollection"></a>
# **MarketplaceWebhooksGetCollection**
> MarketplaceWebhooksResponse MarketplaceWebhooksGetCollection (List<string>? fieldsMarketplaceWebhooks = null, int? limit = null)



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
    public class MarketplaceWebhooksGetCollectionExample
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
            var apiInstance = new MarketplaceWebhooksApi(httpClient, config, httpClientHandler);
            var fieldsMarketplaceWebhooks = new List<string>?(); // List<string>? | the fields to include for returned resources of type marketplaceWebhooks (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                MarketplaceWebhooksResponse result = apiInstance.MarketplaceWebhooksGetCollection(fieldsMarketplaceWebhooks, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceWebhooksGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MarketplaceWebhooksResponse> response = apiInstance.MarketplaceWebhooksGetCollectionWithHttpInfo(fieldsMarketplaceWebhooks, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsMarketplaceWebhooks** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type marketplaceWebhooks | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**MarketplaceWebhooksResponse**](MarketplaceWebhooksResponse.md)

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
| **200** | List of MarketplaceWebhooks |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="marketplacewebhooksupdateinstance"></a>
# **MarketplaceWebhooksUpdateInstance**
> MarketplaceWebhookResponse MarketplaceWebhooksUpdateInstance (string id, MarketplaceWebhookUpdateRequest marketplaceWebhookUpdateRequest)



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
    public class MarketplaceWebhooksUpdateInstanceExample
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
            var apiInstance = new MarketplaceWebhooksApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var marketplaceWebhookUpdateRequest = new MarketplaceWebhookUpdateRequest(); // MarketplaceWebhookUpdateRequest | MarketplaceWebhook representation

            try
            {
                MarketplaceWebhookResponse result = apiInstance.MarketplaceWebhooksUpdateInstance(id, marketplaceWebhookUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceWebhooksUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MarketplaceWebhookResponse> response = apiInstance.MarketplaceWebhooksUpdateInstanceWithHttpInfo(id, marketplaceWebhookUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceWebhooksApi.MarketplaceWebhooksUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **marketplaceWebhookUpdateRequest** | [**MarketplaceWebhookUpdateRequest**](MarketplaceWebhookUpdateRequest.md) | MarketplaceWebhook representation |  |

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
| **200** | Single MarketplaceWebhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

