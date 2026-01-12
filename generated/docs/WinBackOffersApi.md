# AppStoreConnect.Net.Api.WinBackOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**WinBackOffersCreateInstance**](WinBackOffersApi.md#winbackofferscreateinstance) | **POST** /v1/winBackOffers |  |
| [**WinBackOffersDeleteInstance**](WinBackOffersApi.md#winbackoffersdeleteinstance) | **DELETE** /v1/winBackOffers/{id} |  |
| [**WinBackOffersGetInstance**](WinBackOffersApi.md#winbackoffersgetinstance) | **GET** /v1/winBackOffers/{id} |  |
| [**WinBackOffersPricesGetToManyRelated**](WinBackOffersApi.md#winbackofferspricesgettomanyrelated) | **GET** /v1/winBackOffers/{id}/prices |  |
| [**WinBackOffersPricesGetToManyRelationship**](WinBackOffersApi.md#winbackofferspricesgettomanyrelationship) | **GET** /v1/winBackOffers/{id}/relationships/prices |  |
| [**WinBackOffersUpdateInstance**](WinBackOffersApi.md#winbackoffersupdateinstance) | **PATCH** /v1/winBackOffers/{id} |  |

<a id="winbackofferscreateinstance"></a>
# **WinBackOffersCreateInstance**
> WinBackOfferResponse WinBackOffersCreateInstance (WinBackOfferCreateRequest winBackOfferCreateRequest)



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
    public class WinBackOffersCreateInstanceExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var winBackOfferCreateRequest = new WinBackOfferCreateRequest(); // WinBackOfferCreateRequest | WinBackOffer representation

            try
            {
                WinBackOfferResponse result = apiInstance.WinBackOffersCreateInstance(winBackOfferCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOfferResponse> response = apiInstance.WinBackOffersCreateInstanceWithHttpInfo(winBackOfferCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **winBackOfferCreateRequest** | [**WinBackOfferCreateRequest**](WinBackOfferCreateRequest.md) | WinBackOffer representation |  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **201** | Single WinBackOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="winbackoffersdeleteinstance"></a>
# **WinBackOffersDeleteInstance**
> void WinBackOffersDeleteInstance (string id)



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
    public class WinBackOffersDeleteInstanceExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.WinBackOffersDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.WinBackOffersDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="winbackoffersgetinstance"></a>
# **WinBackOffersGetInstance**
> WinBackOfferResponse WinBackOffersGetInstance (string id, List<string>? fieldsWinBackOffers = null, List<string>? fieldsWinBackOfferPrices = null, List<string>? include = null, int? limitPrices = null)



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
    public class WinBackOffersGetInstanceExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsWinBackOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOffers (optional) 
            var fieldsWinBackOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOfferPrices (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                WinBackOfferResponse result = apiInstance.WinBackOffersGetInstance(id, fieldsWinBackOffers, fieldsWinBackOfferPrices, include, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOfferResponse> response = apiInstance.WinBackOffersGetInstanceWithHttpInfo(id, fieldsWinBackOffers, fieldsWinBackOfferPrices, include, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **200** | Single WinBackOffer |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="winbackofferspricesgettomanyrelated"></a>
# **WinBackOffersPricesGetToManyRelated**
> WinBackOfferPricesResponse WinBackOffersPricesGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsWinBackOfferPrices = null, List<string>? fieldsTerritories = null, List<string>? fieldsSubscriptionPricePoints = null, int? limit = null, List<string>? include = null)



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
    public class WinBackOffersPricesGetToManyRelatedExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsWinBackOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOfferPrices (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                WinBackOfferPricesResponse result = apiInstance.WinBackOffersPricesGetToManyRelated(id, filterTerritory, fieldsWinBackOfferPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersPricesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersPricesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOfferPricesResponse> response = apiInstance.WinBackOffersPricesGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsWinBackOfferPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersPricesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**WinBackOfferPricesResponse**](WinBackOfferPricesResponse.md)

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
| **200** | List of WinBackOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="winbackofferspricesgettomanyrelationship"></a>
# **WinBackOffersPricesGetToManyRelationship**
> WinBackOfferPricesLinkagesResponse WinBackOffersPricesGetToManyRelationship (string id, int? limit = null)



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
    public class WinBackOffersPricesGetToManyRelationshipExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                WinBackOfferPricesLinkagesResponse result = apiInstance.WinBackOffersPricesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersPricesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersPricesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOfferPricesLinkagesResponse> response = apiInstance.WinBackOffersPricesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersPricesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**WinBackOfferPricesLinkagesResponse**](WinBackOfferPricesLinkagesResponse.md)

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

<a id="winbackoffersupdateinstance"></a>
# **WinBackOffersUpdateInstance**
> WinBackOfferResponse WinBackOffersUpdateInstance (string id, WinBackOfferUpdateRequest winBackOfferUpdateRequest)



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
    public class WinBackOffersUpdateInstanceExample
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
            var apiInstance = new WinBackOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var winBackOfferUpdateRequest = new WinBackOfferUpdateRequest(); // WinBackOfferUpdateRequest | WinBackOffer representation

            try
            {
                WinBackOfferResponse result = apiInstance.WinBackOffersUpdateInstance(id, winBackOfferUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the WinBackOffersUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOfferResponse> response = apiInstance.WinBackOffersUpdateInstanceWithHttpInfo(id, winBackOfferUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling WinBackOffersApi.WinBackOffersUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **winBackOfferUpdateRequest** | [**WinBackOfferUpdateRequest**](WinBackOfferUpdateRequest.md) | WinBackOffer representation |  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **200** | Single WinBackOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

