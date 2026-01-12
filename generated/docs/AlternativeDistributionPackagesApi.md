# AppStoreConnect.Net.Api.AlternativeDistributionPackagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackagesCreateInstance**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagescreateinstance) | **POST** /v1/alternativeDistributionPackages |  |
| [**AlternativeDistributionPackagesGetInstance**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesgetinstance) | **GET** /v1/alternativeDistributionPackages/{id} |  |
| [**AlternativeDistributionPackagesVersionsGetToManyRelated**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesversionsgettomanyrelated) | **GET** /v1/alternativeDistributionPackages/{id}/versions |  |
| [**AlternativeDistributionPackagesVersionsGetToManyRelationship**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesversionsgettomanyrelationship) | **GET** /v1/alternativeDistributionPackages/{id}/relationships/versions |  |

<a id="alternativedistributionpackagescreateinstance"></a>
# **AlternativeDistributionPackagesCreateInstance**
> AlternativeDistributionPackageResponse AlternativeDistributionPackagesCreateInstance (AlternativeDistributionPackageCreateRequest alternativeDistributionPackageCreateRequest)



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
    public class AlternativeDistributionPackagesCreateInstanceExample
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
            var apiInstance = new AlternativeDistributionPackagesApi(httpClient, config, httpClientHandler);
            var alternativeDistributionPackageCreateRequest = new AlternativeDistributionPackageCreateRequest(); // AlternativeDistributionPackageCreateRequest | AlternativeDistributionPackage representation

            try
            {
                AlternativeDistributionPackageResponse result = apiInstance.AlternativeDistributionPackagesCreateInstance(alternativeDistributionPackageCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackagesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageResponse> response = apiInstance.AlternativeDistributionPackagesCreateInstanceWithHttpInfo(alternativeDistributionPackageCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionPackageCreateRequest** | [**AlternativeDistributionPackageCreateRequest**](AlternativeDistributionPackageCreateRequest.md) | AlternativeDistributionPackage representation |  |

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

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
| **201** | Single AlternativeDistributionPackage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackagesgetinstance"></a>
# **AlternativeDistributionPackagesGetInstance**
> AlternativeDistributionPackageResponse AlternativeDistributionPackagesGetInstance (string id, List<string>? fieldsAlternativeDistributionPackages = null, List<string>? fieldsAlternativeDistributionPackageVersions = null, List<string>? include = null, int? limitVersions = null)



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
    public class AlternativeDistributionPackagesGetInstanceExample
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
            var apiInstance = new AlternativeDistributionPackagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackages = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackages (optional) 
            var fieldsAlternativeDistributionPackageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                AlternativeDistributionPackageResponse result = apiInstance.AlternativeDistributionPackagesGetInstance(id, fieldsAlternativeDistributionPackages, fieldsAlternativeDistributionPackageVersions, include, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackagesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageResponse> response = apiInstance.AlternativeDistributionPackagesGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionPackages, fieldsAlternativeDistributionPackageVersions, include, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

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
| **200** | Single AlternativeDistributionPackage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackagesversionsgettomanyrelated"></a>
# **AlternativeDistributionPackagesVersionsGetToManyRelated**
> AlternativeDistributionPackageVersionsResponse AlternativeDistributionPackagesVersionsGetToManyRelated (string id, List<string>? filterState = null, List<string>? fieldsAlternativeDistributionPackageVersions = null, List<string>? fieldsAlternativeDistributionPackageVariants = null, List<string>? fieldsAlternativeDistributionPackageDeltas = null, List<string>? fieldsAlternativeDistributionPackages = null, int? limit = null, List<string>? include = null, int? limitVariants = null, int? limitDeltas = null)



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
    public class AlternativeDistributionPackagesVersionsGetToManyRelatedExample
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
            var apiInstance = new AlternativeDistributionPackagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterState = new List<string>?(); // List<string>? | filter by attribute 'state' (optional) 
            var fieldsAlternativeDistributionPackageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional) 
            var fieldsAlternativeDistributionPackageVariants = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional) 
            var fieldsAlternativeDistributionPackageDeltas = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional) 
            var fieldsAlternativeDistributionPackages = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVariants = 56;  // int? | maximum number of related variants returned (when they are included) (optional) 
            var limitDeltas = 56;  // int? | maximum number of related deltas returned (when they are included) (optional) 

            try
            {
                AlternativeDistributionPackageVersionsResponse result = apiInstance.AlternativeDistributionPackagesVersionsGetToManyRelated(id, filterState, fieldsAlternativeDistributionPackageVersions, fieldsAlternativeDistributionPackageVariants, fieldsAlternativeDistributionPackageDeltas, fieldsAlternativeDistributionPackages, limit, include, limitVariants, limitDeltas);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackagesVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVersionsResponse> response = apiInstance.AlternativeDistributionPackagesVersionsGetToManyRelatedWithHttpInfo(id, filterState, fieldsAlternativeDistributionPackageVersions, fieldsAlternativeDistributionPackageVariants, fieldsAlternativeDistributionPackageDeltas, fieldsAlternativeDistributionPackages, limit, include, limitVariants, limitDeltas);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVariants** | **int?** | maximum number of related variants returned (when they are included) | [optional]  |
| **limitDeltas** | **int?** | maximum number of related deltas returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionsResponse**](AlternativeDistributionPackageVersionsResponse.md)

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
| **200** | List of AlternativeDistributionPackageVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackagesversionsgettomanyrelationship"></a>
# **AlternativeDistributionPackagesVersionsGetToManyRelationship**
> AlternativeDistributionPackageVersionsLinkagesResponse AlternativeDistributionPackagesVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class AlternativeDistributionPackagesVersionsGetToManyRelationshipExample
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
            var apiInstance = new AlternativeDistributionPackagesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionPackageVersionsLinkagesResponse result = apiInstance.AlternativeDistributionPackagesVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackagesVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVersionsLinkagesResponse> response = apiInstance.AlternativeDistributionPackagesVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackagesApi.AlternativeDistributionPackagesVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AlternativeDistributionPackageVersionsLinkagesResponse**](AlternativeDistributionPackageVersionsLinkagesResponse.md)

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

