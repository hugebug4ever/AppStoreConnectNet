# AppStoreConnect.Net.Api.BuildBetaDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildBetaDetailsBuildGetToOneRelated**](BuildBetaDetailsApi.md#buildbetadetailsbuildgettoonerelated) | **GET** /v1/buildBetaDetails/{id}/build |  |
| [**BuildBetaDetailsBuildGetToOneRelationship**](BuildBetaDetailsApi.md#buildbetadetailsbuildgettoonerelationship) | **GET** /v1/buildBetaDetails/{id}/relationships/build |  |
| [**BuildBetaDetailsGetCollection**](BuildBetaDetailsApi.md#buildbetadetailsgetcollection) | **GET** /v1/buildBetaDetails |  |
| [**BuildBetaDetailsGetInstance**](BuildBetaDetailsApi.md#buildbetadetailsgetinstance) | **GET** /v1/buildBetaDetails/{id} |  |
| [**BuildBetaDetailsUpdateInstance**](BuildBetaDetailsApi.md#buildbetadetailsupdateinstance) | **PATCH** /v1/buildBetaDetails/{id} |  |

<a id="buildbetadetailsbuildgettoonerelated"></a>
# **BuildBetaDetailsBuildGetToOneRelated**
> BuildResponse BuildBetaDetailsBuildGetToOneRelated (string id, List<string>? fieldsBuilds = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaGroups = null, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsApps = null, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsBuildIcons = null, List<string>? fieldsBuildBundles = null, List<string>? fieldsBuildUploads = null, List<string>? include = null, int? limitIndividualTesters = null, int? limitBetaGroups = null, int? limitBetaBuildLocalizations = null, int? limitIcons = null, int? limitBuildBundles = null)



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
    public class BuildBetaDetailsBuildGetToOneRelatedExample
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
            var apiInstance = new BuildBetaDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var fieldsBetaGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaGroups (optional) 
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsBuildIcons = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildIcons (optional) 
            var fieldsBuildBundles = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBundles (optional) 
            var fieldsBuildUploads = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildUploads (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitIndividualTesters = 56;  // int? | maximum number of related individualTesters returned (when they are included) (optional) 
            var limitBetaGroups = 56;  // int? | maximum number of related betaGroups returned (when they are included) (optional) 
            var limitBetaBuildLocalizations = 56;  // int? | maximum number of related betaBuildLocalizations returned (when they are included) (optional) 
            var limitIcons = 56;  // int? | maximum number of related icons returned (when they are included) (optional) 
            var limitBuildBundles = 56;  // int? | maximum number of related buildBundles returned (when they are included) (optional) 

            try
            {
                BuildResponse result = apiInstance.BuildBetaDetailsBuildGetToOneRelated(id, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaGroups, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, fieldsBuildBundles, fieldsBuildUploads, include, limitIndividualTesters, limitBetaGroups, limitBetaBuildLocalizations, limitIcons, limitBuildBundles);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsBuildGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBetaDetailsBuildGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildResponse> response = apiInstance.BuildBetaDetailsBuildGetToOneRelatedWithHttpInfo(id, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaGroups, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, fieldsBuildBundles, fieldsBuildUploads, include, limitIndividualTesters, limitBetaGroups, limitBetaBuildLocalizations, limitIcons, limitBuildBundles);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsBuildGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **fieldsBuildBundles** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBundles | [optional]  |
| **fieldsBuildUploads** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildUploads | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitIndividualTesters** | **int?** | maximum number of related individualTesters returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int?** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBetaBuildLocalizations** | **int?** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitIcons** | **int?** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int?** | maximum number of related buildBundles returned (when they are included) | [optional]  |

### Return type

[**BuildResponse**](BuildResponse.md)

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
| **200** | Single Build |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbetadetailsbuildgettoonerelationship"></a>
# **BuildBetaDetailsBuildGetToOneRelationship**
> BuildBetaDetailBuildLinkageResponse BuildBetaDetailsBuildGetToOneRelationship (string id)



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
    public class BuildBetaDetailsBuildGetToOneRelationshipExample
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
            var apiInstance = new BuildBetaDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildBetaDetailBuildLinkageResponse result = apiInstance.BuildBetaDetailsBuildGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsBuildGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBetaDetailsBuildGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaDetailBuildLinkageResponse> response = apiInstance.BuildBetaDetailsBuildGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsBuildGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBetaDetailBuildLinkageResponse**](BuildBetaDetailBuildLinkageResponse.md)

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

<a id="buildbetadetailsgetcollection"></a>
# **BuildBetaDetailsGetCollection**
> BuildBetaDetailsResponse BuildBetaDetailsGetCollection (List<string>? filterBuild = null, List<string>? filterId = null, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsBuilds = null, int? limit = null, List<string>? include = null)



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
    public class BuildBetaDetailsGetCollectionExample
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
            var apiInstance = new BuildBetaDetailsApi(httpClient, config, httpClientHandler);
            var filterBuild = new List<string>?(); // List<string>? | filter by id(s) of related 'build' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BuildBetaDetailsResponse result = apiInstance.BuildBetaDetailsGetCollection(filterBuild, filterId, fieldsBuildBetaDetails, fieldsBuilds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBetaDetailsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaDetailsResponse> response = apiInstance.BuildBetaDetailsGetCollectionWithHttpInfo(filterBuild, filterId, fieldsBuildBetaDetails, fieldsBuilds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuild** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;build&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BuildBetaDetailsResponse**](BuildBetaDetailsResponse.md)

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
| **200** | List of BuildBetaDetails |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbetadetailsgetinstance"></a>
# **BuildBetaDetailsGetInstance**
> BuildBetaDetailResponse BuildBetaDetailsGetInstance (string id, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsBuilds = null, List<string>? include = null)



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
    public class BuildBetaDetailsGetInstanceExample
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
            var apiInstance = new BuildBetaDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BuildBetaDetailResponse result = apiInstance.BuildBetaDetailsGetInstance(id, fieldsBuildBetaDetails, fieldsBuilds, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBetaDetailsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaDetailResponse> response = apiInstance.BuildBetaDetailsGetInstanceWithHttpInfo(id, fieldsBuildBetaDetails, fieldsBuilds, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
| **200** | Single BuildBetaDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildbetadetailsupdateinstance"></a>
# **BuildBetaDetailsUpdateInstance**
> BuildBetaDetailResponse BuildBetaDetailsUpdateInstance (string id, BuildBetaDetailUpdateRequest buildBetaDetailUpdateRequest)



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
    public class BuildBetaDetailsUpdateInstanceExample
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
            var apiInstance = new BuildBetaDetailsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildBetaDetailUpdateRequest = new BuildBetaDetailUpdateRequest(); // BuildBetaDetailUpdateRequest | BuildBetaDetail representation

            try
            {
                BuildBetaDetailResponse result = apiInstance.BuildBetaDetailsUpdateInstance(id, buildBetaDetailUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildBetaDetailsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaDetailResponse> response = apiInstance.BuildBetaDetailsUpdateInstanceWithHttpInfo(id, buildBetaDetailUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildBetaDetailsApi.BuildBetaDetailsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaDetailUpdateRequest** | [**BuildBetaDetailUpdateRequest**](BuildBetaDetailUpdateRequest.md) | BuildBetaDetail representation |  |

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
| **200** | Single BuildBetaDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

