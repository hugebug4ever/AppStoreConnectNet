# AppStoreConnect.Net.Api.CiProductsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiProductsAdditionalRepositoriesGetToManyRelated**](CiProductsApi.md#ciproductsadditionalrepositoriesgettomanyrelated) | **GET** /v1/ciProducts/{id}/additionalRepositories |  |
| [**CiProductsAdditionalRepositoriesGetToManyRelationship**](CiProductsApi.md#ciproductsadditionalrepositoriesgettomanyrelationship) | **GET** /v1/ciProducts/{id}/relationships/additionalRepositories |  |
| [**CiProductsAppGetToOneRelated**](CiProductsApi.md#ciproductsappgettoonerelated) | **GET** /v1/ciProducts/{id}/app |  |
| [**CiProductsAppGetToOneRelationship**](CiProductsApi.md#ciproductsappgettoonerelationship) | **GET** /v1/ciProducts/{id}/relationships/app |  |
| [**CiProductsBuildRunsGetToManyRelated**](CiProductsApi.md#ciproductsbuildrunsgettomanyrelated) | **GET** /v1/ciProducts/{id}/buildRuns |  |
| [**CiProductsBuildRunsGetToManyRelationship**](CiProductsApi.md#ciproductsbuildrunsgettomanyrelationship) | **GET** /v1/ciProducts/{id}/relationships/buildRuns |  |
| [**CiProductsDeleteInstance**](CiProductsApi.md#ciproductsdeleteinstance) | **DELETE** /v1/ciProducts/{id} |  |
| [**CiProductsGetCollection**](CiProductsApi.md#ciproductsgetcollection) | **GET** /v1/ciProducts |  |
| [**CiProductsGetInstance**](CiProductsApi.md#ciproductsgetinstance) | **GET** /v1/ciProducts/{id} |  |
| [**CiProductsPrimaryRepositoriesGetToManyRelated**](CiProductsApi.md#ciproductsprimaryrepositoriesgettomanyrelated) | **GET** /v1/ciProducts/{id}/primaryRepositories |  |
| [**CiProductsPrimaryRepositoriesGetToManyRelationship**](CiProductsApi.md#ciproductsprimaryrepositoriesgettomanyrelationship) | **GET** /v1/ciProducts/{id}/relationships/primaryRepositories |  |
| [**CiProductsWorkflowsGetToManyRelated**](CiProductsApi.md#ciproductsworkflowsgettomanyrelated) | **GET** /v1/ciProducts/{id}/workflows |  |
| [**CiProductsWorkflowsGetToManyRelationship**](CiProductsApi.md#ciproductsworkflowsgettomanyrelationship) | **GET** /v1/ciProducts/{id}/relationships/workflows |  |

<a id="ciproductsadditionalrepositoriesgettomanyrelated"></a>
# **CiProductsAdditionalRepositoriesGetToManyRelated**
> ScmRepositoriesResponse CiProductsAdditionalRepositoriesGetToManyRelated (string id, List<string>? filterId = null, List<string>? fieldsScmRepositories = null, List<string>? fieldsScmProviders = null, List<string>? fieldsScmGitReferences = null, int? limit = null, List<string>? include = null)



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
    public class CiProductsAdditionalRepositoriesGetToManyRelatedExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var fieldsScmProviders = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmProviders (optional) 
            var fieldsScmGitReferences = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmGitReferences (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                ScmRepositoriesResponse result = apiInstance.CiProductsAdditionalRepositoriesGetToManyRelated(id, filterId, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsAdditionalRepositoriesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsAdditionalRepositoriesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<ScmRepositoriesResponse> response = apiInstance.CiProductsAdditionalRepositoriesGetToManyRelatedWithHttpInfo(id, filterId, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsAdditionalRepositoriesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmRepositoriesResponse**](ScmRepositoriesResponse.md)

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
| **200** | List of ScmRepositories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsadditionalrepositoriesgettomanyrelationship"></a>
# **CiProductsAdditionalRepositoriesGetToManyRelationship**
> CiProductAdditionalRepositoriesLinkagesResponse CiProductsAdditionalRepositoriesGetToManyRelationship (string id, int? limit = null)



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
    public class CiProductsAdditionalRepositoriesGetToManyRelationshipExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiProductAdditionalRepositoriesLinkagesResponse result = apiInstance.CiProductsAdditionalRepositoriesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsAdditionalRepositoriesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsAdditionalRepositoriesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductAdditionalRepositoriesLinkagesResponse> response = apiInstance.CiProductsAdditionalRepositoriesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsAdditionalRepositoriesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiProductAdditionalRepositoriesLinkagesResponse**](CiProductAdditionalRepositoriesLinkagesResponse.md)

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

<a id="ciproductsappgettoonerelated"></a>
# **CiProductsAppGetToOneRelated**
> AppResponse CiProductsAppGetToOneRelated (string id, List<string>? fieldsApps = null, List<string>? fieldsAppEncryptionDeclarations = null, List<string>? fieldsBuildIcons = null, List<string>? fieldsCiProducts = null, List<string>? fieldsBetaGroups = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsPreReleaseVersions = null, List<string>? fieldsBetaAppLocalizations = null, List<string>? fieldsBuilds = null, List<string>? fieldsBetaLicenseAgreements = null, List<string>? fieldsBetaAppReviewDetails = null, List<string>? fieldsAppInfos = null, List<string>? fieldsAppClips = null, List<string>? fieldsEndUserLicenseAgreements = null, List<string>? fieldsInAppPurchases = null, List<string>? fieldsSubscriptionGroups = null, List<string>? fieldsGameCenterEnabledVersions = null, List<string>? fieldsAppCustomProductPages = null, List<string>? fieldsPromotedPurchases = null, List<string>? fieldsAppEvents = null, List<string>? fieldsReviewSubmissions = null, List<string>? fieldsSubscriptionGracePeriods = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAndroidToIosAppMappingDetails = null, List<string>? include = null, int? limitAppEncryptionDeclarations = null, int? limitBetaGroups = null, int? limitAppStoreVersions = null, int? limitPreReleaseVersions = null, int? limitBetaAppLocalizations = null, int? limitBuilds = null, int? limitAppInfos = null, int? limitAppClips = null, int? limitInAppPurchases = null, int? limitSubscriptionGroups = null, int? limitGameCenterEnabledVersions = null, int? limitAppCustomProductPages = null, int? limitInAppPurchasesV2 = null, int? limitPromotedPurchases = null, int? limitAppEvents = null, int? limitReviewSubmissions = null, int? limitAppStoreVersionExperimentsV2 = null, int? limitAndroidToIosAppMappingDetails = null)



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
    public class CiProductsAppGetToOneRelatedExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsAppEncryptionDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEncryptionDeclarations (optional) 
            var fieldsBuildIcons = new List<string>?(); // List<string>? | the fields to include for returned resources of type buildIcons (optional) 
            var fieldsCiProducts = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciProducts (optional) 
            var fieldsBetaGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaGroups (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsPreReleaseVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type preReleaseVersions (optional) 
            var fieldsBetaAppLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppLocalizations (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsBetaLicenseAgreements = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaLicenseAgreements (optional) 
            var fieldsBetaAppReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaAppReviewDetails (optional) 
            var fieldsAppInfos = new List<string>?(); // List<string>? | the fields to include for returned resources of type appInfos (optional) 
            var fieldsAppClips = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClips (optional) 
            var fieldsEndUserLicenseAgreements = new List<string>?(); // List<string>? | the fields to include for returned resources of type endUserLicenseAgreements (optional) 
            var fieldsInAppPurchases = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchases (optional) 
            var fieldsSubscriptionGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionGroups (optional) 
            var fieldsGameCenterEnabledVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterEnabledVersions (optional) 
            var fieldsAppCustomProductPages = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPages (optional) 
            var fieldsPromotedPurchases = new List<string>?(); // List<string>? | the fields to include for returned resources of type promotedPurchases (optional) 
            var fieldsAppEvents = new List<string>?(); // List<string>? | the fields to include for returned resources of type appEvents (optional) 
            var fieldsReviewSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type reviewSubmissions (optional) 
            var fieldsSubscriptionGracePeriods = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionGracePeriods (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAndroidToIosAppMappingDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type androidToIosAppMappingDetails (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppEncryptionDeclarations = 56;  // int? | maximum number of related appEncryptionDeclarations returned (when they are included) (optional) 
            var limitBetaGroups = 56;  // int? | maximum number of related betaGroups returned (when they are included) (optional) 
            var limitAppStoreVersions = 56;  // int? | maximum number of related appStoreVersions returned (when they are included) (optional) 
            var limitPreReleaseVersions = 56;  // int? | maximum number of related preReleaseVersions returned (when they are included) (optional) 
            var limitBetaAppLocalizations = 56;  // int? | maximum number of related betaAppLocalizations returned (when they are included) (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 
            var limitAppInfos = 56;  // int? | maximum number of related appInfos returned (when they are included) (optional) 
            var limitAppClips = 56;  // int? | maximum number of related appClips returned (when they are included) (optional) 
            var limitInAppPurchases = 56;  // int? | maximum number of related inAppPurchases returned (when they are included) (optional) 
            var limitSubscriptionGroups = 56;  // int? | maximum number of related subscriptionGroups returned (when they are included) (optional) 
            var limitGameCenterEnabledVersions = 56;  // int? | maximum number of related gameCenterEnabledVersions returned (when they are included) (optional) 
            var limitAppCustomProductPages = 56;  // int? | maximum number of related appCustomProductPages returned (when they are included) (optional) 
            var limitInAppPurchasesV2 = 56;  // int? | maximum number of related inAppPurchasesV2 returned (when they are included) (optional) 
            var limitPromotedPurchases = 56;  // int? | maximum number of related promotedPurchases returned (when they are included) (optional) 
            var limitAppEvents = 56;  // int? | maximum number of related appEvents returned (when they are included) (optional) 
            var limitReviewSubmissions = 56;  // int? | maximum number of related reviewSubmissions returned (when they are included) (optional) 
            var limitAppStoreVersionExperimentsV2 = 56;  // int? | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional) 
            var limitAndroidToIosAppMappingDetails = 56;  // int? | maximum number of related androidToIosAppMappingDetails returned (when they are included) (optional) 

            try
            {
                AppResponse result = apiInstance.CiProductsAppGetToOneRelated(id, fieldsApps, fieldsAppEncryptionDeclarations, fieldsBuildIcons, fieldsCiProducts, fieldsBetaGroups, fieldsAppStoreVersions, fieldsPreReleaseVersions, fieldsBetaAppLocalizations, fieldsBuilds, fieldsBetaLicenseAgreements, fieldsBetaAppReviewDetails, fieldsAppInfos, fieldsAppClips, fieldsEndUserLicenseAgreements, fieldsInAppPurchases, fieldsSubscriptionGroups, fieldsGameCenterEnabledVersions, fieldsAppCustomProductPages, fieldsPromotedPurchases, fieldsAppEvents, fieldsReviewSubmissions, fieldsSubscriptionGracePeriods, fieldsGameCenterDetails, fieldsAppStoreVersionExperiments, fieldsAndroidToIosAppMappingDetails, include, limitAppEncryptionDeclarations, limitBetaGroups, limitAppStoreVersions, limitPreReleaseVersions, limitBetaAppLocalizations, limitBuilds, limitAppInfos, limitAppClips, limitInAppPurchases, limitSubscriptionGroups, limitGameCenterEnabledVersions, limitAppCustomProductPages, limitInAppPurchasesV2, limitPromotedPurchases, limitAppEvents, limitReviewSubmissions, limitAppStoreVersionExperimentsV2, limitAndroidToIosAppMappingDetails);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppResponse> response = apiInstance.CiProductsAppGetToOneRelatedWithHttpInfo(id, fieldsApps, fieldsAppEncryptionDeclarations, fieldsBuildIcons, fieldsCiProducts, fieldsBetaGroups, fieldsAppStoreVersions, fieldsPreReleaseVersions, fieldsBetaAppLocalizations, fieldsBuilds, fieldsBetaLicenseAgreements, fieldsBetaAppReviewDetails, fieldsAppInfos, fieldsAppClips, fieldsEndUserLicenseAgreements, fieldsInAppPurchases, fieldsSubscriptionGroups, fieldsGameCenterEnabledVersions, fieldsAppCustomProductPages, fieldsPromotedPurchases, fieldsAppEvents, fieldsReviewSubmissions, fieldsSubscriptionGracePeriods, fieldsGameCenterDetails, fieldsAppStoreVersionExperiments, fieldsAndroidToIosAppMappingDetails, include, limitAppEncryptionDeclarations, limitBetaGroups, limitAppStoreVersions, limitPreReleaseVersions, limitBetaAppLocalizations, limitBuilds, limitAppInfos, limitAppClips, limitInAppPurchases, limitSubscriptionGroups, limitGameCenterEnabledVersions, limitAppCustomProductPages, limitInAppPurchasesV2, limitPromotedPurchases, limitAppEvents, limitReviewSubmissions, limitAppStoreVersionExperimentsV2, limitAndroidToIosAppMappingDetails);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsAppGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaAppLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaLicenseAgreements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaLicenseAgreements | [optional]  |
| **fieldsBetaAppReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaAppReviewDetails | [optional]  |
| **fieldsAppInfos** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsEndUserLicenseAgreements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type endUserLicenseAgreements | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **fieldsSubscriptionGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionGroups | [optional]  |
| **fieldsGameCenterEnabledVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterEnabledVersions | [optional]  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsAppEvents** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appEvents | [optional]  |
| **fieldsReviewSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type reviewSubmissions | [optional]  |
| **fieldsSubscriptionGracePeriods** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionGracePeriods | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAndroidToIosAppMappingDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type androidToIosAppMappingDetails | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppEncryptionDeclarations** | **int?** | maximum number of related appEncryptionDeclarations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int?** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitAppStoreVersions** | **int?** | maximum number of related appStoreVersions returned (when they are included) | [optional]  |
| **limitPreReleaseVersions** | **int?** | maximum number of related preReleaseVersions returned (when they are included) | [optional]  |
| **limitBetaAppLocalizations** | **int?** | maximum number of related betaAppLocalizations returned (when they are included) | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |
| **limitAppInfos** | **int?** | maximum number of related appInfos returned (when they are included) | [optional]  |
| **limitAppClips** | **int?** | maximum number of related appClips returned (when they are included) | [optional]  |
| **limitInAppPurchases** | **int?** | maximum number of related inAppPurchases returned (when they are included) | [optional]  |
| **limitSubscriptionGroups** | **int?** | maximum number of related subscriptionGroups returned (when they are included) | [optional]  |
| **limitGameCenterEnabledVersions** | **int?** | maximum number of related gameCenterEnabledVersions returned (when they are included) | [optional]  |
| **limitAppCustomProductPages** | **int?** | maximum number of related appCustomProductPages returned (when they are included) | [optional]  |
| **limitInAppPurchasesV2** | **int?** | maximum number of related inAppPurchasesV2 returned (when they are included) | [optional]  |
| **limitPromotedPurchases** | **int?** | maximum number of related promotedPurchases returned (when they are included) | [optional]  |
| **limitAppEvents** | **int?** | maximum number of related appEvents returned (when they are included) | [optional]  |
| **limitReviewSubmissions** | **int?** | maximum number of related reviewSubmissions returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int?** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |
| **limitAndroidToIosAppMappingDetails** | **int?** | maximum number of related androidToIosAppMappingDetails returned (when they are included) | [optional]  |

### Return type

[**AppResponse**](AppResponse.md)

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
| **200** | Single App |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsappgettoonerelationship"></a>
# **CiProductsAppGetToOneRelationship**
> CiProductAppLinkageResponse CiProductsAppGetToOneRelationship (string id)



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
    public class CiProductsAppGetToOneRelationshipExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                CiProductAppLinkageResponse result = apiInstance.CiProductsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductAppLinkageResponse> response = apiInstance.CiProductsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CiProductAppLinkageResponse**](CiProductAppLinkageResponse.md)

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

<a id="ciproductsbuildrunsgettomanyrelated"></a>
# **CiProductsBuildRunsGetToManyRelated**
> CiBuildRunsResponse CiProductsBuildRunsGetToManyRelated (string id, List<string>? filterBuilds = null, List<string>? sort = null, List<string>? fieldsCiBuildRuns = null, List<string>? fieldsBuilds = null, List<string>? fieldsCiWorkflows = null, List<string>? fieldsCiProducts = null, List<string>? fieldsScmGitReferences = null, List<string>? fieldsScmPullRequests = null, int? limit = null, List<string>? include = null, int? limitBuilds = null)



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
    public class CiProductsBuildRunsGetToManyRelatedExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
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
                CiBuildRunsResponse result = apiInstance.CiProductsBuildRunsGetToManyRelated(id, filterBuilds, sort, fieldsCiBuildRuns, fieldsBuilds, fieldsCiWorkflows, fieldsCiProducts, fieldsScmGitReferences, fieldsScmPullRequests, limit, include, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsBuildRunsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsBuildRunsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiBuildRunsResponse> response = apiInstance.CiProductsBuildRunsGetToManyRelatedWithHttpInfo(id, filterBuilds, sort, fieldsCiBuildRuns, fieldsBuilds, fieldsCiWorkflows, fieldsCiProducts, fieldsScmGitReferences, fieldsScmPullRequests, limit, include, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsBuildRunsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="ciproductsbuildrunsgettomanyrelationship"></a>
# **CiProductsBuildRunsGetToManyRelationship**
> CiProductBuildRunsLinkagesResponse CiProductsBuildRunsGetToManyRelationship (string id, int? limit = null)



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
    public class CiProductsBuildRunsGetToManyRelationshipExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiProductBuildRunsLinkagesResponse result = apiInstance.CiProductsBuildRunsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsBuildRunsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsBuildRunsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductBuildRunsLinkagesResponse> response = apiInstance.CiProductsBuildRunsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsBuildRunsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiProductBuildRunsLinkagesResponse**](CiProductBuildRunsLinkagesResponse.md)

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

<a id="ciproductsdeleteinstance"></a>
# **CiProductsDeleteInstance**
> void CiProductsDeleteInstance (string id)



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
    public class CiProductsDeleteInstanceExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.CiProductsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.CiProductsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="ciproductsgetcollection"></a>
# **CiProductsGetCollection**
> CiProductsResponse CiProductsGetCollection (List<string>? filterProductType = null, List<string>? filterApp = null, List<string>? fieldsCiProducts = null, List<string>? fieldsApps = null, List<string>? fieldsScmRepositories = null, int? limit = null, List<string>? include = null, int? limitPrimaryRepositories = null)



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
    public class CiProductsGetCollectionExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var filterProductType = new List<string>?(); // List<string>? | filter by attribute 'productType' (optional) 
            var filterApp = new List<string>?(); // List<string>? | filter by id(s) of related 'app' (optional) 
            var fieldsCiProducts = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciProducts (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrimaryRepositories = 56;  // int? | maximum number of related primaryRepositories returned (when they are included) (optional) 

            try
            {
                CiProductsResponse result = apiInstance.CiProductsGetCollection(filterProductType, filterApp, fieldsCiProducts, fieldsApps, fieldsScmRepositories, limit, include, limitPrimaryRepositories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductsResponse> response = apiInstance.CiProductsGetCollectionWithHttpInfo(filterProductType, filterApp, fieldsCiProducts, fieldsApps, fieldsScmRepositories, limit, include, limitPrimaryRepositories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterProductType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;productType&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrimaryRepositories** | **int?** | maximum number of related primaryRepositories returned (when they are included) | [optional]  |

### Return type

[**CiProductsResponse**](CiProductsResponse.md)

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
| **200** | List of CiProducts |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsgetinstance"></a>
# **CiProductsGetInstance**
> CiProductResponse CiProductsGetInstance (string id, List<string>? fieldsCiProducts = null, List<string>? fieldsApps = null, List<string>? fieldsScmRepositories = null, List<string>? include = null, int? limitPrimaryRepositories = null)



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
    public class CiProductsGetInstanceExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiProducts = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciProducts (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrimaryRepositories = 56;  // int? | maximum number of related primaryRepositories returned (when they are included) (optional) 

            try
            {
                CiProductResponse result = apiInstance.CiProductsGetInstance(id, fieldsCiProducts, fieldsApps, fieldsScmRepositories, include, limitPrimaryRepositories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductResponse> response = apiInstance.CiProductsGetInstanceWithHttpInfo(id, fieldsCiProducts, fieldsApps, fieldsScmRepositories, include, limitPrimaryRepositories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiProducts** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrimaryRepositories** | **int?** | maximum number of related primaryRepositories returned (when they are included) | [optional]  |

### Return type

[**CiProductResponse**](CiProductResponse.md)

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
| **200** | Single CiProduct |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsprimaryrepositoriesgettomanyrelated"></a>
# **CiProductsPrimaryRepositoriesGetToManyRelated**
> ScmRepositoriesResponse CiProductsPrimaryRepositoriesGetToManyRelated (string id, List<string>? filterId = null, List<string>? fieldsScmRepositories = null, List<string>? fieldsScmProviders = null, List<string>? fieldsScmGitReferences = null, int? limit = null, List<string>? include = null)



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
    public class CiProductsPrimaryRepositoriesGetToManyRelatedExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var fieldsScmProviders = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmProviders (optional) 
            var fieldsScmGitReferences = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmGitReferences (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                ScmRepositoriesResponse result = apiInstance.CiProductsPrimaryRepositoriesGetToManyRelated(id, filterId, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsPrimaryRepositoriesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsPrimaryRepositoriesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<ScmRepositoriesResponse> response = apiInstance.CiProductsPrimaryRepositoriesGetToManyRelatedWithHttpInfo(id, filterId, fieldsScmRepositories, fieldsScmProviders, fieldsScmGitReferences, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsPrimaryRepositoriesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmRepositoriesResponse**](ScmRepositoriesResponse.md)

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
| **200** | List of ScmRepositories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsprimaryrepositoriesgettomanyrelationship"></a>
# **CiProductsPrimaryRepositoriesGetToManyRelationship**
> CiProductPrimaryRepositoriesLinkagesResponse CiProductsPrimaryRepositoriesGetToManyRelationship (string id, int? limit = null)



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
    public class CiProductsPrimaryRepositoriesGetToManyRelationshipExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiProductPrimaryRepositoriesLinkagesResponse result = apiInstance.CiProductsPrimaryRepositoriesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsPrimaryRepositoriesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsPrimaryRepositoriesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductPrimaryRepositoriesLinkagesResponse> response = apiInstance.CiProductsPrimaryRepositoriesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsPrimaryRepositoriesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiProductPrimaryRepositoriesLinkagesResponse**](CiProductPrimaryRepositoriesLinkagesResponse.md)

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

<a id="ciproductsworkflowsgettomanyrelated"></a>
# **CiProductsWorkflowsGetToManyRelated**
> CiWorkflowsResponse CiProductsWorkflowsGetToManyRelated (string id, List<string>? fieldsCiWorkflows = null, List<string>? fieldsCiProducts = null, List<string>? fieldsScmRepositories = null, List<string>? fieldsCiXcodeVersions = null, List<string>? fieldsCiMacOsVersions = null, int? limit = null, List<string>? include = null)



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
    public class CiProductsWorkflowsGetToManyRelatedExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCiWorkflows = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciWorkflows (optional) 
            var fieldsCiProducts = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciProducts (optional) 
            var fieldsScmRepositories = new List<string>?(); // List<string>? | the fields to include for returned resources of type scmRepositories (optional) 
            var fieldsCiXcodeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciXcodeVersions (optional) 
            var fieldsCiMacOsVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type ciMacOsVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CiWorkflowsResponse result = apiInstance.CiProductsWorkflowsGetToManyRelated(id, fieldsCiWorkflows, fieldsCiProducts, fieldsScmRepositories, fieldsCiXcodeVersions, fieldsCiMacOsVersions, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsWorkflowsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsWorkflowsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiWorkflowsResponse> response = apiInstance.CiProductsWorkflowsGetToManyRelatedWithHttpInfo(id, fieldsCiWorkflows, fieldsCiProducts, fieldsScmRepositories, fieldsCiXcodeVersions, fieldsCiMacOsVersions, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsWorkflowsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CiWorkflowsResponse**](CiWorkflowsResponse.md)

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
| **200** | List of CiWorkflows |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="ciproductsworkflowsgettomanyrelationship"></a>
# **CiProductsWorkflowsGetToManyRelationship**
> CiProductWorkflowsLinkagesResponse CiProductsWorkflowsGetToManyRelationship (string id, int? limit = null)



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
    public class CiProductsWorkflowsGetToManyRelationshipExample
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
            var apiInstance = new CiProductsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                CiProductWorkflowsLinkagesResponse result = apiInstance.CiProductsWorkflowsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CiProductsApi.CiProductsWorkflowsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CiProductsWorkflowsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CiProductWorkflowsLinkagesResponse> response = apiInstance.CiProductsWorkflowsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CiProductsApi.CiProductsWorkflowsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**CiProductWorkflowsLinkagesResponse**](CiProductWorkflowsLinkagesResponse.md)

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

