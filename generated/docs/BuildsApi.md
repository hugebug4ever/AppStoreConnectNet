# AppStoreConnect.Net.Api.BuildsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildsAppEncryptionDeclarationGetToOneRelated**](BuildsApi.md#buildsappencryptiondeclarationgettoonerelated) | **GET** /v1/builds/{id}/appEncryptionDeclaration |  |
| [**BuildsAppEncryptionDeclarationGetToOneRelationship**](BuildsApi.md#buildsappencryptiondeclarationgettoonerelationship) | **GET** /v1/builds/{id}/relationships/appEncryptionDeclaration |  |
| [**BuildsAppEncryptionDeclarationUpdateToOneRelationship**](BuildsApi.md#buildsappencryptiondeclarationupdatetoonerelationship) | **PATCH** /v1/builds/{id}/relationships/appEncryptionDeclaration |  |
| [**BuildsAppGetToOneRelated**](BuildsApi.md#buildsappgettoonerelated) | **GET** /v1/builds/{id}/app |  |
| [**BuildsAppGetToOneRelationship**](BuildsApi.md#buildsappgettoonerelationship) | **GET** /v1/builds/{id}/relationships/app |  |
| [**BuildsAppStoreVersionGetToOneRelated**](BuildsApi.md#buildsappstoreversiongettoonerelated) | **GET** /v1/builds/{id}/appStoreVersion |  |
| [**BuildsAppStoreVersionGetToOneRelationship**](BuildsApi.md#buildsappstoreversiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/appStoreVersion |  |
| [**BuildsBetaAppReviewSubmissionGetToOneRelated**](BuildsApi.md#buildsbetaappreviewsubmissiongettoonerelated) | **GET** /v1/builds/{id}/betaAppReviewSubmission |  |
| [**BuildsBetaAppReviewSubmissionGetToOneRelationship**](BuildsApi.md#buildsbetaappreviewsubmissiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/betaAppReviewSubmission |  |
| [**BuildsBetaBuildLocalizationsGetToManyRelated**](BuildsApi.md#buildsbetabuildlocalizationsgettomanyrelated) | **GET** /v1/builds/{id}/betaBuildLocalizations |  |
| [**BuildsBetaBuildLocalizationsGetToManyRelationship**](BuildsApi.md#buildsbetabuildlocalizationsgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/betaBuildLocalizations |  |
| [**BuildsBetaBuildUsagesGetMetrics**](BuildsApi.md#buildsbetabuildusagesgetmetrics) | **GET** /v1/builds/{id}/metrics/betaBuildUsages |  |
| [**BuildsBetaGroupsCreateToManyRelationship**](BuildsApi.md#buildsbetagroupscreatetomanyrelationship) | **POST** /v1/builds/{id}/relationships/betaGroups |  |
| [**BuildsBetaGroupsDeleteToManyRelationship**](BuildsApi.md#buildsbetagroupsdeletetomanyrelationship) | **DELETE** /v1/builds/{id}/relationships/betaGroups |  |
| [**BuildsBuildBetaDetailGetToOneRelated**](BuildsApi.md#buildsbuildbetadetailgettoonerelated) | **GET** /v1/builds/{id}/buildBetaDetail |  |
| [**BuildsBuildBetaDetailGetToOneRelationship**](BuildsApi.md#buildsbuildbetadetailgettoonerelationship) | **GET** /v1/builds/{id}/relationships/buildBetaDetail |  |
| [**BuildsDiagnosticSignaturesGetToManyRelated**](BuildsApi.md#buildsdiagnosticsignaturesgettomanyrelated) | **GET** /v1/builds/{id}/diagnosticSignatures |  |
| [**BuildsDiagnosticSignaturesGetToManyRelationship**](BuildsApi.md#buildsdiagnosticsignaturesgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/diagnosticSignatures |  |
| [**BuildsGetCollection**](BuildsApi.md#buildsgetcollection) | **GET** /v1/builds |  |
| [**BuildsGetInstance**](BuildsApi.md#buildsgetinstance) | **GET** /v1/builds/{id} |  |
| [**BuildsIconsGetToManyRelated**](BuildsApi.md#buildsiconsgettomanyrelated) | **GET** /v1/builds/{id}/icons |  |
| [**BuildsIconsGetToManyRelationship**](BuildsApi.md#buildsiconsgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/icons |  |
| [**BuildsIndividualTestersCreateToManyRelationship**](BuildsApi.md#buildsindividualtesterscreatetomanyrelationship) | **POST** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsIndividualTestersDeleteToManyRelationship**](BuildsApi.md#buildsindividualtestersdeletetomanyrelationship) | **DELETE** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsIndividualTestersGetToManyRelated**](BuildsApi.md#buildsindividualtestersgettomanyrelated) | **GET** /v1/builds/{id}/individualTesters |  |
| [**BuildsIndividualTestersGetToManyRelationship**](BuildsApi.md#buildsindividualtestersgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsPerfPowerMetricsGetToManyRelated**](BuildsApi.md#buildsperfpowermetricsgettomanyrelated) | **GET** /v1/builds/{id}/perfPowerMetrics |  |
| [**BuildsPreReleaseVersionGetToOneRelated**](BuildsApi.md#buildsprereleaseversiongettoonerelated) | **GET** /v1/builds/{id}/preReleaseVersion |  |
| [**BuildsPreReleaseVersionGetToOneRelationship**](BuildsApi.md#buildsprereleaseversiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/preReleaseVersion |  |
| [**BuildsUpdateInstance**](BuildsApi.md#buildsupdateinstance) | **PATCH** /v1/builds/{id} |  |

<a id="buildsappencryptiondeclarationgettoonerelated"></a>
# **BuildsAppEncryptionDeclarationGetToOneRelated**
> AppEncryptionDeclarationWithoutIncludesResponse BuildsAppEncryptionDeclarationGetToOneRelated (string id, List<string>? fieldsAppEncryptionDeclarations = null)



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
    public class BuildsAppEncryptionDeclarationGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 

            try
            {
                AppEncryptionDeclarationWithoutIncludesResponse result = apiInstance.BuildsAppEncryptionDeclarationGetToOneRelated(id, fieldsAppEncryptionDeclarations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppEncryptionDeclarationGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppEncryptionDeclarationWithoutIncludesResponse> response = apiInstance.BuildsAppEncryptionDeclarationGetToOneRelatedWithHttpInfo(id, fieldsAppEncryptionDeclarations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |

### Return type

[**AppEncryptionDeclarationWithoutIncludesResponse**](AppEncryptionDeclarationWithoutIncludesResponse.md)

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
| **200** | Single AppEncryptionDeclaration with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsappencryptiondeclarationgettoonerelationship"></a>
# **BuildsAppEncryptionDeclarationGetToOneRelationship**
> BuildAppEncryptionDeclarationLinkageResponse BuildsAppEncryptionDeclarationGetToOneRelationship (string id)



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
    public class BuildsAppEncryptionDeclarationGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildAppEncryptionDeclarationLinkageResponse result = apiInstance.BuildsAppEncryptionDeclarationGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppEncryptionDeclarationGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildAppEncryptionDeclarationLinkageResponse> response = apiInstance.BuildsAppEncryptionDeclarationGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppEncryptionDeclarationLinkageResponse**](BuildAppEncryptionDeclarationLinkageResponse.md)

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

<a id="buildsappencryptiondeclarationupdatetoonerelationship"></a>
# **BuildsAppEncryptionDeclarationUpdateToOneRelationship**
> void BuildsAppEncryptionDeclarationUpdateToOneRelationship (string id, BuildAppEncryptionDeclarationLinkageRequest buildAppEncryptionDeclarationLinkageRequest)



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
    public class BuildsAppEncryptionDeclarationUpdateToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildAppEncryptionDeclarationLinkageRequest = new BuildAppEncryptionDeclarationLinkageRequest(); // BuildAppEncryptionDeclarationLinkageRequest | Related linkage

            try
            {
                apiInstance.BuildsAppEncryptionDeclarationUpdateToOneRelationship(id, buildAppEncryptionDeclarationLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppEncryptionDeclarationUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BuildsAppEncryptionDeclarationUpdateToOneRelationshipWithHttpInfo(id, buildAppEncryptionDeclarationLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppEncryptionDeclarationUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildAppEncryptionDeclarationLinkageRequest** | [**BuildAppEncryptionDeclarationLinkageRequest**](BuildAppEncryptionDeclarationLinkageRequest.md) | Related linkage |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsappgettoonerelated"></a>
# **BuildsAppGetToOneRelated**
> AppWithoutIncludesResponse BuildsAppGetToOneRelated (string id, List<string>? fieldsApps = null)



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
    public class BuildsAppGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 

            try
            {
                AppWithoutIncludesResponse result = apiInstance.BuildsAppGetToOneRelated(id, fieldsApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppWithoutIncludesResponse> response = apiInstance.BuildsAppGetToOneRelatedWithHttpInfo(id, fieldsApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="buildsappgettoonerelationship"></a>
# **BuildsAppGetToOneRelationship**
> BuildAppLinkageResponse BuildsAppGetToOneRelationship (string id)



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
    public class BuildsAppGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildAppLinkageResponse result = apiInstance.BuildsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildAppLinkageResponse> response = apiInstance.BuildsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppLinkageResponse**](BuildAppLinkageResponse.md)

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

<a id="buildsappstoreversiongettoonerelated"></a>
# **BuildsAppStoreVersionGetToOneRelated**
> AppStoreVersionResponse BuildsAppStoreVersionGetToOneRelated (string id, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsApps = null, List<string>? fieldsAgeRatingDeclarations = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsBuilds = null, List<string>? fieldsAppStoreVersionPhasedReleases = null, List<string>? fieldsGameCenterAppVersions = null, List<string>? fieldsRoutingAppCoverages = null, List<string>? fieldsAppStoreReviewDetails = null, List<string>? fieldsAppStoreVersionSubmissions = null, List<string>? fieldsAppClipDefaultExperiences = null, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAlternativeDistributionPackages = null, List<string>? include = null, int? limitAppStoreVersionLocalizations = null, int? limitAppStoreVersionExperiments = null, int? limitAppStoreVersionExperimentsV2 = null)



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
    public class BuildsAppStoreVersionGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsAgeRatingDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type ageRatingDeclarations (optional) 
            var fieldsAppStoreVersionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionLocalizations (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsAppStoreVersionPhasedReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionPhasedReleases (optional) 
            var fieldsGameCenterAppVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAppVersions (optional) 
            var fieldsRoutingAppCoverages = new List<string>?(); // List<string>? | the fields to include for returned resources of type routingAppCoverages (optional) 
            var fieldsAppStoreReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreReviewDetails (optional) 
            var fieldsAppStoreVersionSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionSubmissions (optional) 
            var fieldsAppClipDefaultExperiences = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDefaultExperiences (optional) 
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAlternativeDistributionPackages = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionLocalizations = 56;  // int? | maximum number of related appStoreVersionLocalizations returned (when they are included) (optional) 
            var limitAppStoreVersionExperiments = 56;  // int? | maximum number of related appStoreVersionExperiments returned (when they are included) (optional) 
            var limitAppStoreVersionExperimentsV2 = 56;  // int? | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional) 

            try
            {
                AppStoreVersionResponse result = apiInstance.BuildsAppStoreVersionGetToOneRelated(id, fieldsAppStoreVersions, fieldsApps, fieldsAgeRatingDeclarations, fieldsAppStoreVersionLocalizations, fieldsBuilds, fieldsAppStoreVersionPhasedReleases, fieldsGameCenterAppVersions, fieldsRoutingAppCoverages, fieldsAppStoreReviewDetails, fieldsAppStoreVersionSubmissions, fieldsAppClipDefaultExperiences, fieldsAppStoreVersionExperiments, fieldsAlternativeDistributionPackages, include, limitAppStoreVersionLocalizations, limitAppStoreVersionExperiments, limitAppStoreVersionExperimentsV2);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppStoreVersionGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppStoreVersionGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionResponse> response = apiInstance.BuildsAppStoreVersionGetToOneRelatedWithHttpInfo(id, fieldsAppStoreVersions, fieldsApps, fieldsAgeRatingDeclarations, fieldsAppStoreVersionLocalizations, fieldsBuilds, fieldsAppStoreVersionPhasedReleases, fieldsGameCenterAppVersions, fieldsRoutingAppCoverages, fieldsAppStoreReviewDetails, fieldsAppStoreVersionSubmissions, fieldsAppClipDefaultExperiences, fieldsAppStoreVersionExperiments, fieldsAlternativeDistributionPackages, include, limitAppStoreVersionLocalizations, limitAppStoreVersionExperiments, limitAppStoreVersionExperimentsV2);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppStoreVersionGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsAppStoreVersionPhasedReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsRoutingAppCoverages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type routingAppCoverages | [optional]  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **fieldsAppStoreVersionSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionSubmissions | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionLocalizations** | **int?** | maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperiments** | **int?** | maximum number of related appStoreVersionExperiments returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int?** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
| **200** | Single AppStoreVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsappstoreversiongettoonerelationship"></a>
# **BuildsAppStoreVersionGetToOneRelationship**
> BuildAppStoreVersionLinkageResponse BuildsAppStoreVersionGetToOneRelationship (string id)



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
    public class BuildsAppStoreVersionGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildAppStoreVersionLinkageResponse result = apiInstance.BuildsAppStoreVersionGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsAppStoreVersionGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsAppStoreVersionGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildAppStoreVersionLinkageResponse> response = apiInstance.BuildsAppStoreVersionGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsAppStoreVersionGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppStoreVersionLinkageResponse**](BuildAppStoreVersionLinkageResponse.md)

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

<a id="buildsbetaappreviewsubmissiongettoonerelated"></a>
# **BuildsBetaAppReviewSubmissionGetToOneRelated**
> BetaAppReviewSubmissionWithoutIncludesResponse BuildsBetaAppReviewSubmissionGetToOneRelated (string id, List<string>? fieldsBetaAppReviewSubmissions = null)



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
    public class BuildsBetaAppReviewSubmissionGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 

            try
            {
                BetaAppReviewSubmissionWithoutIncludesResponse result = apiInstance.BuildsBetaAppReviewSubmissionGetToOneRelated(id, fieldsBetaAppReviewSubmissions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaAppReviewSubmissionGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaAppReviewSubmissionGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaAppReviewSubmissionWithoutIncludesResponse> response = apiInstance.BuildsBetaAppReviewSubmissionGetToOneRelatedWithHttpInfo(id, fieldsBetaAppReviewSubmissions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaAppReviewSubmissionGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |

### Return type

[**BetaAppReviewSubmissionWithoutIncludesResponse**](BetaAppReviewSubmissionWithoutIncludesResponse.md)

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
| **200** | Single BetaAppReviewSubmission with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsbetaappreviewsubmissiongettoonerelationship"></a>
# **BuildsBetaAppReviewSubmissionGetToOneRelationship**
> BuildBetaAppReviewSubmissionLinkageResponse BuildsBetaAppReviewSubmissionGetToOneRelationship (string id)



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
    public class BuildsBetaAppReviewSubmissionGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildBetaAppReviewSubmissionLinkageResponse result = apiInstance.BuildsBetaAppReviewSubmissionGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaAppReviewSubmissionGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaAppReviewSubmissionGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaAppReviewSubmissionLinkageResponse> response = apiInstance.BuildsBetaAppReviewSubmissionGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaAppReviewSubmissionGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBetaAppReviewSubmissionLinkageResponse**](BuildBetaAppReviewSubmissionLinkageResponse.md)

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

<a id="buildsbetabuildlocalizationsgettomanyrelated"></a>
# **BuildsBetaBuildLocalizationsGetToManyRelated**
> BetaBuildLocalizationsWithoutIncludesResponse BuildsBetaBuildLocalizationsGetToManyRelated (string id, List<string>? fieldsBetaBuildLocalizations = null, int? limit = null)



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
    public class BuildsBetaBuildLocalizationsGetToManyRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BetaBuildLocalizationsWithoutIncludesResponse result = apiInstance.BuildsBetaBuildLocalizationsGetToManyRelated(id, fieldsBetaBuildLocalizations, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaBuildLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationsWithoutIncludesResponse> response = apiInstance.BuildsBetaBuildLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsBetaBuildLocalizations, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BetaBuildLocalizationsWithoutIncludesResponse**](BetaBuildLocalizationsWithoutIncludesResponse.md)

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
| **200** | List of BetaBuildLocalizations with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsbetabuildlocalizationsgettomanyrelationship"></a>
# **BuildsBetaBuildLocalizationsGetToManyRelationship**
> BuildBetaBuildLocalizationsLinkagesResponse BuildsBetaBuildLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class BuildsBetaBuildLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildBetaBuildLocalizationsLinkagesResponse result = apiInstance.BuildsBetaBuildLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaBuildLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaBuildLocalizationsLinkagesResponse> response = apiInstance.BuildsBetaBuildLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildBetaBuildLocalizationsLinkagesResponse**](BuildBetaBuildLocalizationsLinkagesResponse.md)

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

<a id="buildsbetabuildusagesgetmetrics"></a>
# **BuildsBetaBuildUsagesGetMetrics**
> BetaBuildUsagesV1MetricResponse BuildsBetaBuildUsagesGetMetrics (string id, int? limit = null)



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
    public class BuildsBetaBuildUsagesGetMetricsExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                BetaBuildUsagesV1MetricResponse result = apiInstance.BuildsBetaBuildUsagesGetMetrics(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaBuildUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildUsagesV1MetricResponse> response = apiInstance.BuildsBetaBuildUsagesGetMetricsWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaBuildUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaBuildUsagesV1MetricResponse**](BetaBuildUsagesV1MetricResponse.md)

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
| **200** | Metrics data response |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsbetagroupscreatetomanyrelationship"></a>
# **BuildsBetaGroupsCreateToManyRelationship**
> void BuildsBetaGroupsCreateToManyRelationship (string id, BuildBetaGroupsLinkagesRequest buildBetaGroupsLinkagesRequest)



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
    public class BuildsBetaGroupsCreateToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildBetaGroupsLinkagesRequest = new BuildBetaGroupsLinkagesRequest(); // BuildBetaGroupsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BuildsBetaGroupsCreateToManyRelationship(id, buildBetaGroupsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaGroupsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaGroupsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BuildsBetaGroupsCreateToManyRelationshipWithHttpInfo(id, buildBetaGroupsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaGroupsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaGroupsLinkagesRequest** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsbetagroupsdeletetomanyrelationship"></a>
# **BuildsBetaGroupsDeleteToManyRelationship**
> void BuildsBetaGroupsDeleteToManyRelationship (string id, BuildBetaGroupsLinkagesRequest buildBetaGroupsLinkagesRequest)



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
    public class BuildsBetaGroupsDeleteToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildBetaGroupsLinkagesRequest = new BuildBetaGroupsLinkagesRequest(); // BuildBetaGroupsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BuildsBetaGroupsDeleteToManyRelationship(id, buildBetaGroupsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBetaGroupsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaGroupsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BuildsBetaGroupsDeleteToManyRelationshipWithHttpInfo(id, buildBetaGroupsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBetaGroupsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaGroupsLinkagesRequest** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsbuildbetadetailgettoonerelated"></a>
# **BuildsBuildBetaDetailGetToOneRelated**
> BuildBetaDetailResponse BuildsBuildBetaDetailGetToOneRelated (string id, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsBuilds = null, List<string>? include = null)



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
    public class BuildsBuildBetaDetailGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BuildBetaDetailResponse result = apiInstance.BuildsBuildBetaDetailGetToOneRelated(id, fieldsBuildBetaDetails, fieldsBuilds, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBuildBetaDetailGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBuildBetaDetailGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBetaDetailResponse> response = apiInstance.BuildsBuildBetaDetailGetToOneRelatedWithHttpInfo(id, fieldsBuildBetaDetails, fieldsBuilds, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBuildBetaDetailGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="buildsbuildbetadetailgettoonerelationship"></a>
# **BuildsBuildBetaDetailGetToOneRelationship**
> BuildBuildBetaDetailLinkageResponse BuildsBuildBetaDetailGetToOneRelationship (string id)



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
    public class BuildsBuildBetaDetailGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildBuildBetaDetailLinkageResponse result = apiInstance.BuildsBuildBetaDetailGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsBuildBetaDetailGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBuildBetaDetailGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildBuildBetaDetailLinkageResponse> response = apiInstance.BuildsBuildBetaDetailGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsBuildBetaDetailGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBuildBetaDetailLinkageResponse**](BuildBuildBetaDetailLinkageResponse.md)

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

<a id="buildsdiagnosticsignaturesgettomanyrelated"></a>
# **BuildsDiagnosticSignaturesGetToManyRelated**
> DiagnosticSignaturesResponse BuildsDiagnosticSignaturesGetToManyRelated (string id, List<string>? filterDiagnosticType = null, List<string>? fieldsDiagnosticSignatures = null, int? limit = null)



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
    public class BuildsDiagnosticSignaturesGetToManyRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterDiagnosticType = new List<string>?(); // List<string>? | filter by attribute 'diagnosticType' (optional) 
            var fieldsDiagnosticSignatures = new List<string>?(); // List<string>? | the fields to include for returned resources of type diagnosticSignatures (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                DiagnosticSignaturesResponse result = apiInstance.BuildsDiagnosticSignaturesGetToManyRelated(id, filterDiagnosticType, fieldsDiagnosticSignatures, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsDiagnosticSignaturesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsDiagnosticSignaturesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<DiagnosticSignaturesResponse> response = apiInstance.BuildsDiagnosticSignaturesGetToManyRelatedWithHttpInfo(id, filterDiagnosticType, fieldsDiagnosticSignatures, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsDiagnosticSignaturesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterDiagnosticType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;diagnosticType&#39; | [optional]  |
| **fieldsDiagnosticSignatures** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type diagnosticSignatures | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**DiagnosticSignaturesResponse**](DiagnosticSignaturesResponse.md)

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
| **200** | List of DiagnosticSignatures |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsdiagnosticsignaturesgettomanyrelationship"></a>
# **BuildsDiagnosticSignaturesGetToManyRelationship**
> BuildDiagnosticSignaturesLinkagesResponse BuildsDiagnosticSignaturesGetToManyRelationship (string id, int? limit = null)



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
    public class BuildsDiagnosticSignaturesGetToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildDiagnosticSignaturesLinkagesResponse result = apiInstance.BuildsDiagnosticSignaturesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsDiagnosticSignaturesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsDiagnosticSignaturesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildDiagnosticSignaturesLinkagesResponse> response = apiInstance.BuildsDiagnosticSignaturesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsDiagnosticSignaturesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildDiagnosticSignaturesLinkagesResponse**](BuildDiagnosticSignaturesLinkagesResponse.md)

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

<a id="buildsgetcollection"></a>
# **BuildsGetCollection**
> BuildsResponse BuildsGetCollection (List<string>? filterVersion = null, List<string>? filterExpired = null, List<string>? filterProcessingState = null, List<string>? filterBetaAppReviewSubmissionBetaReviewState = null, List<string>? filterUsesNonExemptEncryption = null, List<string>? filterPreReleaseVersionVersion = null, List<string>? filterPreReleaseVersionPlatform = null, List<string>? filterBuildAudienceType = null, List<string>? filterPreReleaseVersion = null, List<string>? filterApp = null, List<string>? filterBetaGroups = null, List<string>? filterAppStoreVersion = null, List<string>? filterId = null, bool? existsUsesNonExemptEncryption = null, List<string>? sort = null, List<string>? fieldsBuilds = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsApps = null, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsBuildIcons = null, int? limit = null, List<string>? include = null, int? limitBetaBuildLocalizations = null, int? limitBetaGroups = null, int? limitBuildBundles = null, int? limitIcons = null, int? limitIndividualTesters = null)



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
    public class BuildsGetCollectionExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
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
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsBuildIcons = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildIcons (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBetaBuildLocalizations = 56;  // int? | maximum number of related betaBuildLocalizations returned (when they are included) (optional) 
            var limitBetaGroups = 56;  // int? | maximum number of related betaGroups returned (when they are included) (optional) 
            var limitBuildBundles = 56;  // int? | maximum number of related buildBundles returned (when they are included) (optional) 
            var limitIcons = 56;  // int? | maximum number of related icons returned (when they are included) (optional) 
            var limitIndividualTesters = 56;  // int? | maximum number of related individualTesters returned (when they are included) (optional) 

            try
            {
                BuildsResponse result = apiInstance.BuildsGetCollection(filterVersion, filterExpired, filterProcessingState, filterBetaAppReviewSubmissionBetaReviewState, filterUsesNonExemptEncryption, filterPreReleaseVersionVersion, filterPreReleaseVersionPlatform, filterBuildAudienceType, filterPreReleaseVersion, filterApp, filterBetaGroups, filterAppStoreVersion, filterId, existsUsesNonExemptEncryption, sort, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, limit, include, limitBetaBuildLocalizations, limitBetaGroups, limitBuildBundles, limitIcons, limitIndividualTesters);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildsResponse> response = apiInstance.BuildsGetCollectionWithHttpInfo(filterVersion, filterExpired, filterProcessingState, filterBetaAppReviewSubmissionBetaReviewState, filterUsesNonExemptEncryption, filterPreReleaseVersionVersion, filterPreReleaseVersionPlatform, filterBuildAudienceType, filterPreReleaseVersion, filterApp, filterBetaGroups, filterAppStoreVersion, filterId, existsUsesNonExemptEncryption, sort, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, limit, include, limitBetaBuildLocalizations, limitBetaGroups, limitBuildBundles, limitIcons, limitIndividualTesters);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
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
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaBuildLocalizations** | **int?** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int?** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int?** | maximum number of related buildBundles returned (when they are included) | [optional]  |
| **limitIcons** | **int?** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitIndividualTesters** | **int?** | maximum number of related individualTesters returned (when they are included) | [optional]  |

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
| **200** | List of Builds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsgetinstance"></a>
# **BuildsGetInstance**
> BuildResponse BuildsGetInstance (string id, List<string>? fieldsBuilds = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsBetaAppReviewSubmissions = null, List<string>? fieldsApps = null, List<string>? fieldsBuildBetaDetails = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsBuildIcons = null, List<string>? include = null, int? limitBetaBuildLocalizations = null, int? limitBetaGroups = null, int? limitBuildBundles = null, int? limitIcons = null, int? limitIndividualTesters = null)



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
    public class BuildsGetInstanceExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsBetaAppReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewSubmissions (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsBuildBetaDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildBetaDetails (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsBuildIcons = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildIcons (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBetaBuildLocalizations = 56;  // int? | maximum number of related betaBuildLocalizations returned (when they are included) (optional) 
            var limitBetaGroups = 56;  // int? | maximum number of related betaGroups returned (when they are included) (optional) 
            var limitBuildBundles = 56;  // int? | maximum number of related buildBundles returned (when they are included) (optional) 
            var limitIcons = 56;  // int? | maximum number of related icons returned (when they are included) (optional) 
            var limitIndividualTesters = 56;  // int? | maximum number of related individualTesters returned (when they are included) (optional) 

            try
            {
                BuildResponse result = apiInstance.BuildsGetInstance(id, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, include, limitBetaBuildLocalizations, limitBetaGroups, limitBuildBundles, limitIcons, limitIndividualTesters);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildResponse> response = apiInstance.BuildsGetInstanceWithHttpInfo(id, fieldsBuilds, fieldsPreReleaseVersions, fieldsBetaTesters, fieldsBetaBuildLocalizations, fieldsAppEncryptionDeclarations, fieldsBetaAppReviewSubmissions, fieldsApps, fieldsBuildBetaDetails, fieldsAppStoreVersions, fieldsBuildIcons, include, limitBetaBuildLocalizations, limitBetaGroups, limitBuildBundles, limitIcons, limitIndividualTesters);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsGetInstanceWithHttpInfo: " + e.Message);
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
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaBuildLocalizations** | **int?** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int?** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int?** | maximum number of related buildBundles returned (when they are included) | [optional]  |
| **limitIcons** | **int?** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitIndividualTesters** | **int?** | maximum number of related individualTesters returned (when they are included) | [optional]  |

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

<a id="buildsiconsgettomanyrelated"></a>
# **BuildsIconsGetToManyRelated**
> BuildIconsWithoutIncludesResponse BuildsIconsGetToManyRelated (string id, List<string>? fieldsBuildIcons = null, int? limit = null)



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
    public class BuildsIconsGetToManyRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuildIcons = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildIcons (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildIconsWithoutIncludesResponse result = apiInstance.BuildsIconsGetToManyRelated(id, fieldsBuildIcons, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIconsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIconsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildIconsWithoutIncludesResponse> response = apiInstance.BuildsIconsGetToManyRelatedWithHttpInfo(id, fieldsBuildIcons, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIconsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildIcons** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BuildIconsWithoutIncludesResponse**](BuildIconsWithoutIncludesResponse.md)

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
| **200** | List of BuildIcons with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsiconsgettomanyrelationship"></a>
# **BuildsIconsGetToManyRelationship**
> BuildIconsLinkagesResponse BuildsIconsGetToManyRelationship (string id, int? limit = null)



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
    public class BuildsIconsGetToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildIconsLinkagesResponse result = apiInstance.BuildsIconsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIconsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIconsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildIconsLinkagesResponse> response = apiInstance.BuildsIconsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIconsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildIconsLinkagesResponse**](BuildIconsLinkagesResponse.md)

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

<a id="buildsindividualtesterscreatetomanyrelationship"></a>
# **BuildsIndividualTestersCreateToManyRelationship**
> void BuildsIndividualTestersCreateToManyRelationship (string id, BuildIndividualTestersLinkagesRequest buildIndividualTestersLinkagesRequest)



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
    public class BuildsIndividualTestersCreateToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildIndividualTestersLinkagesRequest = new BuildIndividualTestersLinkagesRequest(); // BuildIndividualTestersLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BuildsIndividualTestersCreateToManyRelationship(id, buildIndividualTestersLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIndividualTestersCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BuildsIndividualTestersCreateToManyRelationshipWithHttpInfo(id, buildIndividualTestersLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildIndividualTestersLinkagesRequest** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsindividualtestersdeletetomanyrelationship"></a>
# **BuildsIndividualTestersDeleteToManyRelationship**
> void BuildsIndividualTestersDeleteToManyRelationship (string id, BuildIndividualTestersLinkagesRequest buildIndividualTestersLinkagesRequest)



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
    public class BuildsIndividualTestersDeleteToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildIndividualTestersLinkagesRequest = new BuildIndividualTestersLinkagesRequest(); // BuildIndividualTestersLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BuildsIndividualTestersDeleteToManyRelationship(id, buildIndividualTestersLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIndividualTestersDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BuildsIndividualTestersDeleteToManyRelationshipWithHttpInfo(id, buildIndividualTestersLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildIndividualTestersLinkagesRequest** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsindividualtestersgettomanyrelated"></a>
# **BuildsIndividualTestersGetToManyRelated**
> BetaTestersWithoutIncludesResponse BuildsIndividualTestersGetToManyRelated (string id, List<string>? fieldsBetaTesters = null, int? limit = null)



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
    public class BuildsIndividualTestersGetToManyRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BetaTestersWithoutIncludesResponse result = apiInstance.BuildsIndividualTestersGetToManyRelated(id, fieldsBetaTesters, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIndividualTestersGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaTestersWithoutIncludesResponse> response = apiInstance.BuildsIndividualTestersGetToManyRelatedWithHttpInfo(id, fieldsBetaTesters, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaTesters** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BetaTestersWithoutIncludesResponse**](BetaTestersWithoutIncludesResponse.md)

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
| **200** | List of BetaTesters with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsindividualtestersgettomanyrelationship"></a>
# **BuildsIndividualTestersGetToManyRelationship**
> BuildIndividualTestersLinkagesResponse BuildsIndividualTestersGetToManyRelationship (string id, int? limit = null)



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
    public class BuildsIndividualTestersGetToManyRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildIndividualTestersLinkagesResponse result = apiInstance.BuildsIndividualTestersGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsIndividualTestersGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildIndividualTestersLinkagesResponse> response = apiInstance.BuildsIndividualTestersGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsIndividualTestersGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BuildIndividualTestersLinkagesResponse**](BuildIndividualTestersLinkagesResponse.md)

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

<a id="buildsperfpowermetricsgettomanyrelated"></a>
# **BuildsPerfPowerMetricsGetToManyRelated**
> XcodeMetrics BuildsPerfPowerMetricsGetToManyRelated (string id, List<string>? filterPlatform = null, List<string>? filterMetricType = null, List<string>? filterDeviceType = null)



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
    public class BuildsPerfPowerMetricsGetToManyRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPlatform = new List<string>?(); // List<string>? | filter by attribute 'platform' (optional) 
            var filterMetricType = new List<string>?(); // List<string>? | filter by attribute 'metricType' (optional) 
            var filterDeviceType = new List<string>?(); // List<string>? | filter by attribute 'deviceType' (optional) 

            try
            {
                XcodeMetrics result = apiInstance.BuildsPerfPowerMetricsGetToManyRelated(id, filterPlatform, filterMetricType, filterDeviceType);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsPerfPowerMetricsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsPerfPowerMetricsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<XcodeMetrics> response = apiInstance.BuildsPerfPowerMetricsGetToManyRelatedWithHttpInfo(id, filterPlatform, filterMetricType, filterDeviceType);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsPerfPowerMetricsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPlatform** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterMetricType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;metricType&#39; | [optional]  |
| **filterDeviceType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;deviceType&#39; | [optional]  |

### Return type

[**XcodeMetrics**](XcodeMetrics.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/vnd.apple.xcode-metrics+json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of PerfPowerMetrics |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsprereleaseversiongettoonerelated"></a>
# **BuildsPreReleaseVersionGetToOneRelated**
> PrereleaseVersionWithoutIncludesResponse BuildsPreReleaseVersionGetToOneRelated (string id, List<string>? fieldsPreReleaseVersions = null)



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
    public class BuildsPreReleaseVersionGetToOneRelatedExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 

            try
            {
                PrereleaseVersionWithoutIncludesResponse result = apiInstance.BuildsPreReleaseVersionGetToOneRelated(id, fieldsPreReleaseVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsPreReleaseVersionGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsPreReleaseVersionGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PrereleaseVersionWithoutIncludesResponse> response = apiInstance.BuildsPreReleaseVersionGetToOneRelatedWithHttpInfo(id, fieldsPreReleaseVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsPreReleaseVersionGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |

### Return type

[**PrereleaseVersionWithoutIncludesResponse**](PrereleaseVersionWithoutIncludesResponse.md)

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
| **200** | Single PrereleaseVersion with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="buildsprereleaseversiongettoonerelationship"></a>
# **BuildsPreReleaseVersionGetToOneRelationship**
> BuildPreReleaseVersionLinkageResponse BuildsPreReleaseVersionGetToOneRelationship (string id)



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
    public class BuildsPreReleaseVersionGetToOneRelationshipExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BuildPreReleaseVersionLinkageResponse result = apiInstance.BuildsPreReleaseVersionGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsPreReleaseVersionGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsPreReleaseVersionGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildPreReleaseVersionLinkageResponse> response = apiInstance.BuildsPreReleaseVersionGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsPreReleaseVersionGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildPreReleaseVersionLinkageResponse**](BuildPreReleaseVersionLinkageResponse.md)

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

<a id="buildsupdateinstance"></a>
# **BuildsUpdateInstance**
> BuildResponse BuildsUpdateInstance (string id, BuildUpdateRequest buildUpdateRequest)



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
    public class BuildsUpdateInstanceExample
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
            var apiInstance = new BuildsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var buildUpdateRequest = new BuildUpdateRequest(); // BuildUpdateRequest | Build representation

            try
            {
                BuildResponse result = apiInstance.BuildsUpdateInstance(id, buildUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BuildsApi.BuildsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildResponse> response = apiInstance.BuildsUpdateInstanceWithHttpInfo(id, buildUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BuildsApi.BuildsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildUpdateRequest** | [**BuildUpdateRequest**](BuildUpdateRequest.md) | Build representation |  |

### Return type

[**BuildResponse**](BuildResponse.md)

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
| **200** | Single Build |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

