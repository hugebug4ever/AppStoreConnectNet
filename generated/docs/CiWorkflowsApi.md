# AppStoreConnect.Net.Api.CiWorkflowsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiWorkflowsBuildRunsGetToManyRelated**](CiWorkflowsApi.md#ciworkflowsbuildrunsgettomanyrelated) | **GET** /v1/ciWorkflows/{id}/buildRuns |  |
| [**CiWorkflowsBuildRunsGetToManyRelationship**](CiWorkflowsApi.md#ciworkflowsbuildrunsgettomanyrelationship) | **GET** /v1/ciWorkflows/{id}/relationships/buildRuns |  |
| [**CiWorkflowsCreateInstance**](CiWorkflowsApi.md#ciworkflowscreateinstance) | **POST** /v1/ciWorkflows |  |
| [**CiWorkflowsDeleteInstance**](CiWorkflowsApi.md#ciworkflowsdeleteinstance) | **DELETE** /v1/ciWorkflows/{id} |  |
| [**CiWorkflowsGetInstance**](CiWorkflowsApi.md#ciworkflowsgetinstance) | **GET** /v1/ciWorkflows/{id} |  |
| [**CiWorkflowsRepositoryGetToOneRelated**](CiWorkflowsApi.md#ciworkflowsrepositorygettoonerelated) | **GET** /v1/ciWorkflows/{id}/repository |  |
| [**CiWorkflowsRepositoryGetToOneRelationship**](CiWorkflowsApi.md#ciworkflowsrepositorygettoonerelationship) | **GET** /v1/ciWorkflows/{id}/relationships/repository |  |
| [**CiWorkflowsUpdateInstance**](CiWorkflowsApi.md#ciworkflowsupdateinstance) | **PATCH** /v1/ciWorkflows/{id} |  |

<a id="ciworkflowsbuildrunsgettomanyrelated"></a>
# **CiWorkflowsBuildRunsGetToManyRelated**
> CiBuildRunsResponse CiWorkflowsBuildRunsGetToManyRelated (string id, List<string>? filterBuilds = null, List<string>? sort = null, List<string>? fieldsCiBuildRuns = null, List<string>? fieldsBuilds = null, List<string>? fieldsCiWorkflows = null, List<string>? fieldsCiProducts = null, List<string>? fieldsScmGitReferences = null, List<string>? fieldsScmPullRequests = null, int? limit = null, List<string>? include = null, int? limitBuilds = null)



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
    public class CiWorkflowsBuildRunsGetToManyRelatedExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterBuilds = new List<string>?(); // List<string>? | filter by id(s) of related 'builds' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsCiBuildRuns = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciBuildRuns (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsCiWorkflows = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciWorkflows (optional) 
            var fieldsCiProducts = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciProducts (optional) 
            var fieldsScmGitReferences = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmGitReferences (optional) 
            var fieldsScmPullRequests = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmPullRequests (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                CiBuildRunsResponse result = apiInstance.CiWorkflowsBuildRunsGetToManyRelated(id, filterBuilds, sort, fieldsCiBuildRuns, fieldsBuilds, fieldsCiWorkflows, fieldsCiProducts, fieldsScmGitReferences, fieldsScmPullRequests, limit, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsBuildRunsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsBuildRunsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunsResponse> response = apiInstance.CiWorkflowsBuildRunsGetToManyRelatedWithHttpInfo(id, filterBuilds, sort, fieldsCiBuildRuns, fieldsBuilds, fieldsCiWorkflows, fieldsCiProducts, fieldsScmGitReferences, fieldsScmPullRequests, limit, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsBuildRunsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterBuilds** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **fieldsScmPullRequests** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmPullRequests | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**CiBuildRunsResponse**](CiBuildRunsResponse.md)

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
| **200** | List of CiBuildRuns |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciworkflowsbuildrunsgettomanyrelationship"></a>
# **CiWorkflowsBuildRunsGetToManyRelationship**
> CiWorkflowBuildRunsLinkagesResponse CiWorkflowsBuildRunsGetToManyRelationship (string id, int? limit = null)



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
    public class CiWorkflowsBuildRunsGetToManyRelationshipExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiWorkflowBuildRunsLinkagesResponse result = apiInstance.CiWorkflowsBuildRunsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsBuildRunsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsBuildRunsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowBuildRunsLinkagesResponse> response = apiInstance.CiWorkflowsBuildRunsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsBuildRunsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiWorkflowBuildRunsLinkagesResponse**](CiWorkflowBuildRunsLinkagesResponse.md)

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

<a id="ciworkflowscreateinstance"></a>
# **CiWorkflowsCreateInstance**
> CiWorkflowResponse CiWorkflowsCreateInstance (CiWorkflowCreateRequest ciWorkflowCreateRequest)



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
    public class CiWorkflowsCreateInstanceExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var ciWorkflowCreateRequest = new CiWorkflowCreateRequest(); // CiWorkflowCreateRequest | CiWorkflow representation

            try
            {
                CiWorkflowResponse result = apiInstance.CiWorkflowsCreateInstance(ciWorkflowCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowResponse> response = apiInstance.CiWorkflowsCreateInstanceWithHttpInfo(ciWorkflowCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **ciWorkflowCreateRequest** | [**CiWorkflowCreateRequest**](CiWorkflowCreateRequest.md) | CiWorkflow representation |  |

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
| **201** | Single CiWorkflow |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciworkflowsdeleteinstance"></a>
# **CiWorkflowsDeleteInstance**
> void CiWorkflowsDeleteInstance (string id)



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
    public class CiWorkflowsDeleteInstanceExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.CiWorkflowsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.CiWorkflowsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="ciworkflowsgetinstance"></a>
# **CiWorkflowsGetInstance**
> CiWorkflowResponse CiWorkflowsGetInstance (string id, List<string>? fieldsCiWorkflows = null, List<string>? fieldsScmRepositories = null, List<string>? include = null)



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
    public class CiWorkflowsGetInstanceExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiWorkflows = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciWorkflows (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CiWorkflowResponse result = apiInstance.CiWorkflowsGetInstance(id, fieldsCiWorkflows, fieldsScmRepositories, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowResponse> response = apiInstance.CiWorkflowsGetInstanceWithHttpInfo(id, fieldsCiWorkflows, fieldsScmRepositories, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
| **200** | Single CiWorkflow |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciworkflowsrepositorygettoonerelated"></a>
# **CiWorkflowsRepositoryGetToOneRelated**
> ScmRepositoryResponse CiWorkflowsRepositoryGetToOneRelated (string id, List<string>? fieldsScmRepositories = null, List<string>? fieldsScmProviders = null, List<string>? fieldsScmGitReferences = null, List<string>? include = null)



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
    public class CiWorkflowsRepositoryGetToOneRelatedExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var fieldsScmProviders = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmProviders (optional) 
            var fieldsScmGitReferences = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmGitReferences (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                ScmRepositoryResponse result = apiInstance.CiWorkflowsRepositoryGetToOneRelated(id, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsRepositoryGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsRepositoryGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<ScmRepositoryResponse> response = apiInstance.CiWorkflowsRepositoryGetToOneRelatedWithHttpInfo(id, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsRepositoryGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmRepositoryResponse**](ScmRepositoryResponse.md)

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
| **200** | Single ScmRepository |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciworkflowsrepositorygettoonerelationship"></a>
# **CiWorkflowsRepositoryGetToOneRelationship**
> CiWorkflowRepositoryLinkageResponse CiWorkflowsRepositoryGetToOneRelationship (string id)



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
    public class CiWorkflowsRepositoryGetToOneRelationshipExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                CiWorkflowRepositoryLinkageResponse result = apiInstance.CiWorkflowsRepositoryGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsRepositoryGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsRepositoryGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowRepositoryLinkageResponse> response = apiInstance.CiWorkflowsRepositoryGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsRepositoryGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CiWorkflowRepositoryLinkageResponse**](CiWorkflowRepositoryLinkageResponse.md)

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

<a id="ciworkflowsupdateinstance"></a>
# **CiWorkflowsUpdateInstance**
> CiWorkflowResponse CiWorkflowsUpdateInstance (string id, CiWorkflowUpdateRequest ciWorkflowUpdateRequest)



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
    public class CiWorkflowsUpdateInstanceExample
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
            var apiInstance = new CiWorkflowsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var ciWorkflowUpdateRequest = new CiWorkflowUpdateRequest(); // CiWorkflowUpdateRequest | CiWorkflow representation

            try
            {
                CiWorkflowResponse result = apiInstance.CiWorkflowsUpdateInstance(id, ciWorkflowUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiWorkflowsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowResponse> response = apiInstance.CiWorkflowsUpdateInstanceWithHttpInfo(id, ciWorkflowUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiWorkflowsApi.CiWorkflowsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **ciWorkflowUpdateRequest** | [**CiWorkflowUpdateRequest**](CiWorkflowUpdateRequest.md) | CiWorkflow representation |  |

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
| **200** | Single CiWorkflow |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

