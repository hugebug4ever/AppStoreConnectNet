# AppStoreConnect.Net.Api.BackgroundAssetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetsCreateInstance**](BackgroundAssetsApi.md#backgroundassetscreateinstance) | **POST** /v1/backgroundAssets |  |
| [**BackgroundAssetsGetInstance**](BackgroundAssetsApi.md#backgroundassetsgetinstance) | **GET** /v1/backgroundAssets/{id} |  |
| [**BackgroundAssetsUpdateInstance**](BackgroundAssetsApi.md#backgroundassetsupdateinstance) | **PATCH** /v1/backgroundAssets/{id} |  |
| [**BackgroundAssetsVersionsGetToManyRelated**](BackgroundAssetsApi.md#backgroundassetsversionsgettomanyrelated) | **GET** /v1/backgroundAssets/{id}/versions |  |
| [**BackgroundAssetsVersionsGetToManyRelationship**](BackgroundAssetsApi.md#backgroundassetsversionsgettomanyrelationship) | **GET** /v1/backgroundAssets/{id}/relationships/versions |  |

<a id="backgroundassetscreateinstance"></a>
# **BackgroundAssetsCreateInstance**
> BackgroundAssetResponse BackgroundAssetsCreateInstance (BackgroundAssetCreateRequest backgroundAssetCreateRequest)



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
    public class BackgroundAssetsCreateInstanceExample
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
            var apiInstance = new BackgroundAssetsApi(httpClient, config, httpClientHandler);
            var backgroundAssetCreateRequest = new BackgroundAssetCreateRequest(); // BackgroundAssetCreateRequest | BackgroundAsset representation

            try
            {
                BackgroundAssetResponse result = apiInstance.BackgroundAssetsCreateInstance(backgroundAssetCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetResponse> response = apiInstance.BackgroundAssetsCreateInstanceWithHttpInfo(backgroundAssetCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetCreateRequest** | [**BackgroundAssetCreateRequest**](BackgroundAssetCreateRequest.md) | BackgroundAsset representation |  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **201** | Single BackgroundAsset |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetsgetinstance"></a>
# **BackgroundAssetsGetInstance**
> BackgroundAssetResponse BackgroundAssetsGetInstance (string id, List<string>? fieldsBackgroundAssets = null, List<string>? include = null)



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
    public class BackgroundAssetsGetInstanceExample
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
            var apiInstance = new BackgroundAssetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBackgroundAssets = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssets (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BackgroundAssetResponse result = apiInstance.BackgroundAssetsGetInstance(id, fieldsBackgroundAssets, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetResponse> response = apiInstance.BackgroundAssetsGetInstanceWithHttpInfo(id, fieldsBackgroundAssets, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssets | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **200** | Single BackgroundAsset |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetsupdateinstance"></a>
# **BackgroundAssetsUpdateInstance**
> BackgroundAssetResponse BackgroundAssetsUpdateInstance (string id, BackgroundAssetUpdateRequest backgroundAssetUpdateRequest)



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
    public class BackgroundAssetsUpdateInstanceExample
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
            var apiInstance = new BackgroundAssetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var backgroundAssetUpdateRequest = new BackgroundAssetUpdateRequest(); // BackgroundAssetUpdateRequest | BackgroundAsset representation

            try
            {
                BackgroundAssetResponse result = apiInstance.BackgroundAssetsUpdateInstance(id, backgroundAssetUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetResponse> response = apiInstance.BackgroundAssetsUpdateInstanceWithHttpInfo(id, backgroundAssetUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **backgroundAssetUpdateRequest** | [**BackgroundAssetUpdateRequest**](BackgroundAssetUpdateRequest.md) | BackgroundAsset representation |  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **200** | Single BackgroundAsset |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetsversionsgettomanyrelated"></a>
# **BackgroundAssetsVersionsGetToManyRelated**
> BackgroundAssetVersionsResponse BackgroundAssetsVersionsGetToManyRelated (string id, List<string>? filterState = null, List<string>? filterVersion = null, List<string>? filterInternalBetaReleaseState = null, List<string>? filterExternalBetaReleaseState = null, List<string>? filterAppStoreReleaseState = null, List<string>? sort = null, List<string>? fieldsBackgroundAssetVersions = null, List<string>? fieldsBackgroundAssets = null, List<string>? fieldsBackgroundAssetVersionInternalBetaReleases = null, List<string>? fieldsBackgroundAssetVersionExternalBetaReleases = null, List<string>? fieldsBackgroundAssetVersionAppStoreReleases = null, List<string>? fieldsBackgroundAssetUploadFiles = null, int? limit = null, List<string>? include = null)



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
    public class BackgroundAssetsVersionsGetToManyRelatedExample
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
            var apiInstance = new BackgroundAssetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterState = new List<string>?(); // List<string>? | filter by attribute 'state' (optional) 
            var filterVersion = new List<string>?(); // List<string>? | filter by attribute 'version' (optional) 
            var filterInternalBetaReleaseState = new List<string>?(); // List<string>? | filter by attribute 'internalBetaRelease.state' (optional) 
            var filterExternalBetaReleaseState = new List<string>?(); // List<string>? | filter by attribute 'externalBetaRelease.state' (optional) 
            var filterAppStoreReleaseState = new List<string>?(); // List<string>? | filter by attribute 'appStoreRelease.state' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsBackgroundAssetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersions (optional) 
            var fieldsBackgroundAssets = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssets (optional) 
            var fieldsBackgroundAssetVersionInternalBetaReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases (optional) 
            var fieldsBackgroundAssetVersionExternalBetaReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases (optional) 
            var fieldsBackgroundAssetVersionAppStoreReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersionAppStoreReleases (optional) 
            var fieldsBackgroundAssetUploadFiles = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetUploadFiles (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BackgroundAssetVersionsResponse result = apiInstance.BackgroundAssetsVersionsGetToManyRelated(id, filterState, filterVersion, filterInternalBetaReleaseState, filterExternalBetaReleaseState, filterAppStoreReleaseState, sort, fieldsBackgroundAssetVersions, fieldsBackgroundAssets, fieldsBackgroundAssetVersionInternalBetaReleases, fieldsBackgroundAssetVersionExternalBetaReleases, fieldsBackgroundAssetVersionAppStoreReleases, fieldsBackgroundAssetUploadFiles, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetsVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionsResponse> response = apiInstance.BackgroundAssetsVersionsGetToManyRelatedWithHttpInfo(id, filterState, filterVersion, filterInternalBetaReleaseState, filterExternalBetaReleaseState, filterAppStoreReleaseState, sort, fieldsBackgroundAssetVersions, fieldsBackgroundAssets, fieldsBackgroundAssetVersionInternalBetaReleases, fieldsBackgroundAssetVersionExternalBetaReleases, fieldsBackgroundAssetVersionAppStoreReleases, fieldsBackgroundAssetUploadFiles, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **filterVersion** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterInternalBetaReleaseState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;internalBetaRelease.state&#39; | [optional]  |
| **filterExternalBetaReleaseState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;externalBetaRelease.state&#39; | [optional]  |
| **filterAppStoreReleaseState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;appStoreRelease.state&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBackgroundAssetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersions | [optional]  |
| **fieldsBackgroundAssets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssets | [optional]  |
| **fieldsBackgroundAssetVersionInternalBetaReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases | [optional]  |
| **fieldsBackgroundAssetVersionExternalBetaReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases | [optional]  |
| **fieldsBackgroundAssetVersionAppStoreReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersionAppStoreReleases | [optional]  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionsResponse**](BackgroundAssetVersionsResponse.md)

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
| **200** | List of BackgroundAssetVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="backgroundassetsversionsgettomanyrelationship"></a>
# **BackgroundAssetsVersionsGetToManyRelationship**
> BackgroundAssetVersionsLinkagesResponse BackgroundAssetsVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class BackgroundAssetsVersionsGetToManyRelationshipExample
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
            var apiInstance = new BackgroundAssetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BackgroundAssetVersionsLinkagesResponse result = apiInstance.BackgroundAssetsVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetsVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionsLinkagesResponse> response = apiInstance.BackgroundAssetsVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetsApi.BackgroundAssetsVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BackgroundAssetVersionsLinkagesResponse**](BackgroundAssetVersionsLinkagesResponse.md)

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

