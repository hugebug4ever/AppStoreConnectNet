# AppStoreConnect.Net.Api.BuildBundlesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildBundlesAppClipDomainCacheStatusGetToOneRelated**](BuildBundlesApi.md#buildbundlesappclipdomaincachestatusgettoonerelated) | **GET** /v1/buildBundles/{id}/appClipDomainCacheStatus |  |
| [**BuildBundlesAppClipDomainCacheStatusGetToOneRelationship**](BuildBundlesApi.md#buildbundlesappclipdomaincachestatusgettoonerelationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainCacheStatus |  |
| [**BuildBundlesAppClipDomainDebugStatusGetToOneRelated**](BuildBundlesApi.md#buildbundlesappclipdomaindebugstatusgettoonerelated) | **GET** /v1/buildBundles/{id}/appClipDomainDebugStatus |  |
| [**BuildBundlesAppClipDomainDebugStatusGetToOneRelationship**](BuildBundlesApi.md#buildbundlesappclipdomaindebugstatusgettoonerelationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainDebugStatus |  |
| [**BuildBundlesBetaAppClipInvocationsGetToManyRelated**](BuildBundlesApi.md#buildbundlesbetaappclipinvocationsgettomanyrelated) | **GET** /v1/buildBundles/{id}/betaAppClipInvocations |  |
| [**BuildBundlesBetaAppClipInvocationsGetToManyRelationship**](BuildBundlesApi.md#buildbundlesbetaappclipinvocationsgettomanyrelationship) | **GET** /v1/buildBundles/{id}/relationships/betaAppClipInvocations |  |
| [**BuildBundlesBuildBundleFileSizesGetToManyRelated**](BuildBundlesApi.md#buildbundlesbuildbundlefilesizesgettomanyrelated) | **GET** /v1/buildBundles/{id}/buildBundleFileSizes |  |
| [**BuildBundlesBuildBundleFileSizesGetToManyRelationship**](BuildBundlesApi.md#buildbundlesbuildbundlefilesizesgettomanyrelationship) | **GET** /v1/buildBundles/{id}/relationships/buildBundleFileSizes |  |

<a id="buildbundlesappclipdomaincachestatusgettoonerelated"></a>
# **BuildBundlesAppClipDomainCacheStatusGetToOneRelated**
> AppClipDomainStatusResponse BuildBundlesAppClipDomainCacheStatusGetToOneRelated (string id, List<string>? fieldsAppClipDomainStatuses = null)



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
    public class BuildBundlesAppClipDomainCacheStatusGetToOneRelatedExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppClipDomainStatuses = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDomainStatuses (optional) 

            try
            {
                AppClipDomainStatusResponse result = apiInstance.BuildBundlesAppClipDomainCacheStatusGetToOneRelated(id, fieldsAppClipDomainStatuses);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainCacheStatusGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesAppClipDomainCacheStatusGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipDomainStatusResponse> response = apiInstance.BuildBundlesAppClipDomainCacheStatusGetToOneRelatedWithHttpInfo(id, fieldsAppClipDomainStatuses);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainCacheStatusGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipDomainStatuses** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDomainStatuses | [optional]  |

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

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
| **200** | Single AppClipDomainStatus |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbundlesappclipdomaincachestatusgettoonerelationship"></a>
# **BuildBundlesAppClipDomainCacheStatusGetToOneRelationship**
> BuildBundleAppClipDomainCacheStatusLinkageResponse BuildBundlesAppClipDomainCacheStatusGetToOneRelationship (string id)



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
    public class BuildBundlesAppClipDomainCacheStatusGetToOneRelationshipExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildBundleAppClipDomainCacheStatusLinkageResponse result = apiInstance.BuildBundlesAppClipDomainCacheStatusGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainCacheStatusGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesAppClipDomainCacheStatusGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBundleAppClipDomainCacheStatusLinkageResponse> response = apiInstance.BuildBundlesAppClipDomainCacheStatusGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainCacheStatusGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBundleAppClipDomainCacheStatusLinkageResponse**](BuildBundleAppClipDomainCacheStatusLinkageResponse.md)

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

<a id="buildbundlesappclipdomaindebugstatusgettoonerelated"></a>
# **BuildBundlesAppClipDomainDebugStatusGetToOneRelated**
> AppClipDomainStatusResponse BuildBundlesAppClipDomainDebugStatusGetToOneRelated (string id, List<string>? fieldsAppClipDomainStatuses = null)



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
    public class BuildBundlesAppClipDomainDebugStatusGetToOneRelatedExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppClipDomainStatuses = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDomainStatuses (optional) 

            try
            {
                AppClipDomainStatusResponse result = apiInstance.BuildBundlesAppClipDomainDebugStatusGetToOneRelated(id, fieldsAppClipDomainStatuses);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainDebugStatusGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesAppClipDomainDebugStatusGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipDomainStatusResponse> response = apiInstance.BuildBundlesAppClipDomainDebugStatusGetToOneRelatedWithHttpInfo(id, fieldsAppClipDomainStatuses);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainDebugStatusGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipDomainStatuses** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDomainStatuses | [optional]  |

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

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
| **200** | Single AppClipDomainStatus |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbundlesappclipdomaindebugstatusgettoonerelationship"></a>
# **BuildBundlesAppClipDomainDebugStatusGetToOneRelationship**
> BuildBundleAppClipDomainDebugStatusLinkageResponse BuildBundlesAppClipDomainDebugStatusGetToOneRelationship (string id)



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
    public class BuildBundlesAppClipDomainDebugStatusGetToOneRelationshipExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildBundleAppClipDomainDebugStatusLinkageResponse result = apiInstance.BuildBundlesAppClipDomainDebugStatusGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainDebugStatusGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesAppClipDomainDebugStatusGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBundleAppClipDomainDebugStatusLinkageResponse> response = apiInstance.BuildBundlesAppClipDomainDebugStatusGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesAppClipDomainDebugStatusGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBundleAppClipDomainDebugStatusLinkageResponse**](BuildBundleAppClipDomainDebugStatusLinkageResponse.md)

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

<a id="buildbundlesbetaappclipinvocationsgettomanyrelated"></a>
# **BuildBundlesBetaAppClipInvocationsGetToManyRelated**
> BetaAppClipInvocationsResponse BuildBundlesBetaAppClipInvocationsGetToManyRelated (string id, List<string>? fieldsBetaAppClipInvocations = null, List<string>? fieldsBetaAppClipInvocationLocalizations = null, int? limit = null, List<string>? include = null, int? limitBetaAppClipInvocationLocalizations = null)



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
    public class BuildBundlesBetaAppClipInvocationsGetToManyRelatedExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaAppClipInvocations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppClipInvocations (optional) 
            var fieldsBetaAppClipInvocationLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppClipInvocationLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBetaAppClipInvocationLocalizations = 56;  // int? | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) (optional) 

            try
            {
                BetaAppClipInvocationsResponse result = apiInstance.BuildBundlesBetaAppClipInvocationsGetToManyRelated(id, fieldsBetaAppClipInvocations, fieldsBetaAppClipInvocationLocalizations, limit, include, limitBetaAppClipInvocationLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBetaAppClipInvocationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesBetaAppClipInvocationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppClipInvocationsResponse> response = apiInstance.BuildBundlesBetaAppClipInvocationsGetToManyRelatedWithHttpInfo(id, fieldsBetaAppClipInvocations, fieldsBetaAppClipInvocationLocalizations, limit, include, limitBetaAppClipInvocationLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBetaAppClipInvocationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppClipInvocations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppClipInvocations | [optional]  |
| **fieldsBetaAppClipInvocationLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppClipInvocationLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaAppClipInvocationLocalizations** | **int?** | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) | [optional]  |

### Return type

[**BetaAppClipInvocationsResponse**](BetaAppClipInvocationsResponse.md)

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
| **200** | List of BetaAppClipInvocations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbundlesbetaappclipinvocationsgettomanyrelationship"></a>
# **BuildBundlesBetaAppClipInvocationsGetToManyRelationship**
> BuildBundleBetaAppClipInvocationsLinkagesResponse BuildBundlesBetaAppClipInvocationsGetToManyRelationship (string id, int? limit = null)



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
    public class BuildBundlesBetaAppClipInvocationsGetToManyRelationshipExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildBundleBetaAppClipInvocationsLinkagesResponse result = apiInstance.BuildBundlesBetaAppClipInvocationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBetaAppClipInvocationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesBetaAppClipInvocationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBundleBetaAppClipInvocationsLinkagesResponse> response = apiInstance.BuildBundlesBetaAppClipInvocationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBetaAppClipInvocationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildBundleBetaAppClipInvocationsLinkagesResponse**](BuildBundleBetaAppClipInvocationsLinkagesResponse.md)

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

<a id="buildbundlesbuildbundlefilesizesgettomanyrelated"></a>
# **BuildBundlesBuildBundleFileSizesGetToManyRelated**
> BuildBundleFileSizesResponse BuildBundlesBuildBundleFileSizesGetToManyRelated (string id, List<string>? fieldsBuildBundleFileSizes = null, int? limit = null)



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
    public class BuildBundlesBuildBundleFileSizesGetToManyRelatedExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuildBundleFileSizes = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBundleFileSizes (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildBundleFileSizesResponse result = apiInstance.BuildBundlesBuildBundleFileSizesGetToManyRelated(id, fieldsBuildBundleFileSizes, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBuildBundleFileSizesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesBuildBundleFileSizesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBundleFileSizesResponse> response = apiInstance.BuildBundlesBuildBundleFileSizesGetToManyRelatedWithHttpInfo(id, fieldsBuildBundleFileSizes, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBuildBundleFileSizesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildBundleFileSizes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBundleFileSizes | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BuildBundleFileSizesResponse**](BuildBundleFileSizesResponse.md)

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
| **200** | List of BuildBundleFileSizes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbundlesbuildbundlefilesizesgettomanyrelationship"></a>
# **BuildBundlesBuildBundleFileSizesGetToManyRelationship**
> BuildBundleBuildBundleFileSizesLinkagesResponse BuildBundlesBuildBundleFileSizesGetToManyRelationship (string id, int? limit = null)



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
    public class BuildBundlesBuildBundleFileSizesGetToManyRelationshipExample
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
            var apiInstance = new BuildBundlesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildBundleBuildBundleFileSizesLinkagesResponse result = apiInstance.BuildBundlesBuildBundleFileSizesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBuildBundleFileSizesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBundlesBuildBundleFileSizesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBundleBuildBundleFileSizesLinkagesResponse> response = apiInstance.BuildBundlesBuildBundleFileSizesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBundlesApi.BuildBundlesBuildBundleFileSizesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildBundleBuildBundleFileSizesLinkagesResponse**](BuildBundleBuildBundleFileSizesLinkagesResponse.md)

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

