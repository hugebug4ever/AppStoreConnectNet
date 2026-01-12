# AppStoreConnect.Net.Api.BetaRecruitmentCriteriaApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaRecruitmentCriteriaCreateInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriacreateinstance) | **POST** /v1/betaRecruitmentCriteria |  |
| [**BetaRecruitmentCriteriaDeleteInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriadeleteinstance) | **DELETE** /v1/betaRecruitmentCriteria/{id} |  |
| [**BetaRecruitmentCriteriaUpdateInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriaupdateinstance) | **PATCH** /v1/betaRecruitmentCriteria/{id} |  |

<a id="betarecruitmentcriteriacreateinstance"></a>
# **BetaRecruitmentCriteriaCreateInstance**
> BetaRecruitmentCriterionResponse BetaRecruitmentCriteriaCreateInstance (BetaRecruitmentCriterionCreateRequest betaRecruitmentCriterionCreateRequest)



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
    public class BetaRecruitmentCriteriaCreateInstanceExample
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
            var apiInstance = new BetaRecruitmentCriteriaApi(httpClient, config, httpClientHandler);
            var betaRecruitmentCriterionCreateRequest = new BetaRecruitmentCriterionCreateRequest(); // BetaRecruitmentCriterionCreateRequest | BetaRecruitmentCriterion representation

            try
            {
                BetaRecruitmentCriterionResponse result = apiInstance.BetaRecruitmentCriteriaCreateInstance(betaRecruitmentCriterionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaRecruitmentCriteriaCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaRecruitmentCriterionResponse> response = apiInstance.BetaRecruitmentCriteriaCreateInstanceWithHttpInfo(betaRecruitmentCriterionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaRecruitmentCriterionCreateRequest** | [**BetaRecruitmentCriterionCreateRequest**](BetaRecruitmentCriterionCreateRequest.md) | BetaRecruitmentCriterion representation |  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **201** | Single BetaRecruitmentCriterion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betarecruitmentcriteriadeleteinstance"></a>
# **BetaRecruitmentCriteriaDeleteInstance**
> void BetaRecruitmentCriteriaDeleteInstance (string id)



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
    public class BetaRecruitmentCriteriaDeleteInstanceExample
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
            var apiInstance = new BetaRecruitmentCriteriaApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.BetaRecruitmentCriteriaDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaRecruitmentCriteriaDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaRecruitmentCriteriaDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="betarecruitmentcriteriaupdateinstance"></a>
# **BetaRecruitmentCriteriaUpdateInstance**
> BetaRecruitmentCriterionResponse BetaRecruitmentCriteriaUpdateInstance (string id, BetaRecruitmentCriterionUpdateRequest betaRecruitmentCriterionUpdateRequest)



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
    public class BetaRecruitmentCriteriaUpdateInstanceExample
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
            var apiInstance = new BetaRecruitmentCriteriaApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaRecruitmentCriterionUpdateRequest = new BetaRecruitmentCriterionUpdateRequest(); // BetaRecruitmentCriterionUpdateRequest | BetaRecruitmentCriterion representation

            try
            {
                BetaRecruitmentCriterionResponse result = apiInstance.BetaRecruitmentCriteriaUpdateInstance(id, betaRecruitmentCriterionUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaRecruitmentCriteriaUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaRecruitmentCriterionResponse> response = apiInstance.BetaRecruitmentCriteriaUpdateInstanceWithHttpInfo(id, betaRecruitmentCriterionUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaRecruitmentCriteriaApi.BetaRecruitmentCriteriaUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaRecruitmentCriterionUpdateRequest** | [**BetaRecruitmentCriterionUpdateRequest**](BetaRecruitmentCriterionUpdateRequest.md) | BetaRecruitmentCriterion representation |  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **200** | Single BetaRecruitmentCriterion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

