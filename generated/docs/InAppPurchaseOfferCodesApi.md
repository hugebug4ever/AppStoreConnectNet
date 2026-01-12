# AppStoreConnect.Net.Api.InAppPurchaseOfferCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodesCreateInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodes |  |
| [**InAppPurchaseOfferCodesCustomCodesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescustomcodesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/customCodes |  |
| [**InAppPurchaseOfferCodesCustomCodesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescustomcodesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/customCodes |  |
| [**InAppPurchaseOfferCodesGetInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodes/{id} |  |
| [**InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesonetimeusecodesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/oneTimeUseCodes |  |
| [**InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesonetimeusecodesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/oneTimeUseCodes |  |
| [**InAppPurchaseOfferCodesPricesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodespricesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/prices |  |
| [**InAppPurchaseOfferCodesPricesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodespricesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/prices |  |
| [**InAppPurchaseOfferCodesUpdateInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodes/{id} |  |

<a id="inapppurchaseoffercodescreateinstance"></a>
# **InAppPurchaseOfferCodesCreateInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesCreateInstance (InAppPurchaseOfferCodeCreateRequest inAppPurchaseOfferCodeCreateRequest)



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
    public class InAppPurchaseOfferCodesCreateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var inAppPurchaseOfferCodeCreateRequest = new InAppPurchaseOfferCodeCreateRequest(); // InAppPurchaseOfferCodeCreateRequest | InAppPurchaseOfferCode representation

            try
            {
                InAppPurchaseOfferCodeResponse result = apiInstance.InAppPurchaseOfferCodesCreateInstance(inAppPurchaseOfferCodeCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeResponse> response = apiInstance.InAppPurchaseOfferCodesCreateInstanceWithHttpInfo(inAppPurchaseOfferCodeCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeCreateRequest** | [**InAppPurchaseOfferCodeCreateRequest**](InAppPurchaseOfferCodeCreateRequest.md) | InAppPurchaseOfferCode representation |  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodescustomcodesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesCustomCodesGetToManyRelated**
> InAppPurchaseOfferCodeCustomCodesResponse InAppPurchaseOfferCodesCustomCodesGetToManyRelated (string id, List<string>? fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string>? fieldsActors = null, int? limit = null, List<string>? include = null)



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
    public class InAppPurchaseOfferCodesCustomCodesGetToManyRelatedExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsInAppPurchaseOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes (optional) 
            var fieldsActors = new List<string>?(); // List<string>? | the fields to include for returned resources of type actors (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                InAppPurchaseOfferCodeCustomCodesResponse result = apiInstance.InAppPurchaseOfferCodesCustomCodesGetToManyRelated(id, fieldsInAppPurchaseOfferCodeCustomCodes, fieldsActors, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCustomCodesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesCustomCodesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeCustomCodesResponse> response = apiInstance.InAppPurchaseOfferCodesCustomCodesGetToManyRelatedWithHttpInfo(id, fieldsInAppPurchaseOfferCodeCustomCodes, fieldsActors, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCustomCodesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **fieldsActors** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type actors | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeCustomCodesResponse**](InAppPurchaseOfferCodeCustomCodesResponse.md)

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
| **200** | List of InAppPurchaseOfferCodeCustomCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodescustomcodesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesCustomCodesGetToManyRelationship**
> InAppPurchaseOfferCodeCustomCodesLinkagesResponse InAppPurchaseOfferCodesCustomCodesGetToManyRelationship (string id, int? limit = null)



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
    public class InAppPurchaseOfferCodesCustomCodesGetToManyRelationshipExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                InAppPurchaseOfferCodeCustomCodesLinkagesResponse result = apiInstance.InAppPurchaseOfferCodesCustomCodesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCustomCodesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeCustomCodesLinkagesResponse> response = apiInstance.InAppPurchaseOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesCustomCodesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**InAppPurchaseOfferCodeCustomCodesLinkagesResponse**](InAppPurchaseOfferCodeCustomCodesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodesgetinstance"></a>
# **InAppPurchaseOfferCodesGetInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesGetInstance (string id, List<string>? fieldsInAppPurchaseOfferCodes = null, List<string>? fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string>? fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string>? fieldsInAppPurchaseOfferPrices = null, List<string>? include = null, int? limitCustomCodes = null, int? limitOneTimeUseCodes = null, int? limitPrices = null)



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
    public class InAppPurchaseOfferCodesGetInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsInAppPurchaseOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodes (optional) 
            var fieldsInAppPurchaseOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes (optional) 
            var fieldsInAppPurchaseOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes (optional) 
            var fieldsInAppPurchaseOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferPrices (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCustomCodes = 56;  // int? | maximum number of related customCodes returned (when they are included) (optional) 
            var limitOneTimeUseCodes = 56;  // int? | maximum number of related oneTimeUseCodes returned (when they are included) (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                InAppPurchaseOfferCodeResponse result = apiInstance.InAppPurchaseOfferCodesGetInstance(id, fieldsInAppPurchaseOfferCodes, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, fieldsInAppPurchaseOfferCodeCustomCodes, fieldsInAppPurchaseOfferPrices, include, limitCustomCodes, limitOneTimeUseCodes, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeResponse> response = apiInstance.InAppPurchaseOfferCodesGetInstanceWithHttpInfo(id, fieldsInAppPurchaseOfferCodes, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, fieldsInAppPurchaseOfferCodeCustomCodes, fieldsInAppPurchaseOfferPrices, include, limitCustomCodes, limitOneTimeUseCodes, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **fieldsInAppPurchaseOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCustomCodes** | **int?** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitOneTimeUseCodes** | **int?** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodesonetimeusecodesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated**
> InAppPurchaseOfferCodeOneTimeUseCodesResponse InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated (string id, List<string>? fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string>? fieldsActors = null, int? limit = null, List<string>? include = null)



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
    public class InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelatedExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsInAppPurchaseOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes (optional) 
            var fieldsActors = new List<string>?(); // List<string>? | the fields to include for returned resources of type actors (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                InAppPurchaseOfferCodeOneTimeUseCodesResponse result = apiInstance.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated(id, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, fieldsActors, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeOneTimeUseCodesResponse> response = apiInstance.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo(id, fieldsInAppPurchaseOfferCodeOneTimeUseCodes, fieldsActors, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsActors** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type actors | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodesResponse**](InAppPurchaseOfferCodeOneTimeUseCodesResponse.md)

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
| **200** | List of InAppPurchaseOfferCodeOneTimeUseCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodesonetimeusecodesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship**
> InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship (string id, int? limit = null)



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
    public class InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationshipExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse result = apiInstance.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse> response = apiInstance.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse**](InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodespricesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesPricesGetToManyRelated**
> InAppPurchaseOfferPricesResponse InAppPurchaseOfferCodesPricesGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsInAppPurchaseOfferPrices = null, List<string>? fieldsTerritories = null, List<string>? fieldsInAppPurchasePricePoints = null, int? limit = null, List<string>? include = null)



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
    public class InAppPurchaseOfferCodesPricesGetToManyRelatedExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsInAppPurchaseOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchaseOfferPrices (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsInAppPurchasePricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchasePricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                InAppPurchaseOfferPricesResponse result = apiInstance.InAppPurchaseOfferCodesPricesGetToManyRelated(id, filterTerritory, fieldsInAppPurchaseOfferPrices, fieldsTerritories, fieldsInAppPurchasePricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesPricesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesPricesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferPricesResponse> response = apiInstance.InAppPurchaseOfferCodesPricesGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsInAppPurchaseOfferPrices, fieldsTerritories, fieldsInAppPurchasePricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesPricesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsInAppPurchaseOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferPricesResponse**](InAppPurchaseOfferPricesResponse.md)

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
| **200** | List of InAppPurchaseOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="inapppurchaseoffercodespricesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesPricesGetToManyRelationship**
> InAppPurchaseOfferCodePricesLinkagesResponse InAppPurchaseOfferCodesPricesGetToManyRelationship (string id, int? limit = null)



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
    public class InAppPurchaseOfferCodesPricesGetToManyRelationshipExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                InAppPurchaseOfferCodePricesLinkagesResponse result = apiInstance.InAppPurchaseOfferCodesPricesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesPricesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesPricesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodePricesLinkagesResponse> response = apiInstance.InAppPurchaseOfferCodesPricesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesPricesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**InAppPurchaseOfferCodePricesLinkagesResponse**](InAppPurchaseOfferCodePricesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodesupdateinstance"></a>
# **InAppPurchaseOfferCodesUpdateInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesUpdateInstance (string id, InAppPurchaseOfferCodeUpdateRequest inAppPurchaseOfferCodeUpdateRequest)



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
    public class InAppPurchaseOfferCodesUpdateInstanceExample
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
            var apiInstance = new InAppPurchaseOfferCodesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var inAppPurchaseOfferCodeUpdateRequest = new InAppPurchaseOfferCodeUpdateRequest(); // InAppPurchaseOfferCodeUpdateRequest | InAppPurchaseOfferCode representation

            try
            {
                InAppPurchaseOfferCodeResponse result = apiInstance.InAppPurchaseOfferCodesUpdateInstance(id, inAppPurchaseOfferCodeUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InAppPurchaseOfferCodesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<InAppPurchaseOfferCodeResponse> response = apiInstance.InAppPurchaseOfferCodesUpdateInstanceWithHttpInfo(id, inAppPurchaseOfferCodeUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InAppPurchaseOfferCodesApi.InAppPurchaseOfferCodesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeUpdateRequest** | [**InAppPurchaseOfferCodeUpdateRequest**](InAppPurchaseOfferCodeUpdateRequest.md) | InAppPurchaseOfferCode representation |  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

