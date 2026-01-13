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
> CiBuildRunsResponse CiWorkflowsBuildRunsGetToManyRelated (string id, List<string> filterBuilds = null, List<string> sort = null, List<string> fieldsCiBuildRuns = null, List<string> fieldsBuilds = null, List<string> fieldsCiWorkflows = null, List<string> fieldsCiProducts = null, List<string> fieldsScmGitReferences = null, List<string> fieldsScmPullRequests = null, int limit = null, List<string> include = null, int limitBuilds = null)




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

<a id="ciworkflowsbuildrunsgettomanyrelationship"></a>
# **CiWorkflowsBuildRunsGetToManyRelationship**
> CiWorkflowBuildRunsLinkagesResponse CiWorkflowsBuildRunsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciworkflowscreateinstance"></a>
# **CiWorkflowsCreateInstance**
> CiWorkflowResponse CiWorkflowsCreateInstance (CiWorkflowCreateRequest ciWorkflowCreateRequest)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciworkflowsdeleteinstance"></a>
# **CiWorkflowsDeleteInstance**
> void CiWorkflowsDeleteInstance (string id)




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

<a id="ciworkflowsgetinstance"></a>
# **CiWorkflowsGetInstance**
> CiWorkflowResponse CiWorkflowsGetInstance (string id, List<string> fieldsCiWorkflows = null, List<string> fieldsScmRepositories = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiWorkflows** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciWorkflows | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciworkflowsrepositorygettoonerelated"></a>
# **CiWorkflowsRepositoryGetToOneRelated**
> ScmRepositoryResponse CiWorkflowsRepositoryGetToOneRelated (string id, List<string> fieldsScmRepositories = null, List<string> fieldsScmProviders = null, List<string> fieldsScmGitReferences = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **fieldsScmProviders** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciworkflowsrepositorygettoonerelationship"></a>
# **CiWorkflowsRepositoryGetToOneRelationship**
> CiWorkflowRepositoryLinkageResponse CiWorkflowsRepositoryGetToOneRelationship (string id)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="ciworkflowsupdateinstance"></a>
# **CiWorkflowsUpdateInstance**
> CiWorkflowResponse CiWorkflowsUpdateInstance (string id, CiWorkflowUpdateRequest ciWorkflowUpdateRequest)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

