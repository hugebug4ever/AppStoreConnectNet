# AppStoreConnect.Net.Api.SubscriptionPromotionalOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionPromotionalOffersCreateInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferscreateinstance) | **POST** /v1/subscriptionPromotionalOffers |  |
| [**SubscriptionPromotionalOffersDeleteInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersdeleteinstance) | **DELETE** /v1/subscriptionPromotionalOffers/{id} |  |
| [**SubscriptionPromotionalOffersGetInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersgetinstance) | **GET** /v1/subscriptionPromotionalOffers/{id} |  |
| [**SubscriptionPromotionalOffersPricesGetToManyRelated**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferspricesgettomanyrelated) | **GET** /v1/subscriptionPromotionalOffers/{id}/prices |  |
| [**SubscriptionPromotionalOffersPricesGetToManyRelationship**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferspricesgettomanyrelationship) | **GET** /v1/subscriptionPromotionalOffers/{id}/relationships/prices |  |
| [**SubscriptionPromotionalOffersUpdateInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersupdateinstance) | **PATCH** /v1/subscriptionPromotionalOffers/{id} |  |

<a id="subscriptionpromotionalofferscreateinstance"></a>
# **SubscriptionPromotionalOffersCreateInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersCreateInstance (SubscriptionPromotionalOfferCreateRequest subscriptionPromotionalOfferCreateRequest)



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
    public class SubscriptionPromotionalOffersCreateInstanceExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var subscriptionPromotionalOfferCreateRequest = new SubscriptionPromotionalOfferCreateRequest(); // SubscriptionPromotionalOfferCreateRequest | SubscriptionPromotionalOffer representation

            try
            {
                SubscriptionPromotionalOfferResponse result = apiInstance.SubscriptionPromotionalOffersCreateInstance(subscriptionPromotionalOfferCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOfferResponse> response = apiInstance.SubscriptionPromotionalOffersCreateInstanceWithHttpInfo(subscriptionPromotionalOfferCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionPromotionalOfferCreateRequest** | [**SubscriptionPromotionalOfferCreateRequest**](SubscriptionPromotionalOfferCreateRequest.md) | SubscriptionPromotionalOffer representation |  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **201** | Single SubscriptionPromotionalOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionpromotionaloffersdeleteinstance"></a>
# **SubscriptionPromotionalOffersDeleteInstance**
> void SubscriptionPromotionalOffersDeleteInstance (string id)



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
    public class SubscriptionPromotionalOffersDeleteInstanceExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.SubscriptionPromotionalOffersDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.SubscriptionPromotionalOffersDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="subscriptionpromotionaloffersgetinstance"></a>
# **SubscriptionPromotionalOffersGetInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersGetInstance (string id, List<string>? fieldsSubscriptionPromotionalOffers = null, List<string>? fieldsSubscriptionPromotionalOfferPrices = null, List<string>? include = null, int? limitPrices = null)



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
    public class SubscriptionPromotionalOffersGetInstanceExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionPromotionalOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOffers (optional) 
            var fieldsSubscriptionPromotionalOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOfferPrices (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                SubscriptionPromotionalOfferResponse result = apiInstance.SubscriptionPromotionalOffersGetInstance(id, fieldsSubscriptionPromotionalOffers, fieldsSubscriptionPromotionalOfferPrices, include, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOfferResponse> response = apiInstance.SubscriptionPromotionalOffersGetInstanceWithHttpInfo(id, fieldsSubscriptionPromotionalOffers, fieldsSubscriptionPromotionalOfferPrices, include, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **200** | Single SubscriptionPromotionalOffer |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionpromotionalofferspricesgettomanyrelated"></a>
# **SubscriptionPromotionalOffersPricesGetToManyRelated**
> SubscriptionPromotionalOfferPricesResponse SubscriptionPromotionalOffersPricesGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionPromotionalOfferPrices = null, List<string>? fieldsTerritories = null, List<string>? fieldsSubscriptionPricePoints = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionPromotionalOffersPricesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsSubscriptionPromotionalOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOfferPrices (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionPromotionalOfferPricesResponse result = apiInstance.SubscriptionPromotionalOffersPricesGetToManyRelated(id, filterTerritory, fieldsSubscriptionPromotionalOfferPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersPricesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersPricesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOfferPricesResponse> response = apiInstance.SubscriptionPromotionalOffersPricesGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionPromotionalOfferPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersPricesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPromotionalOfferPricesResponse**](SubscriptionPromotionalOfferPricesResponse.md)

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
| **200** | List of SubscriptionPromotionalOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionpromotionalofferspricesgettomanyrelationship"></a>
# **SubscriptionPromotionalOffersPricesGetToManyRelationship**
> SubscriptionPromotionalOfferPricesLinkagesResponse SubscriptionPromotionalOffersPricesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionPromotionalOffersPricesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionPromotionalOfferPricesLinkagesResponse result = apiInstance.SubscriptionPromotionalOffersPricesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersPricesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersPricesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOfferPricesLinkagesResponse> response = apiInstance.SubscriptionPromotionalOffersPricesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersPricesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionPromotionalOfferPricesLinkagesResponse**](SubscriptionPromotionalOfferPricesLinkagesResponse.md)

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

<a id="subscriptionpromotionaloffersupdateinstance"></a>
# **SubscriptionPromotionalOffersUpdateInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersUpdateInstance (string id, SubscriptionPromotionalOfferUpdateRequest subscriptionPromotionalOfferUpdateRequest)



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
    public class SubscriptionPromotionalOffersUpdateInstanceExample
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
            var apiInstance = new SubscriptionPromotionalOffersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var subscriptionPromotionalOfferUpdateRequest = new SubscriptionPromotionalOfferUpdateRequest(); // SubscriptionPromotionalOfferUpdateRequest | SubscriptionPromotionalOffer representation

            try
            {
                SubscriptionPromotionalOfferResponse result = apiInstance.SubscriptionPromotionalOffersUpdateInstance(id, subscriptionPromotionalOfferUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionPromotionalOffersUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOfferResponse> response = apiInstance.SubscriptionPromotionalOffersUpdateInstanceWithHttpInfo(id, subscriptionPromotionalOfferUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionPromotionalOffersApi.SubscriptionPromotionalOffersUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionPromotionalOfferUpdateRequest** | [**SubscriptionPromotionalOfferUpdateRequest**](SubscriptionPromotionalOfferUpdateRequest.md) | SubscriptionPromotionalOffer representation |  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **200** | Single SubscriptionPromotionalOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

