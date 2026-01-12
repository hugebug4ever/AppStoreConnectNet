# AppStoreConnect.Net.Api.PreReleaseVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**PreReleaseVersionsAppGetToOneRelated**](PreReleaseVersionsApi.md#prereleaseversionsappgettoonerelated) | **GET** /v1/preReleaseVersions/{id}/app |  |
| [**PreReleaseVersionsAppGetToOneRelationship**](PreReleaseVersionsApi.md#prereleaseversionsappgettoonerelationship) | **GET** /v1/preReleaseVersions/{id}/relationships/app |  |
| [**PreReleaseVersionsBuildsGetToManyRelated**](PreReleaseVersionsApi.md#prereleaseversionsbuildsgettomanyrelated) | **GET** /v1/preReleaseVersions/{id}/builds |  |
| [**PreReleaseVersionsBuildsGetToManyRelationship**](PreReleaseVersionsApi.md#prereleaseversionsbuildsgettomanyrelationship) | **GET** /v1/preReleaseVersions/{id}/relationships/builds |  |
| [**PreReleaseVersionsGetCollection**](PreReleaseVersionsApi.md#prereleaseversionsgetcollection) | **GET** /v1/preReleaseVersions |  |
| [**PreReleaseVersionsGetInstance**](PreReleaseVersionsApi.md#prereleaseversionsgetinstance) | **GET** /v1/preReleaseVersions/{id} |  |

<a id="prereleaseversionsappgettoonerelated"></a>
# **PreReleaseVersionsAppGetToOneRelated**
> AppWithoutIncludesResponse PreReleaseVersionsAppGetToOneRelated (string id, List<string>? fieldsApps = null)



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
    public class PreReleaseVersionsAppGetToOneRelatedExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 

            try
            {
                AppWithoutIncludesResponse result = apiInstance.PreReleaseVersionsAppGetToOneRelated(id, fieldsApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppWithoutIncludesResponse> response = apiInstance.PreReleaseVersionsAppGetToOneRelatedWithHttpInfo(id, fieldsApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsAppGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="prereleaseversionsappgettoonerelationship"></a>
# **PreReleaseVersionsAppGetToOneRelationship**
> PrereleaseVersionAppLinkageResponse PreReleaseVersionsAppGetToOneRelationship (string id)



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
    public class PreReleaseVersionsAppGetToOneRelationshipExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                PrereleaseVersionAppLinkageResponse result = apiInstance.PreReleaseVersionsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PrereleaseVersionAppLinkageResponse> response = apiInstance.PreReleaseVersionsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**PrereleaseVersionAppLinkageResponse**](PrereleaseVersionAppLinkageResponse.md)

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

<a id="prereleaseversionsbuildsgettomanyrelated"></a>
# **PreReleaseVersionsBuildsGetToManyRelated**
> BuildsWithoutIncludesResponse PreReleaseVersionsBuildsGetToManyRelated (string id, List<string>? fieldsBuilds = null, int? limit = null)



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
    public class PreReleaseVersionsBuildsGetToManyRelatedExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildsWithoutIncludesResponse result = apiInstance.PreReleaseVersionsBuildsGetToManyRelated(id, fieldsBuilds, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsBuildsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsBuildsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildsWithoutIncludesResponse> response = apiInstance.PreReleaseVersionsBuildsGetToManyRelatedWithHttpInfo(id, fieldsBuilds, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsBuildsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BuildsWithoutIncludesResponse**](BuildsWithoutIncludesResponse.md)

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
| **200** | List of Builds with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="prereleaseversionsbuildsgettomanyrelationship"></a>
# **PreReleaseVersionsBuildsGetToManyRelationship**
> PrereleaseVersionBuildsLinkagesResponse PreReleaseVersionsBuildsGetToManyRelationship (string id, int? limit = null)



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
    public class PreReleaseVersionsBuildsGetToManyRelationshipExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                PrereleaseVersionBuildsLinkagesResponse result = apiInstance.PreReleaseVersionsBuildsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsBuildsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsBuildsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PrereleaseVersionBuildsLinkagesResponse> response = apiInstance.PreReleaseVersionsBuildsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsBuildsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**PrereleaseVersionBuildsLinkagesResponse**](PrereleaseVersionBuildsLinkagesResponse.md)

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

<a id="prereleaseversionsgetcollection"></a>
# **PreReleaseVersionsGetCollection**
> PreReleaseVersionsResponse PreReleaseVersionsGetCollection (List<string>? filterBuildsBuildAudienceType = null, List<string>? filterBuildsExpired = null, List<string>? filterBuildsProcessingState = null, List<string>? filterBuildsVersion = null, List<string>? filterPlatform = null, List<string>? filterVersion = null, List<string>? filterApp = null, List<string>? filterBuilds = null, List<string>? sort = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBuilds = null, List<string>? fieldsApps = null, int? limit = null, List<string>? include = null, int? limitBuilds = null)



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
    public class PreReleaseVersionsGetCollectionExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var filterBuildsBuildAudienceType = new List<string>?(); // List<string>? | filter by attribute 'builds.buildAudienceType' (optional) 
            var filterBuildsExpired = new List<string>?(); // List<string>? | filter by attribute 'builds.expired' (optional) 
            var filterBuildsProcessingState = new List<string>?(); // List<string>? | filter by attribute 'builds.processingState' (optional) 
            var filterBuildsVersion = new List<string>?(); // List<string>? | filter by attribute 'builds.version' (optional) 
            var filterPlatform = new List<string>?(); // List<string>? | filter by attribute 'platform' (optional) 
            var filterVersion = new List<string>?(); // List<string>? | filter by attribute 'version' (optional) 
            var filterApp = new List<string>?(); // List<string>? | filter by id(s) of related 'app' (optional) 
            var filterBuilds = new List<string>?(); // List<string>? | filter by id(s) of related 'builds' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                PreReleaseVersionsResponse result = apiInstance.PreReleaseVersionsGetCollection(filterBuildsBuildAudienceType, filterBuildsExpired, filterBuildsProcessingState, filterBuildsVersion, filterPlatform, filterVersion, filterApp, filterBuilds, sort, fieldsPreReleaseVersions, fieldsBuilds, fieldsApps, limit, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PreReleaseVersionsResponse> response = apiInstance.PreReleaseVersionsGetCollectionWithHttpInfo(filterBuildsBuildAudienceType, filterBuildsExpired, filterBuildsProcessingState, filterBuildsVersion, filterPlatform, filterVersion, filterApp, filterBuilds, sort, fieldsPreReleaseVersions, fieldsBuilds, fieldsApps, limit, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuildsBuildAudienceType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;builds.buildAudienceType&#39; | [optional]  |
| **filterBuildsExpired** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;builds.expired&#39; | [optional]  |
| **filterBuildsProcessingState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;builds.processingState&#39; | [optional]  |
| **filterBuildsVersion** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;builds.version&#39; | [optional]  |
| **filterPlatform** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterVersion** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**PreReleaseVersionsResponse**](PreReleaseVersionsResponse.md)

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
| **200** | List of PreReleaseVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="prereleaseversionsgetinstance"></a>
# **PreReleaseVersionsGetInstance**
> PrereleaseVersionResponse PreReleaseVersionsGetInstance (string id, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBuilds = null, List<string>? fieldsApps = null, List<string>? include = null, int? limitBuilds = null)



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
    public class PreReleaseVersionsGetInstanceExample
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
            var apiInstance = new PreReleaseVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                PrereleaseVersionResponse result = apiInstance.PreReleaseVersionsGetInstance(id, fieldsPreReleaseVersions, fieldsBuilds, fieldsApps, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PreReleaseVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PrereleaseVersionResponse> response = apiInstance.PreReleaseVersionsGetInstanceWithHttpInfo(id, fieldsPreReleaseVersions, fieldsBuilds, fieldsApps, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PreReleaseVersionsApi.PreReleaseVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**PrereleaseVersionResponse**](PrereleaseVersionResponse.md)

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
| **200** | Single PrereleaseVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

