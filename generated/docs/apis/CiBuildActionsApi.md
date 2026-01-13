# AppStoreConnect.Net.Api.CiBuildActionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiBuildActionsArtifactsGetToManyRelated**](CiBuildActionsApi.md#cibuildactionsartifactsgettomanyrelated) | **GET** /v1/ciBuildActions/{id}/artifacts |  |
| [**CiBuildActionsArtifactsGetToManyRelationship**](CiBuildActionsApi.md#cibuildactionsartifactsgettomanyrelationship) | **GET** /v1/ciBuildActions/{id}/relationships/artifacts |  |
| [**CiBuildActionsBuildRunGetToOneRelated**](CiBuildActionsApi.md#cibuildactionsbuildrungettoonerelated) | **GET** /v1/ciBuildActions/{id}/buildRun |  |
| [**CiBuildActionsBuildRunGetToOneRelationship**](CiBuildActionsApi.md#cibuildactionsbuildrungettoonerelationship) | **GET** /v1/ciBuildActions/{id}/relationships/buildRun |  |
| [**CiBuildActionsGetInstance**](CiBuildActionsApi.md#cibuildactionsgetinstance) | **GET** /v1/ciBuildActions/{id} |  |
| [**CiBuildActionsIssuesGetToManyRelated**](CiBuildActionsApi.md#cibuildactionsissuesgettomanyrelated) | **GET** /v1/ciBuildActions/{id}/issues |  |
| [**CiBuildActionsIssuesGetToManyRelationship**](CiBuildActionsApi.md#cibuildactionsissuesgettomanyrelationship) | **GET** /v1/ciBuildActions/{id}/relationships/issues |  |
| [**CiBuildActionsTestResultsGetToManyRelated**](CiBuildActionsApi.md#cibuildactionstestresultsgettomanyrelated) | **GET** /v1/ciBuildActions/{id}/testResults |  |
| [**CiBuildActionsTestResultsGetToManyRelationship**](CiBuildActionsApi.md#cibuildactionstestresultsgettomanyrelationship) | **GET** /v1/ciBuildActions/{id}/relationships/testResults |  |

<a id="cibuildactionsartifactsgettomanyrelated"></a>
# **CiBuildActionsArtifactsGetToManyRelated**
> CiArtifactsResponse CiBuildActionsArtifactsGetToManyRelated (string id, List<string> fieldsCiArtifacts = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiArtifacts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciArtifacts | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiArtifactsResponse**](CiArtifactsResponse.md)

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
| **200** | List of CiArtifacts |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildactionsartifactsgettomanyrelationship"></a>
# **CiBuildActionsArtifactsGetToManyRelationship**
> CiBuildActionArtifactsLinkagesResponse CiBuildActionsArtifactsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiBuildActionArtifactsLinkagesResponse**](CiBuildActionArtifactsLinkagesResponse.md)

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

<a id="cibuildactionsbuildrungettoonerelated"></a>
# **CiBuildActionsBuildRunGetToOneRelated**
> CiBuildRunResponse CiBuildActionsBuildRunGetToOneRelated (string id, List<string> fieldsCiBuildRuns = null, List<string> fieldsBuilds = null, List<string> fieldsCiWorkflows = null, List<string> fieldsCiProducts = null, List<string> fieldsScmGitReferences = null, List<string> fieldsScmPullRequests = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsCiProducts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciProducts | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **fieldsScmPullRequests** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmPullRequests | [optional]  |
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

<a id="cibuildactionsbuildrungettoonerelationship"></a>
# **CiBuildActionsBuildRunGetToOneRelationship**
> CiBuildActionBuildRunLinkageResponse CiBuildActionsBuildRunGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CiBuildActionBuildRunLinkageResponse**](CiBuildActionBuildRunLinkageResponse.md)

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

<a id="cibuildactionsgetinstance"></a>
# **CiBuildActionsGetInstance**
> CiBuildActionResponse CiBuildActionsGetInstance (string id, List<string> fieldsCiBuildActions = null, List<string> fieldsCiBuildRuns = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiBuildActions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildActions | [optional]  |
| **fieldsCiBuildRuns** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciBuildRuns | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CiBuildActionResponse**](CiBuildActionResponse.md)

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
| **200** | Single CiBuildAction |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildactionsissuesgettomanyrelated"></a>
# **CiBuildActionsIssuesGetToManyRelated**
> CiIssuesResponse CiBuildActionsIssuesGetToManyRelated (string id, List<string> fieldsCiIssues = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiIssues** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciIssues | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiIssuesResponse**](CiIssuesResponse.md)

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
| **200** | List of CiIssues |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildactionsissuesgettomanyrelationship"></a>
# **CiBuildActionsIssuesGetToManyRelationship**
> CiBuildActionIssuesLinkagesResponse CiBuildActionsIssuesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiBuildActionIssuesLinkagesResponse**](CiBuildActionIssuesLinkagesResponse.md)

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

<a id="cibuildactionstestresultsgettomanyrelated"></a>
# **CiBuildActionsTestResultsGetToManyRelated**
> CiTestResultsResponse CiBuildActionsTestResultsGetToManyRelated (string id, List<string> fieldsCiTestResults = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiTestResults** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciTestResults | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiTestResultsResponse**](CiTestResultsResponse.md)

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
| **200** | List of CiTestResults |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cibuildactionstestresultsgettomanyrelationship"></a>
# **CiBuildActionsTestResultsGetToManyRelationship**
> CiBuildActionTestResultsLinkagesResponse CiBuildActionsTestResultsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiBuildActionTestResultsLinkagesResponse**](CiBuildActionTestResultsLinkagesResponse.md)

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

