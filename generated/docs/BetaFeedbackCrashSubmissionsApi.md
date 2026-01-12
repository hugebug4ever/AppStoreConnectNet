# AppStoreConnect.Net.Api.BetaFeedbackCrashSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionscrashloggettoonerelated) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/crashLog |  |
| [**BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionscrashloggettoonerelationship) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/relationships/crashLog |  |
| [**BetaFeedbackCrashSubmissionsDeleteInstance**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionsdeleteinstance) | **DELETE** /v1/betaFeedbackCrashSubmissions/{id} |  |
| [**BetaFeedbackCrashSubmissionsGetInstance**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionsgetinstance) | **GET** /v1/betaFeedbackCrashSubmissions/{id} |  |

<a id="betafeedbackcrashsubmissionscrashloggettoonerelated"></a>
# **BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated**
> BetaCrashLogResponse BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated (string id, List<string>? fieldsBetaCrashLogs = null)



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
    public class BetaFeedbackCrashSubmissionsCrashLogGetToOneRelatedExample
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
            var apiInstance = new BetaFeedbackCrashSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaCrashLogs = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaCrashLogs (optional) 

            try
            {
                BetaCrashLogResponse result = apiInstance.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated(id, fieldsBetaCrashLogs);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackCrashSubmissionsCrashLogGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaCrashLogResponse> response = apiInstance.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelatedWithHttpInfo(id, fieldsBetaCrashLogs);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaCrashLogs** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaCrashLogs | [optional]  |

### Return type

[**BetaCrashLogResponse**](BetaCrashLogResponse.md)

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
| **200** | Single BetaCrashLog |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betafeedbackcrashsubmissionscrashloggettoonerelationship"></a>
# **BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship**
> BetaFeedbackCrashSubmissionCrashLogLinkageResponse BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship (string id)



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
    public class BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationshipExample
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
            var apiInstance = new BetaFeedbackCrashSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaFeedbackCrashSubmissionCrashLogLinkageResponse result = apiInstance.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaFeedbackCrashSubmissionCrashLogLinkageResponse> response = apiInstance.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaFeedbackCrashSubmissionCrashLogLinkageResponse**](BetaFeedbackCrashSubmissionCrashLogLinkageResponse.md)

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

<a id="betafeedbackcrashsubmissionsdeleteinstance"></a>
# **BetaFeedbackCrashSubmissionsDeleteInstance**
> void BetaFeedbackCrashSubmissionsDeleteInstance (string id)



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
    public class BetaFeedbackCrashSubmissionsDeleteInstanceExample
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
            var apiInstance = new BetaFeedbackCrashSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.BetaFeedbackCrashSubmissionsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackCrashSubmissionsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaFeedbackCrashSubmissionsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="betafeedbackcrashsubmissionsgetinstance"></a>
# **BetaFeedbackCrashSubmissionsGetInstance**
> BetaFeedbackCrashSubmissionResponse BetaFeedbackCrashSubmissionsGetInstance (string id, List<string>? fieldsBetaFeedbackCrashSubmissions = null, List<string>? include = null)



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
    public class BetaFeedbackCrashSubmissionsGetInstanceExample
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
            var apiInstance = new BetaFeedbackCrashSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaFeedbackCrashSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaFeedbackCrashSubmissions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaFeedbackCrashSubmissionResponse result = apiInstance.BetaFeedbackCrashSubmissionsGetInstance(id, fieldsBetaFeedbackCrashSubmissions, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackCrashSubmissionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaFeedbackCrashSubmissionResponse> response = apiInstance.BetaFeedbackCrashSubmissionsGetInstanceWithHttpInfo(id, fieldsBetaFeedbackCrashSubmissions, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackCrashSubmissionsApi.BetaFeedbackCrashSubmissionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaFeedbackCrashSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaFeedbackCrashSubmissions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaFeedbackCrashSubmissionResponse**](BetaFeedbackCrashSubmissionResponse.md)

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
| **200** | Single BetaFeedbackCrashSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

