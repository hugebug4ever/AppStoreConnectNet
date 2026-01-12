# AppStoreConnect.Net.Api.BetaAppReviewSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaAppReviewSubmissionsBuildGetToOneRelated**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsbuildgettoonerelated) | **GET** /v1/betaAppReviewSubmissions/{id}/build |  |
| [**BetaAppReviewSubmissionsBuildGetToOneRelationship**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsbuildgettoonerelationship) | **GET** /v1/betaAppReviewSubmissions/{id}/relationships/build |  |
| [**BetaAppReviewSubmissionsCreateInstance**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionscreateinstance) | **POST** /v1/betaAppReviewSubmissions |  |
| [**BetaAppReviewSubmissionsGetCollection**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsgetcollection) | **GET** /v1/betaAppReviewSubmissions |  |
| [**BetaAppReviewSubmissionsGetInstance**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsgetinstance) | **GET** /v1/betaAppReviewSubmissions/{id} |  |

<a id="betaappreviewsubmissionsbuildgettoonerelated"></a>
# **BetaAppReviewSubmissionsBuildGetToOneRelated**
> BuildWithoutIncludesResponse BetaAppReviewSubmissionsBuildGetToOneRelated (string id, List<string>? fieldsBuilds = null)



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
    public class BetaAppReviewSubmissionsBuildGetToOneRelatedExample
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
            var apiInstance = new BetaAppReviewSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 

            try
            {
                BuildWithoutIncludesResponse result = apiInstance.BetaAppReviewSubmissionsBuildGetToOneRelated(id, fieldsBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsBuildGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewSubmissionsBuildGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildWithoutIncludesResponse> response = apiInstance.BetaAppReviewSubmissionsBuildGetToOneRelatedWithHttpInfo(id, fieldsBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsBuildGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |

### Return type

[**BuildWithoutIncludesResponse**](BuildWithoutIncludesResponse.md)

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
| **200** | Single Build with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewsubmissionsbuildgettoonerelationship"></a>
# **BetaAppReviewSubmissionsBuildGetToOneRelationship**
> BetaAppReviewSubmissionBuildLinkageResponse BetaAppReviewSubmissionsBuildGetToOneRelationship (string id)



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
    public class BetaAppReviewSubmissionsBuildGetToOneRelationshipExample
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
            var apiInstance = new BetaAppReviewSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaAppReviewSubmissionBuildLinkageResponse result = apiInstance.BetaAppReviewSubmissionsBuildGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsBuildGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewSubmissionsBuildGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewSubmissionBuildLinkageResponse> response = apiInstance.BetaAppReviewSubmissionsBuildGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsBuildGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaAppReviewSubmissionBuildLinkageResponse**](BetaAppReviewSubmissionBuildLinkageResponse.md)

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

<a id="betaappreviewsubmissionscreateinstance"></a>
# **BetaAppReviewSubmissionsCreateInstance**
> BetaAppReviewSubmissionResponse BetaAppReviewSubmissionsCreateInstance (BetaAppReviewSubmissionCreateRequest betaAppReviewSubmissionCreateRequest)



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
    public class BetaAppReviewSubmissionsCreateInstanceExample
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
            var apiInstance = new BetaAppReviewSubmissionsApi(httpClient, config, httpClientHandler);
            var betaAppReviewSubmissionCreateRequest = new BetaAppReviewSubmissionCreateRequest(); // BetaAppReviewSubmissionCreateRequest | BetaAppReviewSubmission representation

            try
            {
                BetaAppReviewSubmissionResponse result = apiInstance.BetaAppReviewSubmissionsCreateInstance(betaAppReviewSubmissionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewSubmissionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewSubmissionResponse> response = apiInstance.BetaAppReviewSubmissionsCreateInstanceWithHttpInfo(betaAppReviewSubmissionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaAppReviewSubmissionCreateRequest** | [**BetaAppReviewSubmissionCreateRequest**](BetaAppReviewSubmissionCreateRequest.md) | BetaAppReviewSubmission representation |  |

### Return type

[**BetaAppReviewSubmissionResponse**](BetaAppReviewSubmissionResponse.md)

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
| **201** | Single BetaAppReviewSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewsubmissionsgetcollection"></a>
# **BetaAppReviewSubmissionsGetCollection**
> BetaAppReviewSubmissionsResponse BetaAppReviewSubmissionsGetCollection (List<string> filterBuild, List<string>? filterBetaReviewState = null, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsBuilds = null, int? limit = null, List<string>? include = null)



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
    public class BetaAppReviewSubmissionsGetCollectionExample
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
            var apiInstance = new BetaAppReviewSubmissionsApi(httpClient, config, httpClientHandler);
            var filterBuild = new List<string>(); // List<string> | filter by id(s) of related 'build'
            var filterBetaReviewState = new List<string>?(); // List<string>? | filter by attribute 'betaReviewState' (optional) 
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaAppReviewSubmissionsResponse result = apiInstance.BetaAppReviewSubmissionsGetCollection(filterBuild, filterBetaReviewState, fieldsBetaAppReviewSubmissions, fieldsBuilds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewSubmissionsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewSubmissionsResponse> response = apiInstance.BetaAppReviewSubmissionsGetCollectionWithHttpInfo(filterBuild, filterBetaReviewState, fieldsBetaAppReviewSubmissions, fieldsBuilds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuild** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;build&#39; |  |
| **filterBetaReviewState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;betaReviewState&#39; | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewSubmissionsResponse**](BetaAppReviewSubmissionsResponse.md)

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
| **200** | List of BetaAppReviewSubmissions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betaappreviewsubmissionsgetinstance"></a>
# **BetaAppReviewSubmissionsGetInstance**
> BetaAppReviewSubmissionResponse BetaAppReviewSubmissionsGetInstance (string id, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsBuilds = null, List<string>? include = null)



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
    public class BetaAppReviewSubmissionsGetInstanceExample
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
            var apiInstance = new BetaAppReviewSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaAppReviewSubmissionResponse result = apiInstance.BetaAppReviewSubmissionsGetInstance(id, fieldsBetaAppReviewSubmissions, fieldsBuilds, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaAppReviewSubmissionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewSubmissionResponse> response = apiInstance.BetaAppReviewSubmissionsGetInstanceWithHttpInfo(id, fieldsBetaAppReviewSubmissions, fieldsBuilds, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaAppReviewSubmissionsApi.BetaAppReviewSubmissionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewSubmissionResponse**](BetaAppReviewSubmissionResponse.md)

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
| **200** | Single BetaAppReviewSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

