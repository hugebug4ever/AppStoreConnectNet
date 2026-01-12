# AppStoreConnect.Net.Api.CiMacOsVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiMacOsVersionsGetCollection**](CiMacOsVersionsApi.md#cimacosversionsgetcollection) | **GET** /v1/ciMacOsVersions |  |
| [**CiMacOsVersionsGetInstance**](CiMacOsVersionsApi.md#cimacosversionsgetinstance) | **GET** /v1/ciMacOsVersions/{id} |  |
| [**CiMacOsVersionsXcodeVersionsGetToManyRelated**](CiMacOsVersionsApi.md#cimacosversionsxcodeversionsgettomanyrelated) | **GET** /v1/ciMacOsVersions/{id}/xcodeVersions |  |
| [**CiMacOsVersionsXcodeVersionsGetToManyRelationship**](CiMacOsVersionsApi.md#cimacosversionsxcodeversionsgettomanyrelationship) | **GET** /v1/ciMacOsVersions/{id}/relationships/xcodeVersions |  |

<a id="cimacosversionsgetcollection"></a>
# **CiMacOsVersionsGetCollection**
> CiMacOsVersionsResponse CiMacOsVersionsGetCollection (List<string>? fieldsCiMacOsVersions = null, List<string>? fieldsCiXcodeVersions = null, int? limit = null, List<string>? include = null, int? limitXcodeVersions = null)



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
    public class CiMacOsVersionsGetCollectionExample
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
            var apiInstance = new CiMacOsVersionsApi(httpClient, config, httpClientHandler);
            var fieldsCiMacOsVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciMacOsVersions (optional) 
            var fieldsCiXcodeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciXcodeVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitXcodeVersions = 56;  // int? | maximum number of related xcodeVersions returned (when they are included) (optional) 

            try
            {
                CiMacOsVersionsResponse result = apiInstance.CiMacOsVersionsGetCollection(fieldsCiMacOsVersions, fieldsCiXcodeVersions, limit, include, limitXcodeVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiMacOsVersionsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiMacOsVersionsResponse> response = apiInstance.CiMacOsVersionsGetCollectionWithHttpInfo(fieldsCiMacOsVersions, fieldsCiXcodeVersions, limit, include, limitXcodeVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitXcodeVersions** | **int?** | maximum number of related xcodeVersions returned (when they are included) | [optional]  |

### Return type

[**CiMacOsVersionsResponse**](CiMacOsVersionsResponse.md)

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
| **200** | List of CiMacOsVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cimacosversionsgetinstance"></a>
# **CiMacOsVersionsGetInstance**
> CiMacOsVersionResponse CiMacOsVersionsGetInstance (string id, List<string>? fieldsCiMacOsVersions = null, List<string>? fieldsCiXcodeVersions = null, List<string>? include = null, int? limitXcodeVersions = null)



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
    public class CiMacOsVersionsGetInstanceExample
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
            var apiInstance = new CiMacOsVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiMacOsVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciMacOsVersions (optional) 
            var fieldsCiXcodeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciXcodeVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitXcodeVersions = 56;  // int? | maximum number of related xcodeVersions returned (when they are included) (optional) 

            try
            {
                CiMacOsVersionResponse result = apiInstance.CiMacOsVersionsGetInstance(id, fieldsCiMacOsVersions, fieldsCiXcodeVersions, include, limitXcodeVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiMacOsVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiMacOsVersionResponse> response = apiInstance.CiMacOsVersionsGetInstanceWithHttpInfo(id, fieldsCiMacOsVersions, fieldsCiXcodeVersions, include, limitXcodeVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitXcodeVersions** | **int?** | maximum number of related xcodeVersions returned (when they are included) | [optional]  |

### Return type

[**CiMacOsVersionResponse**](CiMacOsVersionResponse.md)

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
| **200** | Single CiMacOsVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cimacosversionsxcodeversionsgettomanyrelated"></a>
# **CiMacOsVersionsXcodeVersionsGetToManyRelated**
> CiXcodeVersionsResponse CiMacOsVersionsXcodeVersionsGetToManyRelated (string id, List<string>? fieldsCiXcodeVersions = null, List<string>? fieldsCiMacOsVersions = null, int? limit = null, List<string>? include = null, int? limitMacOsVersions = null)



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
    public class CiMacOsVersionsXcodeVersionsGetToManyRelatedExample
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
            var apiInstance = new CiMacOsVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiXcodeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciXcodeVersions (optional) 
            var fieldsCiMacOsVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciMacOsVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitMacOsVersions = 56;  // int? | maximum number of related macOsVersions returned (when they are included) (optional) 

            try
            {
                CiXcodeVersionsResponse result = apiInstance.CiMacOsVersionsXcodeVersionsGetToManyRelated(id, fieldsCiXcodeVersions, fieldsCiMacOsVersions, limit, include, limitMacOsVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsXcodeVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiMacOsVersionsXcodeVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiXcodeVersionsResponse> response = apiInstance.CiMacOsVersionsXcodeVersionsGetToManyRelatedWithHttpInfo(id, fieldsCiXcodeVersions, fieldsCiMacOsVersions, limit, include, limitMacOsVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsXcodeVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMacOsVersions** | **int?** | maximum number of related macOsVersions returned (when they are included) | [optional]  |

### Return type

[**CiXcodeVersionsResponse**](CiXcodeVersionsResponse.md)

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
| **200** | List of CiXcodeVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cimacosversionsxcodeversionsgettomanyrelationship"></a>
# **CiMacOsVersionsXcodeVersionsGetToManyRelationship**
> CiMacOsVersionXcodeVersionsLinkagesResponse CiMacOsVersionsXcodeVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class CiMacOsVersionsXcodeVersionsGetToManyRelationshipExample
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
            var apiInstance = new CiMacOsVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiMacOsVersionXcodeVersionsLinkagesResponse result = apiInstance.CiMacOsVersionsXcodeVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsXcodeVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiMacOsVersionsXcodeVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiMacOsVersionXcodeVersionsLinkagesResponse> response = apiInstance.CiMacOsVersionsXcodeVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiMacOsVersionsApi.CiMacOsVersionsXcodeVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiMacOsVersionXcodeVersionsLinkagesResponse**](CiMacOsVersionXcodeVersionsLinkagesResponse.md)

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

