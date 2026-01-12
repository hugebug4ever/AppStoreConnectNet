# AppStoreConnect.Net.Api.MarketplaceSearchDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MarketplaceSearchDetailsCreateInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailscreateinstance) | **POST** /v1/marketplaceSearchDetails |  |
| [**MarketplaceSearchDetailsDeleteInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailsdeleteinstance) | **DELETE** /v1/marketplaceSearchDetails/{id} |  |
| [**MarketplaceSearchDetailsUpdateInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailsupdateinstance) | **PATCH** /v1/marketplaceSearchDetails/{id} |  |

<a id="marketplacesearchdetailscreateinstance"></a>
# **MarketplaceSearchDetailsCreateInstance**
> MarketplaceSearchDetailResponse MarketplaceSearchDetailsCreateInstance (MarketplaceSearchDetailCreateRequest marketplaceSearchDetailCreateRequest)



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
    public class MarketplaceSearchDetailsCreateInstanceExample
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
            var apiInstance = new MarketplaceSearchDetailsApi(httpClient, config, httpClientHandler);
            var marketplaceSearchDetailCreateRequest = new MarketplaceSearchDetailCreateRequest(); // MarketplaceSearchDetailCreateRequest | MarketplaceSearchDetail representation

            try
            {
                MarketplaceSearchDetailResponse result = apiInstance.MarketplaceSearchDetailsCreateInstance(marketplaceSearchDetailCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceSearchDetailsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MarketplaceSearchDetailResponse> response = apiInstance.MarketplaceSearchDetailsCreateInstanceWithHttpInfo(marketplaceSearchDetailCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **marketplaceSearchDetailCreateRequest** | [**MarketplaceSearchDetailCreateRequest**](MarketplaceSearchDetailCreateRequest.md) | MarketplaceSearchDetail representation |  |

### Return type

[**MarketplaceSearchDetailResponse**](MarketplaceSearchDetailResponse.md)

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
| **201** | Single MarketplaceSearchDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="marketplacesearchdetailsdeleteinstance"></a>
# **MarketplaceSearchDetailsDeleteInstance**
> void MarketplaceSearchDetailsDeleteInstance (string id)



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
    public class MarketplaceSearchDetailsDeleteInstanceExample
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
            var apiInstance = new MarketplaceSearchDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.MarketplaceSearchDetailsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceSearchDetailsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.MarketplaceSearchDetailsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="marketplacesearchdetailsupdateinstance"></a>
# **MarketplaceSearchDetailsUpdateInstance**
> MarketplaceSearchDetailResponse MarketplaceSearchDetailsUpdateInstance (string id, MarketplaceSearchDetailUpdateRequest marketplaceSearchDetailUpdateRequest)



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
    public class MarketplaceSearchDetailsUpdateInstanceExample
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
            var apiInstance = new MarketplaceSearchDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var marketplaceSearchDetailUpdateRequest = new MarketplaceSearchDetailUpdateRequest(); // MarketplaceSearchDetailUpdateRequest | MarketplaceSearchDetail representation

            try
            {
                MarketplaceSearchDetailResponse result = apiInstance.MarketplaceSearchDetailsUpdateInstance(id, marketplaceSearchDetailUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MarketplaceSearchDetailsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MarketplaceSearchDetailResponse> response = apiInstance.MarketplaceSearchDetailsUpdateInstanceWithHttpInfo(id, marketplaceSearchDetailUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MarketplaceSearchDetailsApi.MarketplaceSearchDetailsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **marketplaceSearchDetailUpdateRequest** | [**MarketplaceSearchDetailUpdateRequest**](MarketplaceSearchDetailUpdateRequest.md) | MarketplaceSearchDetail representation |  |

### Return type

[**MarketplaceSearchDetailResponse**](MarketplaceSearchDetailResponse.md)

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
| **200** | Single MarketplaceSearchDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

