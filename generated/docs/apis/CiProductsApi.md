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
> ScmRepositoriesResponse CiProductsAdditionalRepositoriesGetToManyRelated (string id, List<string> filterId = null, List<string> fieldsScmRepositories = null, List<string> fieldsScmProviders = null, List<string> fieldsScmGitReferences = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsadditionalrepositoriesgettomanyrelationship"></a>
# **CiProductsAdditionalRepositoriesGetToManyRelationship**
> CiProductAdditionalRepositoriesLinkagesResponse CiProductsAdditionalRepositoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsappgettoonerelated"></a>
# **CiProductsAppGetToOneRelated**
> AppResponse CiProductsAppGetToOneRelated (string id, List<string> fieldsApps = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsBuildIcons = null, List<string> fieldsCiProducts = null, List<string> fieldsBetaGroups = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBetaAppLocalizations = null, List<string> fieldsBuilds = null, List<string> fieldsBetaLicenseAgreements = null, List<string> fieldsBetaAppReviewDetails = null, List<string> fieldsAppInfos = null, List<string> fieldsAppClips = null, List<string> fieldsEndUserLicenseAgreements = null, List<string> fieldsInAppPurchases = null, List<string> fieldsSubscriptionGroups = null, List<string> fieldsGameCenterEnabledVersions = null, List<string> fieldsAppCustomProductPages = null, List<string> fieldsPromotedPurchases = null, List<string> fieldsAppEvents = null, List<string> fieldsReviewSubmissions = null, List<string> fieldsSubscriptionGracePeriods = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAndroidToIosAppMappingDetails = null, List<string> include = null, int limitAppEncryptionDeclarations = null, int limitBetaGroups = null, int limitAppStoreVersions = null, int limitPreReleaseVersions = null, int limitBetaAppLocalizations = null, int limitBuilds = null, int limitAppInfos = null, int limitAppClips = null, int limitInAppPurchases = null, int limitSubscriptionGroups = null, int limitGameCenterEnabledVersions = null, int limitAppCustomProductPages = null, int limitInAppPurchasesV2 = null, int limitPromotedPurchases = null, int limitAppEvents = null, int limitReviewSubmissions = null, int limitAppStoreVersionExperimentsV2 = null, int limitAndroidToIosAppMappingDetails = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaAppLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaLicenseAgreements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaLicenseAgreements | [optional]  |
| **fieldsBetaAppReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewDetails | [optional]  |
| **fieldsAppInfos** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsEndUserLicenseAgreements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type endUserLicenseAgreements | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **fieldsSubscriptionGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroups | [optional]  |
| **fieldsGameCenterEnabledVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterEnabledVersions | [optional]  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsAppEvents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEvents | [optional]  |
| **fieldsReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissions | [optional]  |
| **fieldsSubscriptionGracePeriods** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGracePeriods | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAndroidToIosAppMappingDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type androidToIosAppMappingDetails | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppEncryptionDeclarations** | **int** | maximum number of related appEncryptionDeclarations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitAppStoreVersions** | **int** | maximum number of related appStoreVersions returned (when they are included) | [optional]  |
| **limitPreReleaseVersions** | **int** | maximum number of related preReleaseVersions returned (when they are included) | [optional]  |
| **limitBetaAppLocalizations** | **int** | maximum number of related betaAppLocalizations returned (when they are included) | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |
| **limitAppInfos** | **int** | maximum number of related appInfos returned (when they are included) | [optional]  |
| **limitAppClips** | **int** | maximum number of related appClips returned (when they are included) | [optional]  |
| **limitInAppPurchases** | **int** | maximum number of related inAppPurchases returned (when they are included) | [optional]  |
| **limitSubscriptionGroups** | **int** | maximum number of related subscriptionGroups returned (when they are included) | [optional]  |
| **limitGameCenterEnabledVersions** | **int** | maximum number of related gameCenterEnabledVersions returned (when they are included) | [optional]  |
| **limitAppCustomProductPages** | **int** | maximum number of related appCustomProductPages returned (when they are included) | [optional]  |
| **limitInAppPurchasesV2** | **int** | maximum number of related inAppPurchasesV2 returned (when they are included) | [optional]  |
| **limitPromotedPurchases** | **int** | maximum number of related promotedPurchases returned (when they are included) | [optional]  |
| **limitAppEvents** | **int** | maximum number of related appEvents returned (when they are included) | [optional]  |
| **limitReviewSubmissions** | **int** | maximum number of related reviewSubmissions returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |
| **limitAndroidToIosAppMappingDetails** | **int** | maximum number of related androidToIosAppMappingDetails returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsappgettoonerelationship"></a>
# **CiProductsAppGetToOneRelationship**
> CiProductAppLinkageResponse CiProductsAppGetToOneRelationship (string id)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsbuildrunsgettomanyrelated"></a>
# **CiProductsBuildRunsGetToManyRelated**
> CiBuildRunsResponse CiProductsBuildRunsGetToManyRelated (string id, List<string> filterBuilds = null, List<string> sort = null, List<string> fieldsCiBuildRuns = null, List<string> fieldsBuilds = null, List<string> fieldsCiWorkflows = null, List<string> fieldsCiProducts = null, List<string> fieldsScmGitReferences = null, List<string> fieldsScmPullRequests = null, int limit = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterBuilds** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **fieldsScmPullRequests** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmPullRequests | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsbuildrunsgettomanyrelationship"></a>
# **CiProductsBuildRunsGetToManyRelationship**
> CiProductBuildRunsLinkagesResponse CiProductsBuildRunsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsdeleteinstance"></a>
# **CiProductsDeleteInstance**
> void CiProductsDeleteInstance (string id)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsgetcollection"></a>
# **CiProductsGetCollection**
> CiProductsResponse CiProductsGetCollection (List<string> filterProductType = null, List<string> filterApp = null, List<string> fieldsCiProducts = null, List<string> fieldsApps = null, List<string> fieldsScmRepositories = null, int limit = null, List<string> include = null, int limitPrimaryRepositories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterProductType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;productType&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrimaryRepositories** | **int** | maximum number of related primaryRepositories returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsgetinstance"></a>
# **CiProductsGetInstance**
> CiProductResponse CiProductsGetInstance (string id, List<string> fieldsCiProducts = null, List<string> fieldsApps = null, List<string> fieldsScmRepositories = null, List<string> include = null, int limitPrimaryRepositories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrimaryRepositories** | **int** | maximum number of related primaryRepositories returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsprimaryrepositoriesgettomanyrelated"></a>
# **CiProductsPrimaryRepositoriesGetToManyRelated**
> ScmRepositoriesResponse CiProductsPrimaryRepositoriesGetToManyRelated (string id, List<string> filterId = null, List<string> fieldsScmRepositories = null, List<string> fieldsScmProviders = null, List<string> fieldsScmGitReferences = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsprimaryrepositoriesgettomanyrelationship"></a>
# **CiProductsPrimaryRepositoriesGetToManyRelationship**
> CiProductPrimaryRepositoriesLinkagesResponse CiProductsPrimaryRepositoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsworkflowsgettomanyrelated"></a>
# **CiProductsWorkflowsGetToManyRelated**
> CiWorkflowsResponse CiProductsWorkflowsGetToManyRelated (string id, List<string> fieldsCiWorkflows = null, List<string> fieldsCiProducts = null, List<string> fieldsScmRepositories = null, List<string> fieldsCiXcodeVersions = null, List<string> fieldsCiMacOsVersions = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciproductsworkflowsgettomanyrelationship"></a>
# **CiProductsWorkflowsGetToManyRelationship**
> CiProductWorkflowsLinkagesResponse CiProductsWorkflowsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

