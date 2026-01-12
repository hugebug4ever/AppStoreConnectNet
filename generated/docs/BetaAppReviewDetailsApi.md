# AppStoreConnect.Net.Api.BetaAppReviewDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaAppReviewDetailsAppGetToOneRelated**](BetaAppReviewDetailsApi.md#betaappreviewdetailsappgettoonerelated) | **GET** /v1/betaAppReviewDetails/{id}/app |  |
| [**BetaAppReviewDetailsAppGetToOneRelationship**](BetaAppReviewDetailsApi.md#betaappreviewdetailsappgettoonerelationship) | **GET** /v1/betaAppReviewDetails/{id}/relationships/app |  |
| [**BetaAppReviewDetailsGetCollection**](BetaAppReviewDetailsApi.md#betaappreviewdetailsgetcollection) | **GET** /v1/betaAppReviewDetails |  |
| [**BetaAppReviewDetailsGetInstance**](BetaAppReviewDetailsApi.md#betaappreviewdetailsgetinstance) | **GET** /v1/betaAppReviewDetails/{id} |  |
| [**BetaAppReviewDetailsUpdateInstance**](BetaAppReviewDetailsApi.md#betaappreviewdetailsupdateinstance) | **PATCH** /v1/betaAppReviewDetails/{id} |  |

<a id="betaappreviewdetailsappgettoonerelated"></a>
# **BetaAppReviewDetailsAppGetToOneRelated**
> AppWithoutIncludesResponse BetaAppReviewDetailsAppGetToOneRelated (string id, List<string>? fieldsApps = null)



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
    public class BetaAppReviewDetailsAppGetToOneRelatedExample
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
            var apiInstance = new BetaAppReviewDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 

            try
            {
                AppWithoutIncludesResponse result = apiInstance.BetaAppReviewDetailsAppGetToOneRelated(id, fieldsApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewDetailsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppWithoutIncludesResponse> response = apiInstance.BetaAppReviewDetailsAppGetToOneRelatedWithHttpInfo(id, fieldsApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsAppGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewdetailsappgettoonerelationship"></a>
# **BetaAppReviewDetailsAppGetToOneRelationship**
> BetaAppReviewDetailAppLinkageResponse BetaAppReviewDetailsAppGetToOneRelationship (string id)



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
    public class BetaAppReviewDetailsAppGetToOneRelationshipExample
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
            var apiInstance = new BetaAppReviewDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaAppReviewDetailAppLinkageResponse result = apiInstance.BetaAppReviewDetailsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewDetailsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewDetailAppLinkageResponse> response = apiInstance.BetaAppReviewDetailsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaAppReviewDetailAppLinkageResponse**](BetaAppReviewDetailAppLinkageResponse.md)

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
| **200** | Related linkage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewdetailsgetcollection"></a>
# **BetaAppReviewDetailsGetCollection**
> BetaAppReviewDetailsResponse BetaAppReviewDetailsGetCollection (List<string> filterApp, List<string>? fieldsBetaAppReviewDetails = null, List<string>? fieldsApps = null, int? limit = null, List<string>? include = null)



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
    public class BetaAppReviewDetailsGetCollectionExample
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
            var apiInstance = new BetaAppReviewDetailsApi(httpClient, config, httpClientHandler);
            var filterApp = new List<string>(); // List<string> | filter by id(s) of related 'app'
            var fieldsBetaAppReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewDetails (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaAppReviewDetailsResponse result = apiInstance.BetaAppReviewDetailsGetCollection(filterApp, fieldsBetaAppReviewDetails, fieldsApps, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewDetailsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewDetailsResponse> response = apiInstance.BetaAppReviewDetailsGetCollectionWithHttpInfo(filterApp, fieldsBetaAppReviewDetails, fieldsApps, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; |  |
| **fieldsBetaAppReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewDetails | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewDetailsResponse**](BetaAppReviewDetailsResponse.md)

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
| **200** | List of BetaAppReviewDetails |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewdetailsgetinstance"></a>
# **BetaAppReviewDetailsGetInstance**
> BetaAppReviewDetailResponse BetaAppReviewDetailsGetInstance (string id, List<string>? fieldsBetaAppReviewDetails = null, List<string>? fieldsApps = null, List<string>? include = null)



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
    public class BetaAppReviewDetailsGetInstanceExample
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
            var apiInstance = new BetaAppReviewDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaAppReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewDetails (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaAppReviewDetailResponse result = apiInstance.BetaAppReviewDetailsGetInstance(id, fieldsBetaAppReviewDetails, fieldsApps, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewDetailsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewDetailResponse> response = apiInstance.BetaAppReviewDetailsGetInstanceWithHttpInfo(id, fieldsBetaAppReviewDetails, fieldsApps, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewDetails | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewDetailResponse**](BetaAppReviewDetailResponse.md)

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
| **200** | Single BetaAppReviewDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewdetailsupdateinstance"></a>
# **BetaAppReviewDetailsUpdateInstance**
> BetaAppReviewDetailResponse BetaAppReviewDetailsUpdateInstance (string id, BetaAppReviewDetailUpdateRequest betaAppReviewDetailUpdateRequest)



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
    public class BetaAppReviewDetailsUpdateInstanceExample
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
            var apiInstance = new BetaAppReviewDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaAppReviewDetailUpdateRequest = new BetaAppReviewDetailUpdateRequest(); // BetaAppReviewDetailUpdateRequest | BetaAppReviewDetail representation

            try
            {
                BetaAppReviewDetailResponse result = apiInstance.BetaAppReviewDetailsUpdateInstance(id, betaAppReviewDetailUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewDetailsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewDetailResponse> response = apiInstance.BetaAppReviewDetailsUpdateInstanceWithHttpInfo(id, betaAppReviewDetailUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewDetailsApi.BetaAppReviewDetailsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaAppReviewDetailUpdateRequest** | [**BetaAppReviewDetailUpdateRequest**](BetaAppReviewDetailUpdateRequest.md) | BetaAppReviewDetail representation |  |

### Return type

[**BetaAppReviewDetailResponse**](BetaAppReviewDetailResponse.md)

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
| **200** | Single BetaAppReviewDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

