# AppStoreConnect.Net.Api.BackgroundAssetVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated**](BackgroundAssetVersionsApi.md#backgroundassetversionsbackgroundassetuploadfilesgettomanyrelated) | **GET** /v1/backgroundAssetVersions/{id}/backgroundAssetUploadFiles |  |
| [**BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship**](BackgroundAssetVersionsApi.md#backgroundassetversionsbackgroundassetuploadfilesgettomanyrelationship) | **GET** /v1/backgroundAssetVersions/{id}/relationships/backgroundAssetUploadFiles |  |
| [**BackgroundAssetVersionsCreateInstance**](BackgroundAssetVersionsApi.md#backgroundassetversionscreateinstance) | **POST** /v1/backgroundAssetVersions |  |
| [**BackgroundAssetVersionsGetInstance**](BackgroundAssetVersionsApi.md#backgroundassetversionsgetinstance) | **GET** /v1/backgroundAssetVersions/{id} |  |

<a id="backgroundassetversionsbackgroundassetuploadfilesgettomanyrelated"></a>
# **BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated**
> BackgroundAssetUploadFilesResponse BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated (string id, List<string>? fieldsBackgroundAssetUploadFiles = null, int? limit = null)



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
    public class BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelatedExample
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
            var apiInstance = new BackgroundAssetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBackgroundAssetUploadFiles = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetUploadFiles (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BackgroundAssetUploadFilesResponse result = apiInstance.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated(id, fieldsBackgroundAssetUploadFiles, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetUploadFilesResponse> response = apiInstance.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelatedWithHttpInfo(id, fieldsBackgroundAssetUploadFiles, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BackgroundAssetUploadFilesResponse**](BackgroundAssetUploadFilesResponse.md)

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
| **200** | List of BackgroundAssetUploadFiles |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetversionsbackgroundassetuploadfilesgettomanyrelationship"></a>
# **BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship**
> BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship (string id, int? limit = null)



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
    public class BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationshipExample
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
            var apiInstance = new BackgroundAssetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse result = apiInstance.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse> response = apiInstance.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse**](BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.md)

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

<a id="backgroundassetversionscreateinstance"></a>
# **BackgroundAssetVersionsCreateInstance**
> BackgroundAssetVersionResponse BackgroundAssetVersionsCreateInstance (BackgroundAssetVersionCreateRequest backgroundAssetVersionCreateRequest)



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
    public class BackgroundAssetVersionsCreateInstanceExample
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
            var apiInstance = new BackgroundAssetVersionsApi(httpClient, config, httpClientHandler);
            var backgroundAssetVersionCreateRequest = new BackgroundAssetVersionCreateRequest(); // BackgroundAssetVersionCreateRequest | BackgroundAssetVersion representation

            try
            {
                BackgroundAssetVersionResponse result = apiInstance.BackgroundAssetVersionsCreateInstance(backgroundAssetVersionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetVersionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionResponse> response = apiInstance.BackgroundAssetVersionsCreateInstanceWithHttpInfo(backgroundAssetVersionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetVersionCreateRequest** | [**BackgroundAssetVersionCreateRequest**](BackgroundAssetVersionCreateRequest.md) | BackgroundAssetVersion representation |  |

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
| **201** | Single BackgroundAssetVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetversionsgetinstance"></a>
# **BackgroundAssetVersionsGetInstance**
> BackgroundAssetVersionResponse BackgroundAssetVersionsGetInstance (string id, List<string>? fieldsBackgroundAssetVersions = null, List<string>? include = null)



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
    public class BackgroundAssetVersionsGetInstanceExample
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
            var apiInstance = new BackgroundAssetVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBackgroundAssetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BackgroundAssetVersionResponse result = apiInstance.BackgroundAssetVersionsGetInstance(id, fieldsBackgroundAssetVersions, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionResponse> response = apiInstance.BackgroundAssetVersionsGetInstanceWithHttpInfo(id, fieldsBackgroundAssetVersions, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetVersionsApi.BackgroundAssetVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
| **200** | Single BackgroundAssetVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

