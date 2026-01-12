# AppStoreConnect.Net.Api.AlternativeDistributionPackageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackageVersionsDeltasGetToManyRelated**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsdeltasgettomanyrelated) | **GET** /v1/alternativeDistributionPackageVersions/{id}/deltas |  |
| [**AlternativeDistributionPackageVersionsDeltasGetToManyRelationship**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsdeltasgettomanyrelationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/deltas |  |
| [**AlternativeDistributionPackageVersionsGetInstance**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsgetinstance) | **GET** /v1/alternativeDistributionPackageVersions/{id} |  |
| [**AlternativeDistributionPackageVersionsVariantsGetToManyRelated**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsvariantsgettomanyrelated) | **GET** /v1/alternativeDistributionPackageVersions/{id}/variants |  |
| [**AlternativeDistributionPackageVersionsVariantsGetToManyRelationship**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsvariantsgettomanyrelationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/variants |  |

<a id="alternativedistributionpackageversionsdeltasgettomanyrelated"></a>
# **AlternativeDistributionPackageVersionsDeltasGetToManyRelated**
> AlternativeDistributionPackageDeltasResponse AlternativeDistributionPackageVersionsDeltasGetToManyRelated (string id, List<string>? fieldsAlternativeDistributionPackageDeltas = null, int? limit = null)



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
    public class AlternativeDistributionPackageVersionsDeltasGetToManyRelatedExample
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
            var apiInstance = new AlternativeDistributionPackageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackageDeltas = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionPackageDeltasResponse result = apiInstance.AlternativeDistributionPackageVersionsDeltasGetToManyRelated(id, fieldsAlternativeDistributionPackageDeltas, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsDeltasGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVersionsDeltasGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageDeltasResponse> response = apiInstance.AlternativeDistributionPackageVersionsDeltasGetToManyRelatedWithHttpInfo(id, fieldsAlternativeDistributionPackageDeltas, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsDeltasGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageDeltasResponse**](AlternativeDistributionPackageDeltasResponse.md)

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
| **200** | List of AlternativeDistributionPackageDeltas |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackageversionsdeltasgettomanyrelationship"></a>
# **AlternativeDistributionPackageVersionsDeltasGetToManyRelationship**
> AlternativeDistributionPackageVersionDeltasLinkagesResponse AlternativeDistributionPackageVersionsDeltasGetToManyRelationship (string id, int? limit = null)



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
    public class AlternativeDistributionPackageVersionsDeltasGetToManyRelationshipExample
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
            var apiInstance = new AlternativeDistributionPackageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionPackageVersionDeltasLinkagesResponse result = apiInstance.AlternativeDistributionPackageVersionsDeltasGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsDeltasGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVersionsDeltasGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVersionDeltasLinkagesResponse> response = apiInstance.AlternativeDistributionPackageVersionsDeltasGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsDeltasGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AlternativeDistributionPackageVersionDeltasLinkagesResponse**](AlternativeDistributionPackageVersionDeltasLinkagesResponse.md)

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

<a id="alternativedistributionpackageversionsgetinstance"></a>
# **AlternativeDistributionPackageVersionsGetInstance**
> AlternativeDistributionPackageVersionResponse AlternativeDistributionPackageVersionsGetInstance (string id, List<string>? fieldsAlternativeDistributionPackageVersions = null, List<string>? fieldsAlternativeDistributionPackageVariants = null, List<string>? fieldsAlternativeDistributionPackageDeltas = null, List<string>? include = null, int? limitDeltas = null, int? limitVariants = null)



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
    public class AlternativeDistributionPackageVersionsGetInstanceExample
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
            var apiInstance = new AlternativeDistributionPackageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackageVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional) 
            var fieldsAlternativeDistributionPackageVariants = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional) 
            var fieldsAlternativeDistributionPackageDeltas = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitDeltas = 56;  // int? | maximum number of related deltas returned (when they are included) (optional) 
            var limitVariants = 56;  // int? | maximum number of related variants returned (when they are included) (optional) 

            try
            {
                AlternativeDistributionPackageVersionResponse result = apiInstance.AlternativeDistributionPackageVersionsGetInstance(id, fieldsAlternativeDistributionPackageVersions, fieldsAlternativeDistributionPackageVariants, fieldsAlternativeDistributionPackageDeltas, include, limitDeltas, limitVariants);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVersionResponse> response = apiInstance.AlternativeDistributionPackageVersionsGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionPackageVersions, fieldsAlternativeDistributionPackageVariants, fieldsAlternativeDistributionPackageDeltas, include, limitDeltas, limitVariants);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitDeltas** | **int?** | maximum number of related deltas returned (when they are included) | [optional]  |
| **limitVariants** | **int?** | maximum number of related variants returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionResponse**](AlternativeDistributionPackageVersionResponse.md)

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
| **200** | Single AlternativeDistributionPackageVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackageversionsvariantsgettomanyrelated"></a>
# **AlternativeDistributionPackageVersionsVariantsGetToManyRelated**
> AlternativeDistributionPackageVariantsResponse AlternativeDistributionPackageVersionsVariantsGetToManyRelated (string id, List<string>? fieldsAlternativeDistributionPackageVariants = null, int? limit = null)



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
    public class AlternativeDistributionPackageVersionsVariantsGetToManyRelatedExample
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
            var apiInstance = new AlternativeDistributionPackageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackageVariants = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionPackageVariantsResponse result = apiInstance.AlternativeDistributionPackageVersionsVariantsGetToManyRelated(id, fieldsAlternativeDistributionPackageVariants, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsVariantsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVersionsVariantsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVariantsResponse> response = apiInstance.AlternativeDistributionPackageVersionsVariantsGetToManyRelatedWithHttpInfo(id, fieldsAlternativeDistributionPackageVariants, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsVariantsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageVariantsResponse**](AlternativeDistributionPackageVariantsResponse.md)

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
| **200** | List of AlternativeDistributionPackageVariants |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="alternativedistributionpackageversionsvariantsgettomanyrelationship"></a>
# **AlternativeDistributionPackageVersionsVariantsGetToManyRelationship**
> AlternativeDistributionPackageVersionVariantsLinkagesResponse AlternativeDistributionPackageVersionsVariantsGetToManyRelationship (string id, int? limit = null)



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
    public class AlternativeDistributionPackageVersionsVariantsGetToManyRelationshipExample
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
            var apiInstance = new AlternativeDistributionPackageVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AlternativeDistributionPackageVersionVariantsLinkagesResponse result = apiInstance.AlternativeDistributionPackageVersionsVariantsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsVariantsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVersionsVariantsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVersionVariantsLinkagesResponse> response = apiInstance.AlternativeDistributionPackageVersionsVariantsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVersionsApi.AlternativeDistributionPackageVersionsVariantsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AlternativeDistributionPackageVersionVariantsLinkagesResponse**](AlternativeDistributionPackageVersionVariantsLinkagesResponse.md)

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

