# AppStoreConnect.Net.Api.ScmRepositoriesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ScmRepositoriesGetCollection**](ScmRepositoriesApi.md#scmrepositoriesgetcollection) | **GET** /v1/scmRepositories |  |
| [**ScmRepositoriesGetInstance**](ScmRepositoriesApi.md#scmrepositoriesgetinstance) | **GET** /v1/scmRepositories/{id} |  |
| [**ScmRepositoriesGitReferencesGetToManyRelated**](ScmRepositoriesApi.md#scmrepositoriesgitreferencesgettomanyrelated) | **GET** /v1/scmRepositories/{id}/gitReferences |  |
| [**ScmRepositoriesGitReferencesGetToManyRelationship**](ScmRepositoriesApi.md#scmrepositoriesgitreferencesgettomanyrelationship) | **GET** /v1/scmRepositories/{id}/relationships/gitReferences |  |
| [**ScmRepositoriesPullRequestsGetToManyRelated**](ScmRepositoriesApi.md#scmrepositoriespullrequestsgettomanyrelated) | **GET** /v1/scmRepositories/{id}/pullRequests |  |
| [**ScmRepositoriesPullRequestsGetToManyRelationship**](ScmRepositoriesApi.md#scmrepositoriespullrequestsgettomanyrelationship) | **GET** /v1/scmRepositories/{id}/relationships/pullRequests |  |

<a id="scmrepositoriesgetcollection"></a>
# **ScmRepositoriesGetCollection**
> ScmRepositoriesResponse ScmRepositoriesGetCollection (List<string> filterId = null, List<string> fieldsScmRepositories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
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
| **200** | List of ScmRepositories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="scmrepositoriesgetinstance"></a>
# **ScmRepositoriesGetInstance**
> ScmRepositoryResponse ScmRepositoriesGetInstance (string id, List<string> fieldsScmRepositories = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
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

<a id="scmrepositoriesgitreferencesgettomanyrelated"></a>
# **ScmRepositoriesGitReferencesGetToManyRelated**
> ScmGitReferencesResponse ScmRepositoriesGitReferencesGetToManyRelated (string id, List<string> fieldsScmGitReferences = null, List<string> fieldsScmRepositories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmGitReferences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmGitReferences | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmGitReferencesResponse**](ScmGitReferencesResponse.md)

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
| **200** | List of ScmGitReferences |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="scmrepositoriesgitreferencesgettomanyrelationship"></a>
# **ScmRepositoriesGitReferencesGetToManyRelationship**
> ScmRepositoryGitReferencesLinkagesResponse ScmRepositoriesGitReferencesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ScmRepositoryGitReferencesLinkagesResponse**](ScmRepositoryGitReferencesLinkagesResponse.md)

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

<a id="scmrepositoriespullrequestsgettomanyrelated"></a>
# **ScmRepositoriesPullRequestsGetToManyRelated**
> ScmPullRequestsResponse ScmRepositoriesPullRequestsGetToManyRelated (string id, List<string> fieldsScmPullRequests = null, List<string> fieldsScmRepositories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmPullRequests** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmPullRequests | [optional]  |
| **fieldsScmRepositories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmRepositories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmPullRequestsResponse**](ScmPullRequestsResponse.md)

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
| **200** | List of ScmPullRequests |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="scmrepositoriespullrequestsgettomanyrelationship"></a>
# **ScmRepositoriesPullRequestsGetToManyRelationship**
> ScmRepositoryPullRequestsLinkagesResponse ScmRepositoriesPullRequestsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ScmRepositoryPullRequestsLinkagesResponse**](ScmRepositoryPullRequestsLinkagesResponse.md)

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

