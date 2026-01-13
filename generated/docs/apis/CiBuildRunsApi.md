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
> CiBuildActionsResponse CiBuildRunsActionsGetToManyRelated (string id, List<string> fieldsCiBuildActions = null, List<string> fieldsCiBuildRuns = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildActions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildActions | [optional]  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildrunsactionsgettomanyrelationship"></a>
# **CiBuildRunsActionsGetToManyRelationship**
> CiBuildRunActionsLinkagesResponse CiBuildRunsActionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildrunsbuildsgettomanyrelated"></a>
# **CiBuildRunsBuildsGetToManyRelated**
> BuildsResponse CiBuildRunsBuildsGetToManyRelated (string id, List<string> filterVersion = null, List<string> filterExpired = null, List<string> filterProcessingState = null, List<string> filterBetaAppReviewSubmissionBetaReviewState = null, List<string> filterUsesNonExemptEncryption = null, List<string> filterPreReleaseVersionVersion = null, List<string> filterPreReleaseVersionPlatform = null, List<string> filterBuildAudienceType = null, List<string> filterPreReleaseVersion = null, List<string> filterApp = null, List<string> filterBetaGroups = null, List<string> filterAppStoreVersion = null, List<string> filterId = null, bool existsUsesNonExemptEncryption = null, List<string> sort = null, List<string> fieldsBuilds = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaGroups = null, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsApps = null, List<string> fieldsBuildBetaDetails = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsBuildIcons = null, List<string> fieldsBuildBundles = null, List<string> fieldsBuildUploads = null, int limit = null, List<string> include = null, int limitIndividualTesters = null, int limitBetaGroups = null, int limitBetaBuildLocalizations = null, int limitIcons = null, int limitBuildBundles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterExpired** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;expired&#39; | [optional]  |
| **filterProcessingState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;processingState&#39; | [optional]  |
| **filterBetaAppReviewSubmissionBetaReviewState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;betaAppReviewSubmission.betaReviewState&#39; | [optional]  |
| **filterUsesNonExemptEncryption** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **filterPreReleaseVersionVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;preReleaseVersion.version&#39; | [optional]  |
| **filterPreReleaseVersionPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;preReleaseVersion.platform&#39; | [optional]  |
| **filterBuildAudienceType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;buildAudienceType&#39; | [optional]  |
| **filterPreReleaseVersion** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;preReleaseVersion&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBetaGroups** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;betaGroups&#39; | [optional]  |
| **filterAppStoreVersion** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersion&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **existsUsesNonExemptEncryption** | **bool** | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **fieldsBuildBundles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBundles | [optional]  |
| **fieldsBuildUploads** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildUploads | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitIndividualTesters** | **int** | maximum number of related individualTesters returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBetaBuildLocalizations** | **int** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitIcons** | **int** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int** | maximum number of related buildBundles returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildrunsbuildsgettomanyrelationship"></a>
# **CiBuildRunsBuildsGetToManyRelationship**
> CiBuildRunBuildsLinkagesResponse CiBuildRunsBuildsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildrunscreateinstance"></a>
# **CiBuildRunsCreateInstance**
> CiBuildRunResponse CiBuildRunsCreateInstance (CiBuildRunCreateRequest ciBuildRunCreateRequest)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildrunsgetinstance"></a>
# **CiBuildRunsGetInstance**
> CiBuildRunResponse CiBuildRunsGetInstance (string id, List<string> fieldsCiBuildRuns = null, List<string> fieldsBuilds = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

