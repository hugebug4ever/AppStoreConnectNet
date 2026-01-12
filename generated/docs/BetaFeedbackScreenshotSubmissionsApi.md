# AppStoreConnect.Net.Api.BetaFeedbackScreenshotSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaFeedbackScreenshotSubmissionsDeleteInstance**](BetaFeedbackScreenshotSubmissionsApi.md#betafeedbackscreenshotsubmissionsdeleteinstance) | **DELETE** /v1/betaFeedbackScreenshotSubmissions/{id} |  |
| [**BetaFeedbackScreenshotSubmissionsGetInstance**](BetaFeedbackScreenshotSubmissionsApi.md#betafeedbackscreenshotsubmissionsgetinstance) | **GET** /v1/betaFeedbackScreenshotSubmissions/{id} |  |

<a id="betafeedbackscreenshotsubmissionsdeleteinstance"></a>
# **BetaFeedbackScreenshotSubmissionsDeleteInstance**
> void BetaFeedbackScreenshotSubmissionsDeleteInstance (string id)



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
    public class BetaFeedbackScreenshotSubmissionsDeleteInstanceExample
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
            var apiInstance = new BetaFeedbackScreenshotSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.BetaFeedbackScreenshotSubmissionsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackScreenshotSubmissionsApi.BetaFeedbackScreenshotSubmissionsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackScreenshotSubmissionsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaFeedbackScreenshotSubmissionsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackScreenshotSubmissionsApi.BetaFeedbackScreenshotSubmissionsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="betafeedbackscreenshotsubmissionsgetinstance"></a>
# **BetaFeedbackScreenshotSubmissionsGetInstance**
> BetaFeedbackScreenshotSubmissionResponse BetaFeedbackScreenshotSubmissionsGetInstance (string id, List<string>? fieldsBetaFeedbackScreenshotSubmissions = null, List<string>? include = null)



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
    public class BetaFeedbackScreenshotSubmissionsGetInstanceExample
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
            var apiInstance = new BetaFeedbackScreenshotSubmissionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaFeedbackScreenshotSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaFeedbackScreenshotSubmissions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaFeedbackScreenshotSubmissionResponse result = apiInstance.BetaFeedbackScreenshotSubmissionsGetInstance(id, fieldsBetaFeedbackScreenshotSubmissions, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaFeedbackScreenshotSubmissionsApi.BetaFeedbackScreenshotSubmissionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaFeedbackScreenshotSubmissionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaFeedbackScreenshotSubmissionResponse> response = apiInstance.BetaFeedbackScreenshotSubmissionsGetInstanceWithHttpInfo(id, fieldsBetaFeedbackScreenshotSubmissions, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaFeedbackScreenshotSubmissionsApi.BetaFeedbackScreenshotSubmissionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaFeedbackScreenshotSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaFeedbackScreenshotSubmissions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaFeedbackScreenshotSubmissionResponse**](BetaFeedbackScreenshotSubmissionResponse.md)

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
| **200** | Single BetaFeedbackScreenshotSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

