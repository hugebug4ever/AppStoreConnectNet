# AppStoreConnect.Net.Api.AlternativeDistributionKeysApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionKeysCreateInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeyscreateinstance) | **POST** /v1/alternativeDistributionKeys |  |
| [**AlternativeDistributionKeysDeleteInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeysdeleteinstance) | **DELETE** /v1/alternativeDistributionKeys/{id} |  |
| [**AlternativeDistributionKeysGetCollection**](AlternativeDistributionKeysApi.md#alternativedistributionkeysgetcollection) | **GET** /v1/alternativeDistributionKeys |  |
| [**AlternativeDistributionKeysGetInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeysgetinstance) | **GET** /v1/alternativeDistributionKeys/{id} |  |

<a id="alternativedistributionkeyscreateinstance"></a>
# **AlternativeDistributionKeysCreateInstance**
> AlternativeDistributionKeyResponse AlternativeDistributionKeysCreateInstance (AlternativeDistributionKeyCreateRequest alternativeDistributionKeyCreateRequest)



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
    public class AlternativeDistributionKeysCreateInstanceExample
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
            var apiInstance = new AlternativeDistributionKeysApi(httpClient, config, httpClientHandler);
            var alternativeDistributionKeyCreateRequest = new AlternativeDistributionKeyCreateRequest(); // AlternativeDistributionKeyCreateRequest | AlternativeDistributionKey representation

            try
            {
                AlternativeDistributionKeyResponse result = apiInstance.AlternativeDistributionKeysCreateInstance(alternativeDistributionKeyCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionKeysCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionKeyResponse> response = apiInstance.AlternativeDistributionKeysCreateInstanceWithHttpInfo(alternativeDistributionKeyCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionKeyCreateRequest** | [**AlternativeDistributionKeyCreateRequest**](AlternativeDistributionKeyCreateRequest.md) | AlternativeDistributionKey representation |  |

### Return type

[**AlternativeDistributionKeyResponse**](AlternativeDistributionKeyResponse.md)

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
| **201** | Single AlternativeDistributionKey |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionkeysdeleteinstance"></a>
# **AlternativeDistributionKeysDeleteInstance**
> void AlternativeDistributionKeysDeleteInstance (string id)



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
    public class AlternativeDistributionKeysDeleteInstanceExample
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
            var apiInstance = new AlternativeDistributionKeysApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AlternativeDistributionKeysDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionKeysDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AlternativeDistributionKeysDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="alternativedistributionkeysgetcollection"></a>
# **AlternativeDistributionKeysGetCollection**
> AlternativeDistributionKeysResponse AlternativeDistributionKeysGetCollection (bool? existsApp = null, List<string>? fieldsAlternativeDistributionKeys = null, int? limit = null)



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
    public class AlternativeDistributionKeysGetCollectionExample
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
            var apiInstance = new AlternativeDistributionKeysApi(httpClient, config, httpClientHandler);
            var existsApp = true;  // bool? | filter by existence or non-existence of related 'app' (optional) 
            var fieldsAlternativeDistributionKeys = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionKeys (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionKeysResponse result = apiInstance.AlternativeDistributionKeysGetCollection(existsApp, fieldsAlternativeDistributionKeys, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionKeysGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionKeysResponse> response = apiInstance.AlternativeDistributionKeysGetCollectionWithHttpInfo(existsApp, fieldsAlternativeDistributionKeys, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **existsApp** | **bool?** | filter by existence or non-existence of related &#39;app&#39; | [optional]  |
| **fieldsAlternativeDistributionKeys** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionKeys | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionKeysResponse**](AlternativeDistributionKeysResponse.md)

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
| **200** | List of AlternativeDistributionKeys |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionkeysgetinstance"></a>
# **AlternativeDistributionKeysGetInstance**
> AlternativeDistributionKeyResponse AlternativeDistributionKeysGetInstance (string id, List<string>? fieldsAlternativeDistributionKeys = null)



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
    public class AlternativeDistributionKeysGetInstanceExample
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
            var apiInstance = new AlternativeDistributionKeysApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionKeys = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionKeys (optional) 

            try
            {
                AlternativeDistributionKeyResponse result = apiInstance.AlternativeDistributionKeysGetInstance(id, fieldsAlternativeDistributionKeys);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionKeysGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionKeyResponse> response = apiInstance.AlternativeDistributionKeysGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionKeys);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionKeysApi.AlternativeDistributionKeysGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionKeys** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionKeys | [optional]  |

### Return type

[**AlternativeDistributionKeyResponse**](AlternativeDistributionKeyResponse.md)

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
| **200** | Single AlternativeDistributionKey |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

