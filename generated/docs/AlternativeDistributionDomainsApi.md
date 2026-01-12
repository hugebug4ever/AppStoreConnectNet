# AppStoreConnect.Net.Api.AlternativeDistributionDomainsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionDomainsCreateInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainscreateinstance) | **POST** /v1/alternativeDistributionDomains |  |
| [**AlternativeDistributionDomainsDeleteInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsdeleteinstance) | **DELETE** /v1/alternativeDistributionDomains/{id} |  |
| [**AlternativeDistributionDomainsGetCollection**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsgetcollection) | **GET** /v1/alternativeDistributionDomains |  |
| [**AlternativeDistributionDomainsGetInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsgetinstance) | **GET** /v1/alternativeDistributionDomains/{id} |  |

<a id="alternativedistributiondomainscreateinstance"></a>
# **AlternativeDistributionDomainsCreateInstance**
> AlternativeDistributionDomainResponse AlternativeDistributionDomainsCreateInstance (AlternativeDistributionDomainCreateRequest alternativeDistributionDomainCreateRequest)



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
    public class AlternativeDistributionDomainsCreateInstanceExample
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
            var apiInstance = new AlternativeDistributionDomainsApi(httpClient, config, httpClientHandler);
            var alternativeDistributionDomainCreateRequest = new AlternativeDistributionDomainCreateRequest(); // AlternativeDistributionDomainCreateRequest | AlternativeDistributionDomain representation

            try
            {
                AlternativeDistributionDomainResponse result = apiInstance.AlternativeDistributionDomainsCreateInstance(alternativeDistributionDomainCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionDomainsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionDomainResponse> response = apiInstance.AlternativeDistributionDomainsCreateInstanceWithHttpInfo(alternativeDistributionDomainCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionDomainCreateRequest** | [**AlternativeDistributionDomainCreateRequest**](AlternativeDistributionDomainCreateRequest.md) | AlternativeDistributionDomain representation |  |

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
| **201** | Single AlternativeDistributionDomain |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributiondomainsdeleteinstance"></a>
# **AlternativeDistributionDomainsDeleteInstance**
> void AlternativeDistributionDomainsDeleteInstance (string id)



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
    public class AlternativeDistributionDomainsDeleteInstanceExample
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
            var apiInstance = new AlternativeDistributionDomainsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AlternativeDistributionDomainsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionDomainsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AlternativeDistributionDomainsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="alternativedistributiondomainsgetcollection"></a>
# **AlternativeDistributionDomainsGetCollection**
> AlternativeDistributionDomainsResponse AlternativeDistributionDomainsGetCollection (List<string>? fieldsAlternativeDistributionDomains = null, int? limit = null)



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
    public class AlternativeDistributionDomainsGetCollectionExample
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
            var apiInstance = new AlternativeDistributionDomainsApi(httpClient, config, httpClientHandler);
            var fieldsAlternativeDistributionDomains = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionDomains (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionDomainsResponse result = apiInstance.AlternativeDistributionDomainsGetCollection(fieldsAlternativeDistributionDomains, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionDomainsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionDomainsResponse> response = apiInstance.AlternativeDistributionDomainsGetCollectionWithHttpInfo(fieldsAlternativeDistributionDomains, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsAlternativeDistributionDomains** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionDomains | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionDomainsResponse**](AlternativeDistributionDomainsResponse.md)

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
| **200** | List of AlternativeDistributionDomains |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributiondomainsgetinstance"></a>
# **AlternativeDistributionDomainsGetInstance**
> AlternativeDistributionDomainResponse AlternativeDistributionDomainsGetInstance (string id, List<string>? fieldsAlternativeDistributionDomains = null)



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
    public class AlternativeDistributionDomainsGetInstanceExample
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
            var apiInstance = new AlternativeDistributionDomainsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionDomains = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionDomains (optional) 

            try
            {
                AlternativeDistributionDomainResponse result = apiInstance.AlternativeDistributionDomainsGetInstance(id, fieldsAlternativeDistributionDomains);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionDomainsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionDomainResponse> response = apiInstance.AlternativeDistributionDomainsGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionDomains);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionDomainsApi.AlternativeDistributionDomainsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionDomains** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionDomains | [optional]  |

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
| **200** | Single AlternativeDistributionDomain |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

