# AppStoreConnect.Net.Api.BackgroundAssetUploadFilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetUploadFilesCreateInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilescreateinstance) | **POST** /v1/backgroundAssetUploadFiles |  |
| [**BackgroundAssetUploadFilesGetInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilesgetinstance) | **GET** /v1/backgroundAssetUploadFiles/{id} |  |
| [**BackgroundAssetUploadFilesUpdateInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilesupdateinstance) | **PATCH** /v1/backgroundAssetUploadFiles/{id} |  |

<a id="backgroundassetuploadfilescreateinstance"></a>
# **BackgroundAssetUploadFilesCreateInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesCreateInstance (BackgroundAssetUploadFileCreateRequest backgroundAssetUploadFileCreateRequest)



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
    public class BackgroundAssetUploadFilesCreateInstanceExample
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
            var apiInstance = new BackgroundAssetUploadFilesApi(httpClient, config, httpClientHandler);
            var backgroundAssetUploadFileCreateRequest = new BackgroundAssetUploadFileCreateRequest(); // BackgroundAssetUploadFileCreateRequest | BackgroundAssetUploadFile representation

            try
            {
                BackgroundAssetUploadFileResponse result = apiInstance.BackgroundAssetUploadFilesCreateInstance(backgroundAssetUploadFileCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetUploadFilesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetUploadFileResponse> response = apiInstance.BackgroundAssetUploadFilesCreateInstanceWithHttpInfo(backgroundAssetUploadFileCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetUploadFileCreateRequest** | [**BackgroundAssetUploadFileCreateRequest**](BackgroundAssetUploadFileCreateRequest.md) | BackgroundAssetUploadFile representation |  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **201** | Single BackgroundAssetUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetuploadfilesgetinstance"></a>
# **BackgroundAssetUploadFilesGetInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesGetInstance (string id, List<string>? fieldsBackgroundAssetUploadFiles = null)



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
    public class BackgroundAssetUploadFilesGetInstanceExample
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
            var apiInstance = new BackgroundAssetUploadFilesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBackgroundAssetUploadFiles = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetUploadFiles (optional) 

            try
            {
                BackgroundAssetUploadFileResponse result = apiInstance.BackgroundAssetUploadFilesGetInstance(id, fieldsBackgroundAssetUploadFiles);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetUploadFilesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetUploadFileResponse> response = apiInstance.BackgroundAssetUploadFilesGetInstanceWithHttpInfo(id, fieldsBackgroundAssetUploadFiles);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **200** | Single BackgroundAssetUploadFile |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetuploadfilesupdateinstance"></a>
# **BackgroundAssetUploadFilesUpdateInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesUpdateInstance (string id, BackgroundAssetUploadFileUpdateRequest backgroundAssetUploadFileUpdateRequest)



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
    public class BackgroundAssetUploadFilesUpdateInstanceExample
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
            var apiInstance = new BackgroundAssetUploadFilesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var backgroundAssetUploadFileUpdateRequest = new BackgroundAssetUploadFileUpdateRequest(); // BackgroundAssetUploadFileUpdateRequest | BackgroundAssetUploadFile representation

            try
            {
                BackgroundAssetUploadFileResponse result = apiInstance.BackgroundAssetUploadFilesUpdateInstance(id, backgroundAssetUploadFileUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetUploadFilesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetUploadFileResponse> response = apiInstance.BackgroundAssetUploadFilesUpdateInstanceWithHttpInfo(id, backgroundAssetUploadFileUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetUploadFilesApi.BackgroundAssetUploadFilesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **backgroundAssetUploadFileUpdateRequest** | [**BackgroundAssetUploadFileUpdateRequest**](BackgroundAssetUploadFileUpdateRequest.md) | BackgroundAssetUploadFile representation |  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **200** | Single BackgroundAssetUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

