# AppStoreConnect.Net.Api.BuildUploadFilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildUploadFilesCreateInstance**](BuildUploadFilesApi.md#builduploadfilescreateinstance) | **POST** /v1/buildUploadFiles |  |
| [**BuildUploadFilesGetInstance**](BuildUploadFilesApi.md#builduploadfilesgetinstance) | **GET** /v1/buildUploadFiles/{id} |  |
| [**BuildUploadFilesUpdateInstance**](BuildUploadFilesApi.md#builduploadfilesupdateinstance) | **PATCH** /v1/buildUploadFiles/{id} |  |

<a id="builduploadfilescreateinstance"></a>
# **BuildUploadFilesCreateInstance**
> BuildUploadFileResponse BuildUploadFilesCreateInstance (BuildUploadFileCreateRequest buildUploadFileCreateRequest)



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
    public class BuildUploadFilesCreateInstanceExample
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
            var apiInstance = new BuildUploadFilesApi(httpClient, config, httpClientHandler);
            var buildUploadFileCreateRequest = new BuildUploadFileCreateRequest(); // BuildUploadFileCreateRequest | BuildUploadFile representation

            try
            {
                BuildUploadFileResponse result = apiInstance.BuildUploadFilesCreateInstance(buildUploadFileCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildUploadFilesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildUploadFileResponse> response = apiInstance.BuildUploadFilesCreateInstanceWithHttpInfo(buildUploadFileCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **buildUploadFileCreateRequest** | [**BuildUploadFileCreateRequest**](BuildUploadFileCreateRequest.md) | BuildUploadFile representation |  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **201** | Single BuildUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="builduploadfilesgetinstance"></a>
# **BuildUploadFilesGetInstance**
> BuildUploadFileResponse BuildUploadFilesGetInstance (string id, List<string>? fieldsBuildUploadFiles = null)



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
    public class BuildUploadFilesGetInstanceExample
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
            var apiInstance = new BuildUploadFilesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuildUploadFiles = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildUploadFiles (optional) 

            try
            {
                BuildUploadFileResponse result = apiInstance.BuildUploadFilesGetInstance(id, fieldsBuildUploadFiles);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildUploadFilesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildUploadFileResponse> response = apiInstance.BuildUploadFilesGetInstanceWithHttpInfo(id, fieldsBuildUploadFiles);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildUploadFiles** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildUploadFiles | [optional]  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **200** | Single BuildUploadFile |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="builduploadfilesupdateinstance"></a>
# **BuildUploadFilesUpdateInstance**
> BuildUploadFileResponse BuildUploadFilesUpdateInstance (string id, BuildUploadFileUpdateRequest buildUploadFileUpdateRequest)



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
    public class BuildUploadFilesUpdateInstanceExample
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
            var apiInstance = new BuildUploadFilesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildUploadFileUpdateRequest = new BuildUploadFileUpdateRequest(); // BuildUploadFileUpdateRequest | BuildUploadFile representation

            try
            {
                BuildUploadFileResponse result = apiInstance.BuildUploadFilesUpdateInstance(id, buildUploadFileUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildUploadFilesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildUploadFileResponse> response = apiInstance.BuildUploadFilesUpdateInstanceWithHttpInfo(id, buildUploadFileUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildUploadFilesApi.BuildUploadFilesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildUploadFileUpdateRequest** | [**BuildUploadFileUpdateRequest**](BuildUploadFileUpdateRequest.md) | BuildUploadFile representation |  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **200** | Single BuildUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

