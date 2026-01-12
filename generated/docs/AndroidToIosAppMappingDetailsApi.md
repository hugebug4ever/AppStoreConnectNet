# AppStoreConnect.Net.Api.AndroidToIosAppMappingDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AndroidToIosAppMappingDetailsCreateInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailscreateinstance) | **POST** /v1/androidToIosAppMappingDetails |  |
| [**AndroidToIosAppMappingDetailsDeleteInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsdeleteinstance) | **DELETE** /v1/androidToIosAppMappingDetails/{id} |  |
| [**AndroidToIosAppMappingDetailsGetInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsgetinstance) | **GET** /v1/androidToIosAppMappingDetails/{id} |  |
| [**AndroidToIosAppMappingDetailsUpdateInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsupdateinstance) | **PATCH** /v1/androidToIosAppMappingDetails/{id} |  |

<a id="androidtoiosappmappingdetailscreateinstance"></a>
# **AndroidToIosAppMappingDetailsCreateInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsCreateInstance (AndroidToIosAppMappingDetailCreateRequest androidToIosAppMappingDetailCreateRequest)



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
    public class AndroidToIosAppMappingDetailsCreateInstanceExample
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
            var apiInstance = new AndroidToIosAppMappingDetailsApi(httpClient, config, httpClientHandler);
            var androidToIosAppMappingDetailCreateRequest = new AndroidToIosAppMappingDetailCreateRequest(); // AndroidToIosAppMappingDetailCreateRequest | AndroidToIosAppMappingDetail representation

            try
            {
                AndroidToIosAppMappingDetailResponse result = apiInstance.AndroidToIosAppMappingDetailsCreateInstance(androidToIosAppMappingDetailCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AndroidToIosAppMappingDetailsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AndroidToIosAppMappingDetailResponse> response = apiInstance.AndroidToIosAppMappingDetailsCreateInstanceWithHttpInfo(androidToIosAppMappingDetailCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **androidToIosAppMappingDetailCreateRequest** | [**AndroidToIosAppMappingDetailCreateRequest**](AndroidToIosAppMappingDetailCreateRequest.md) | AndroidToIosAppMappingDetail representation |  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **201** | Single AndroidToIosAppMappingDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="androidtoiosappmappingdetailsdeleteinstance"></a>
# **AndroidToIosAppMappingDetailsDeleteInstance**
> void AndroidToIosAppMappingDetailsDeleteInstance (string id)



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
    public class AndroidToIosAppMappingDetailsDeleteInstanceExample
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
            var apiInstance = new AndroidToIosAppMappingDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AndroidToIosAppMappingDetailsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AndroidToIosAppMappingDetailsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AndroidToIosAppMappingDetailsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="androidtoiosappmappingdetailsgetinstance"></a>
# **AndroidToIosAppMappingDetailsGetInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsGetInstance (string id, List<string>? fieldsAndroidToIosAppMappingDetails = null)



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
    public class AndroidToIosAppMappingDetailsGetInstanceExample
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
            var apiInstance = new AndroidToIosAppMappingDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAndroidToIosAppMappingDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type androidToIosAppMappingDetails (optional) 

            try
            {
                AndroidToIosAppMappingDetailResponse result = apiInstance.AndroidToIosAppMappingDetailsGetInstance(id, fieldsAndroidToIosAppMappingDetails);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AndroidToIosAppMappingDetailsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AndroidToIosAppMappingDetailResponse> response = apiInstance.AndroidToIosAppMappingDetailsGetInstanceWithHttpInfo(id, fieldsAndroidToIosAppMappingDetails);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAndroidToIosAppMappingDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type androidToIosAppMappingDetails | [optional]  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **200** | Single AndroidToIosAppMappingDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="androidtoiosappmappingdetailsupdateinstance"></a>
# **AndroidToIosAppMappingDetailsUpdateInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsUpdateInstance (string id, AndroidToIosAppMappingDetailUpdateRequest androidToIosAppMappingDetailUpdateRequest)



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
    public class AndroidToIosAppMappingDetailsUpdateInstanceExample
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
            var apiInstance = new AndroidToIosAppMappingDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var androidToIosAppMappingDetailUpdateRequest = new AndroidToIosAppMappingDetailUpdateRequest(); // AndroidToIosAppMappingDetailUpdateRequest | AndroidToIosAppMappingDetail representation

            try
            {
                AndroidToIosAppMappingDetailResponse result = apiInstance.AndroidToIosAppMappingDetailsUpdateInstance(id, androidToIosAppMappingDetailUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AndroidToIosAppMappingDetailsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AndroidToIosAppMappingDetailResponse> response = apiInstance.AndroidToIosAppMappingDetailsUpdateInstanceWithHttpInfo(id, androidToIosAppMappingDetailUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AndroidToIosAppMappingDetailsApi.AndroidToIosAppMappingDetailsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **androidToIosAppMappingDetailUpdateRequest** | [**AndroidToIosAppMappingDetailUpdateRequest**](AndroidToIosAppMappingDetailUpdateRequest.md) | AndroidToIosAppMappingDetail representation |  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **200** | Single AndroidToIosAppMappingDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

