# AppStoreConnect.Net.Api.AccessibilityDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AccessibilityDeclarationsCreateInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationscreateinstance) | **POST** /v1/accessibilityDeclarations |  |
| [**AccessibilityDeclarationsDeleteInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsdeleteinstance) | **DELETE** /v1/accessibilityDeclarations/{id} |  |
| [**AccessibilityDeclarationsGetInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsgetinstance) | **GET** /v1/accessibilityDeclarations/{id} |  |
| [**AccessibilityDeclarationsUpdateInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsupdateinstance) | **PATCH** /v1/accessibilityDeclarations/{id} |  |

<a id="accessibilitydeclarationscreateinstance"></a>
# **AccessibilityDeclarationsCreateInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsCreateInstance (AccessibilityDeclarationCreateRequest accessibilityDeclarationCreateRequest)



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
    public class AccessibilityDeclarationsCreateInstanceExample
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
            var apiInstance = new AccessibilityDeclarationsApi(httpClient, config, httpClientHandler);
            var accessibilityDeclarationCreateRequest = new AccessibilityDeclarationCreateRequest(); // AccessibilityDeclarationCreateRequest | AccessibilityDeclaration representation

            try
            {
                AccessibilityDeclarationResponse result = apiInstance.AccessibilityDeclarationsCreateInstance(accessibilityDeclarationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AccessibilityDeclarationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AccessibilityDeclarationResponse> response = apiInstance.AccessibilityDeclarationsCreateInstanceWithHttpInfo(accessibilityDeclarationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **accessibilityDeclarationCreateRequest** | [**AccessibilityDeclarationCreateRequest**](AccessibilityDeclarationCreateRequest.md) | AccessibilityDeclaration representation |  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **201** | Single AccessibilityDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="accessibilitydeclarationsdeleteinstance"></a>
# **AccessibilityDeclarationsDeleteInstance**
> void AccessibilityDeclarationsDeleteInstance (string id)



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
    public class AccessibilityDeclarationsDeleteInstanceExample
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
            var apiInstance = new AccessibilityDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AccessibilityDeclarationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AccessibilityDeclarationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AccessibilityDeclarationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="accessibilitydeclarationsgetinstance"></a>
# **AccessibilityDeclarationsGetInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsGetInstance (string id, List<string>? fieldsAccessibilityDeclarations = null)



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
    public class AccessibilityDeclarationsGetInstanceExample
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
            var apiInstance = new AccessibilityDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAccessibilityDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type accessibilityDeclarations (optional) 

            try
            {
                AccessibilityDeclarationResponse result = apiInstance.AccessibilityDeclarationsGetInstance(id, fieldsAccessibilityDeclarations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AccessibilityDeclarationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AccessibilityDeclarationResponse> response = apiInstance.AccessibilityDeclarationsGetInstanceWithHttpInfo(id, fieldsAccessibilityDeclarations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAccessibilityDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type accessibilityDeclarations | [optional]  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **200** | Single AccessibilityDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="accessibilitydeclarationsupdateinstance"></a>
# **AccessibilityDeclarationsUpdateInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsUpdateInstance (string id, AccessibilityDeclarationUpdateRequest accessibilityDeclarationUpdateRequest)



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
    public class AccessibilityDeclarationsUpdateInstanceExample
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
            var apiInstance = new AccessibilityDeclarationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var accessibilityDeclarationUpdateRequest = new AccessibilityDeclarationUpdateRequest(); // AccessibilityDeclarationUpdateRequest | AccessibilityDeclaration representation

            try
            {
                AccessibilityDeclarationResponse result = apiInstance.AccessibilityDeclarationsUpdateInstance(id, accessibilityDeclarationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AccessibilityDeclarationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AccessibilityDeclarationResponse> response = apiInstance.AccessibilityDeclarationsUpdateInstanceWithHttpInfo(id, accessibilityDeclarationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AccessibilityDeclarationsApi.AccessibilityDeclarationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **accessibilityDeclarationUpdateRequest** | [**AccessibilityDeclarationUpdateRequest**](AccessibilityDeclarationUpdateRequest.md) | AccessibilityDeclaration representation |  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **200** | Single AccessibilityDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

