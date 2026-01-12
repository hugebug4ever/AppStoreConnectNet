# AppStoreConnect.Net.Api.SubscriptionOfferCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionOfferCodesCreateInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodescreateinstance) | **POST** /v1/subscriptionOfferCodes |  |
| [**SubscriptionOfferCodesCustomCodesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodescustomcodesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/customCodes |  |
| [**SubscriptionOfferCodesCustomCodesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodescustomcodesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/customCodes |  |
| [**SubscriptionOfferCodesGetInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodesgetinstance) | **GET** /v1/subscriptionOfferCodes/{id} |  |
| [**SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodesonetimeusecodesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/oneTimeUseCodes |  |
| [**SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodesonetimeusecodesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/oneTimeUseCodes |  |
| [**SubscriptionOfferCodesPricesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodespricesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/prices |  |
| [**SubscriptionOfferCodesPricesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodespricesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/prices |  |
| [**SubscriptionOfferCodesUpdateInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodesupdateinstance) | **PATCH** /v1/subscriptionOfferCodes/{id} |  |

<a id="subscriptionoffercodescreateinstance"></a>
# **SubscriptionOfferCodesCreateInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesCreateInstance (SubscriptionOfferCodeCreateRequest subscriptionOfferCodeCreateRequest)



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
    public class SubscriptionOfferCodesCreateInstanceExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var subscriptionOfferCodeCreateRequest = new SubscriptionOfferCodeCreateRequest(); // SubscriptionOfferCodeCreateRequest | SubscriptionOfferCode representation

            try
            {
                SubscriptionOfferCodeResponse result = apiInstance.SubscriptionOfferCodesCreateInstance(subscriptionOfferCodeCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeResponse> response = apiInstance.SubscriptionOfferCodesCreateInstanceWithHttpInfo(subscriptionOfferCodeCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionOfferCodeCreateRequest** | [**SubscriptionOfferCodeCreateRequest**](SubscriptionOfferCodeCreateRequest.md) | SubscriptionOfferCode representation |  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **201** | Single SubscriptionOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionoffercodescustomcodesgettomanyrelated"></a>
# **SubscriptionOfferCodesCustomCodesGetToManyRelated**
> SubscriptionOfferCodeCustomCodesResponse SubscriptionOfferCodesCustomCodesGetToManyRelated (string id, List<string>? fieldsSubscriptionOfferCodeCustomCodes = null, List<string>? fieldsSubscriptionOfferCodes = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionOfferCodesCustomCodesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional) 
            var fieldsSubscriptionOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodes (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionOfferCodeCustomCodesResponse result = apiInstance.SubscriptionOfferCodesCustomCodesGetToManyRelated(id, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodes, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCustomCodesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesCustomCodesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeCustomCodesResponse> response = apiInstance.SubscriptionOfferCodesCustomCodesGetToManyRelatedWithHttpInfo(id, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodes, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCustomCodesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodeCustomCodesResponse**](SubscriptionOfferCodeCustomCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodeCustomCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionoffercodescustomcodesgettomanyrelationship"></a>
# **SubscriptionOfferCodesCustomCodesGetToManyRelationship**
> SubscriptionOfferCodeCustomCodesLinkagesResponse SubscriptionOfferCodesCustomCodesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionOfferCodesCustomCodesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionOfferCodeCustomCodesLinkagesResponse result = apiInstance.SubscriptionOfferCodesCustomCodesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCustomCodesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeCustomCodesLinkagesResponse> response = apiInstance.SubscriptionOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionOfferCodeCustomCodesLinkagesResponse**](SubscriptionOfferCodeCustomCodesLinkagesResponse.md)

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

<a id="subscriptionoffercodesgetinstance"></a>
# **SubscriptionOfferCodesGetInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesGetInstance (string id, List<string>? fieldsSubscriptionOfferCodes = null, List<string>? fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string>? fieldsSubscriptionOfferCodeCustomCodes = null, List<string>? fieldsSubscriptionOfferCodePrices = null, List<string>? include = null, int? limitCustomCodes = null, int? limitOneTimeUseCodes = null, int? limitPrices = null)



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
    public class SubscriptionOfferCodesGetInstanceExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodes (optional) 
            var fieldsSubscriptionOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional) 
            var fieldsSubscriptionOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional) 
            var fieldsSubscriptionOfferCodePrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodePrices (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCustomCodes = 56;  // int? | maximum number of related customCodes returned (when they are included) (optional) 
            var limitOneTimeUseCodes = 56;  // int? | maximum number of related oneTimeUseCodes returned (when they are included) (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                SubscriptionOfferCodeResponse result = apiInstance.SubscriptionOfferCodesGetInstance(id, fieldsSubscriptionOfferCodes, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodePrices, include, limitCustomCodes, limitOneTimeUseCodes, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeResponse> response = apiInstance.SubscriptionOfferCodesGetInstanceWithHttpInfo(id, fieldsSubscriptionOfferCodes, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodePrices, include, limitCustomCodes, limitOneTimeUseCodes, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCustomCodes** | **int?** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitOneTimeUseCodes** | **int?** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **200** | Single SubscriptionOfferCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionoffercodesonetimeusecodesgettomanyrelated"></a>
# **SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated**
> SubscriptionOfferCodeOneTimeUseCodesResponse SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated (string id, List<string>? fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string>? fieldsSubscriptionOfferCodes = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionOfferCodesOneTimeUseCodesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional) 
            var fieldsSubscriptionOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodes (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionOfferCodeOneTimeUseCodesResponse result = apiInstance.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated(id, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodes, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeOneTimeUseCodesResponse> response = apiInstance.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo(id, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodes, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodeOneTimeUseCodesResponse**](SubscriptionOfferCodeOneTimeUseCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodeOneTimeUseCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionoffercodesonetimeusecodesgettomanyrelationship"></a>
# **SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship**
> SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse result = apiInstance.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse> response = apiInstance.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse**](SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.md)

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

<a id="subscriptionoffercodespricesgettomanyrelated"></a>
# **SubscriptionOfferCodesPricesGetToManyRelated**
> SubscriptionOfferCodePricesResponse SubscriptionOfferCodesPricesGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionOfferCodePrices = null, List<string>? fieldsTerritories = null, List<string>? fieldsSubscriptionPricePoints = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionOfferCodesPricesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsSubscriptionOfferCodePrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodePrices (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionOfferCodePricesResponse result = apiInstance.SubscriptionOfferCodesPricesGetToManyRelated(id, filterTerritory, fieldsSubscriptionOfferCodePrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesPricesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesPricesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodePricesResponse> response = apiInstance.SubscriptionOfferCodesPricesGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionOfferCodePrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesPricesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodePricesResponse**](SubscriptionOfferCodePricesResponse.md)

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
| **200** | List of SubscriptionOfferCodePrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionoffercodespricesgettomanyrelationship"></a>
# **SubscriptionOfferCodesPricesGetToManyRelationship**
> SubscriptionOfferCodePricesLinkagesResponse SubscriptionOfferCodesPricesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionOfferCodesPricesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionOfferCodePricesLinkagesResponse result = apiInstance.SubscriptionOfferCodesPricesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesPricesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesPricesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodePricesLinkagesResponse> response = apiInstance.SubscriptionOfferCodesPricesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesPricesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionOfferCodePricesLinkagesResponse**](SubscriptionOfferCodePricesLinkagesResponse.md)

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

<a id="subscriptionoffercodesupdateinstance"></a>
# **SubscriptionOfferCodesUpdateInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesUpdateInstance (string id, SubscriptionOfferCodeUpdateRequest subscriptionOfferCodeUpdateRequest)



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
    public class SubscriptionOfferCodesUpdateInstanceExample
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
            var apiInstance = new SubscriptionOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var subscriptionOfferCodeUpdateRequest = new SubscriptionOfferCodeUpdateRequest(); // SubscriptionOfferCodeUpdateRequest | SubscriptionOfferCode representation

            try
            {
                SubscriptionOfferCodeResponse result = apiInstance.SubscriptionOfferCodesUpdateInstance(id, subscriptionOfferCodeUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionOfferCodesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodeResponse> response = apiInstance.SubscriptionOfferCodesUpdateInstanceWithHttpInfo(id, subscriptionOfferCodeUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionOfferCodesApi.SubscriptionOfferCodesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionOfferCodeUpdateRequest** | [**SubscriptionOfferCodeUpdateRequest**](SubscriptionOfferCodeUpdateRequest.md) | SubscriptionOfferCode representation |  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **200** | Single SubscriptionOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

