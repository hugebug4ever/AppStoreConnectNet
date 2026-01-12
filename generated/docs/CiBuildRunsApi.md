# AppStoreConnect.Net.Api.CiBuildRunsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiBuildRunsActionsGetToManyRelated**](CiBuildRunsApi.md#cibuildrunsactionsgettomanyrelated) | **GET** /v1/ciBuildRuns/{id}/actions |  |
| [**CiBuildRunsActionsGetToManyRelationship**](CiBuildRunsApi.md#cibuildrunsactionsgettomanyrelationship) | **GET** /v1/ciBuildRuns/{id}/relationships/actions |  |
| [**CiBuildRunsBuildsGetToManyRelated**](CiBuildRunsApi.md#cibuildrunsbuildsgettomanyrelated) | **GET** /v1/ciBuildRuns/{id}/builds |  |
| [**CiBuildRunsBuildsGetToManyRelationship**](CiBuildRunsApi.md#cibuildrunsbuildsgettomanyrelationship) | **GET** /v1/ciBuildRuns/{id}/relationships/builds |  |
| [**CiBuildRunsCreateInstance**](CiBuildRunsApi.md#cibuildrunscreateinstance) | **POST** /v1/ciBuildRuns |  |
| [**CiBuildRunsGetInstance**](CiBuildRunsApi.md#cibuildrunsgetinstance) | **GET** /v1/ciBuildRuns/{id} |  |

<a id="cibuildrunsactionsgettomanyrelated"></a>
# **CiBuildRunsActionsGetToManyRelated**
> CiBuildActionsResponse CiBuildRunsActionsGetToManyRelated (string id, List<string>? fieldsCiBuildActions = null, List<string>? fieldsCiBuildRuns = null, int? limit = null, List<string>? include = null)



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
    public class CiBuildRunsActionsGetToManyRelatedExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiBuildActions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciBuildActions (optional) 
            var fieldsCiBuildRuns = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciBuildRuns (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CiBuildActionsResponse result = apiInstance.CiBuildRunsActionsGetToManyRelated(id, fieldsCiBuildActions, fieldsCiBuildRuns, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsActionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsActionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildActionsResponse> response = apiInstance.CiBuildRunsActionsGetToManyRelatedWithHttpInfo(id, fieldsCiBuildActions, fieldsCiBuildRuns, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsActionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildActions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciBuildActions | [optional]  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CiBuildActionsResponse**](CiBuildActionsResponse.md)

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
| **200** | List of CiBuildActions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cibuildrunsactionsgettomanyrelationship"></a>
# **CiBuildRunsActionsGetToManyRelationship**
> CiBuildRunActionsLinkagesResponse CiBuildRunsActionsGetToManyRelationship (string id, int? limit = null)



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
    public class CiBuildRunsActionsGetToManyRelationshipExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiBuildRunActionsLinkagesResponse result = apiInstance.CiBuildRunsActionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsActionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsActionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunActionsLinkagesResponse> response = apiInstance.CiBuildRunsActionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsActionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiBuildRunActionsLinkagesResponse**](CiBuildRunActionsLinkagesResponse.md)

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

<a id="cibuildrunsbuildsgettomanyrelated"></a>
# **CiBuildRunsBuildsGetToManyRelated**
> BuildsResponse CiBuildRunsBuildsGetToManyRelated (string id, List<string>? filterVersion = null, List<string>? filterExpired = null, List<string>? filterProcessingState = null, List<string>? filterBetaAppReviewSubmissionBetaReviewState = null, List<string>? filterUsesNonExemptEncryption = null, List<string>? filterPreReleaseVersionVersion = null, List<string>? filterPreReleaseVersionPlatform = null, List<string>? filterBuildAudienceType = null, List<string>? filterPreReleaseVersion = null, List<string>? filterApp = null, List<string>? filterBetaGroups = null, List<string>? filterAppStoreVersion = null, List<string>? filterId = null, bool? existsUsesNonExemptEncryption = null, List<string>? sort = null, List<string>? fieldsBuilds = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaGroups = null, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsApps = null, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsBuildIcons = null, List<string>? fieldsBuildBundles = null, List<string>? fieldsBuildUploads = null, int? limit = null, List<string>? include = null, int? limitIndividualTesters = null, int? limitBetaGroups = null, int? limitBetaBuildLocalizations = null, int? limitIcons = null, int? limitBuildBundles = null)



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
    public class CiBuildRunsBuildsGetToManyRelatedExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterVersion = new List<string>?(); // List<string>? | filter by attribute 'version' (optional) 
            var filterExpired = new List<string>?(); // List<string>? | filter by attribute 'expired' (optional) 
            var filterProcessingState = new List<string>?(); // List<string>? | filter by attribute 'processingState' (optional) 
            var filterBetaAppReviewSubmissionBetaReviewState = new List<string>?(); // List<string>? | filter by attribute 'betaAppReviewSubmission.betaReviewState' (optional) 
            var filterUsesNonExemptEncryption = new List<string>?(); // List<string>? | filter by attribute 'usesNonExemptEncryption' (optional) 
            var filterPreReleaseVersionVersion = new List<string>?(); // List<string>? | filter by attribute 'preReleaseVersion.version' (optional) 
            var filterPreReleaseVersionPlatform = new List<string>?(); // List<string>? | filter by attribute 'preReleaseVersion.platform' (optional) 
            var filterBuildAudienceType = new List<string>?(); // List<string>? | filter by attribute 'buildAudienceType' (optional) 
            var filterPreReleaseVersion = new List<string>?(); // List<string>? | filter by id(s) of related 'preReleaseVersion' (optional) 
            var filterApp = new List<string>?(); // List<string>? | filter by id(s) of related 'app' (optional) 
            var filterBetaGroups = new List<string>?(); // List<string>? | filter by id(s) of related 'betaGroups' (optional) 
            var filterAppStoreVersion = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersion' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var existsUsesNonExemptEncryption = true;  // bool? | filter by attribute 'usesNonExemptEncryption' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
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
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitIndividualTesters = 56;  // int? | maximum number of related individualTesters returned (when they are included) (optional) 
            var limitBetaGroups = 56;  // int? | maximum number of related betaGroups returned (when they are included) (optional) 
            var limitBetaBuildLocalizations = 56;  // int? | maximum number of related betaBuildLocalizations returned (when they are included) (optional) 
            var limitIcons = 56;  // int? | maximum number of related icons returned (when they are included) (optional) 
            var limitBuildBundles = 56;  // int? | maximum number of related buildBundles returned (when they are included) (optional) 

            try
            {
                BuildsResponse result = apiInstance.CiBuildRunsBuildsGetToManyRelated(id, filterVersion, filterExpired, filterProcessingState, filterBetaAppReviewSubmissionBetaReviewState, filterUsesNonExemptEncryption, filterPreReleaseVersionVersion, filterPreReleaseVersionPlatform, filterBuildAudienceType, filterPreReleaseVersion, filterApp, filterBetaGroups, filterAppStoreVersion, filterId, existsUsesNonExemptEncryption, sort, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaGroups, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, fieldsBuildBundles, fieldsBuildUploads, limit, include, limitIndividualTesters, limitBetaGroups, limitBetaBuildLocalizations, limitIcons, limitBuildBundles);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsBuildsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsBuildsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildsResponse> response = apiInstance.CiBuildRunsBuildsGetToManyRelatedWithHttpInfo(id, filterVersion, filterExpired, filterProcessingState, filterBetaAppReviewSubmissionBetaReviewState, filterUsesNonExemptEncryption, filterPreReleaseVersionVersion, filterPreReleaseVersionPlatform, filterBuildAudienceType, filterPreReleaseVersion, filterApp, filterBetaGroups, filterAppStoreVersion, filterId, existsUsesNonExemptEncryption, sort, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaGroups, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, fieldsBuildBundles, fieldsBuildUploads, limit, include, limitIndividualTesters, limitBetaGroups, limitBetaBuildLocalizations, limitIcons, limitBuildBundles);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsBuildsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterVersion** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterExpired** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;expired&#39; | [optional]  |
| **filterProcessingState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;processingState&#39; | [optional]  |
| **filterBetaAppReviewSubmissionBetaReviewState** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;betaAppReviewSubmission.betaReviewState&#39; | [optional]  |
| **filterUsesNonExemptEncryption** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **filterPreReleaseVersionVersion** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;preReleaseVersion.version&#39; | [optional]  |
| **filterPreReleaseVersionPlatform** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;preReleaseVersion.platform&#39; | [optional]  |
| **filterBuildAudienceType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;buildAudienceType&#39; | [optional]  |
| **filterPreReleaseVersion** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;preReleaseVersion&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBetaGroups** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;betaGroups&#39; | [optional]  |
| **filterAppStoreVersion** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appStoreVersion&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **existsUsesNonExemptEncryption** | **bool?** | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
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
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitIndividualTesters** | **int?** | maximum number of related individualTesters returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int?** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBetaBuildLocalizations** | **int?** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitIcons** | **int?** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int?** | maximum number of related buildBundles returned (when they are included) | [optional]  |

### Return type

[**BuildsResponse**](BuildsResponse.md)

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
| **200** | List of Builds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cibuildrunsbuildsgettomanyrelationship"></a>
# **CiBuildRunsBuildsGetToManyRelationship**
> CiBuildRunBuildsLinkagesResponse CiBuildRunsBuildsGetToManyRelationship (string id, int? limit = null)



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
    public class CiBuildRunsBuildsGetToManyRelationshipExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiBuildRunBuildsLinkagesResponse result = apiInstance.CiBuildRunsBuildsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsBuildsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsBuildsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunBuildsLinkagesResponse> response = apiInstance.CiBuildRunsBuildsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsBuildsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiBuildRunBuildsLinkagesResponse**](CiBuildRunBuildsLinkagesResponse.md)

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

<a id="cibuildrunscreateinstance"></a>
# **CiBuildRunsCreateInstance**
> CiBuildRunResponse CiBuildRunsCreateInstance (CiBuildRunCreateRequest ciBuildRunCreateRequest)



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
    public class CiBuildRunsCreateInstanceExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var ciBuildRunCreateRequest = new CiBuildRunCreateRequest(); // CiBuildRunCreateRequest | CiBuildRun representation

            try
            {
                CiBuildRunResponse result = apiInstance.CiBuildRunsCreateInstance(ciBuildRunCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunResponse> response = apiInstance.CiBuildRunsCreateInstanceWithHttpInfo(ciBuildRunCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **ciBuildRunCreateRequest** | [**CiBuildRunCreateRequest**](CiBuildRunCreateRequest.md) | CiBuildRun representation |  |

### Return type

[**CiBuildRunResponse**](CiBuildRunResponse.md)

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
| **201** | Single CiBuildRun |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="cibuildrunsgetinstance"></a>
# **CiBuildRunsGetInstance**
> CiBuildRunResponse CiBuildRunsGetInstance (string id, List<string>? fieldsCiBuildRuns = null, List<string>? fieldsBuilds = null, List<string>? include = null, int? limitBuilds = null)



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
    public class CiBuildRunsGetInstanceExample
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
            var apiInstance = new CiBuildRunsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiBuildRuns = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciBuildRuns (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                CiBuildRunResponse result = apiInstance.CiBuildRunsGetInstance(id, fieldsCiBuildRuns, fieldsBuilds, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiBuildRunsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunResponse> response = apiInstance.CiBuildRunsGetInstanceWithHttpInfo(id, fieldsCiBuildRuns, fieldsBuilds, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiBuildRunsApi.CiBuildRunsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**CiBuildRunResponse**](CiBuildRunResponse.md)

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
| **200** | Single CiBuildRun |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

