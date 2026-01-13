# AppStoreConnect.Net.Api.ScmProvidersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ScmProvidersGetCollection**](ScmProvidersApi.md#scmprovidersgetcollection) | **GET** /v1/scmProviders |  |
| [**ScmProvidersGetInstance**](ScmProvidersApi.md#scmprovidersgetinstance) | **GET** /v1/scmProviders/{id} |  |
| [**ScmProvidersRepositoriesGetToManyRelated**](ScmProvidersApi.md#scmprovidersrepositoriesgettomanyrelated) | **GET** /v1/scmProviders/{id}/repositories |  |
| [**ScmProvidersRepositoriesGetToManyRelationship**](ScmProvidersApi.md#scmprovidersrepositoriesgettomanyrelationship) | **GET** /v1/scmProviders/{id}/relationships/repositories |  |

<a id="scmprovidersgetcollection"></a>
# **ScmProvidersGetCollection**
> ScmProvidersResponse ScmProvidersGetCollection (List<string> fieldsScmProviders = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsScmProviders** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ScmProvidersResponse**](ScmProvidersResponse.md)

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
| **200** | List of ScmProviders |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="scmprovidersgetinstance"></a>
# **ScmProvidersGetInstance**
> ScmProviderResponse ScmProvidersGetInstance (string id, List<string> fieldsScmProviders = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmProviders** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmProviders | [optional]  |

### Return type

[**ScmProviderResponse**](ScmProviderResponse.md)

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
| **200** | Single ScmProvider |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="scmprovidersrepositoriesgettomanyrelated"></a>
# **ScmProvidersRepositoriesGetToManyRelated**
> ScmRepositoriesResponse ScmProvidersRepositoriesGetToManyRelated (string id, List<string> filterId = null, List<string> fieldsScmRepositories = null, List<string> fieldsScmProviders = null, List<string> fieldsScmGitReferences = null, int limit = null, List<string> include = null)




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

<a id="scmprovidersrepositoriesgettomanyrelationship"></a>
# **ScmProvidersRepositoriesGetToManyRelationship**
> ScmProviderRepositoriesLinkagesResponse ScmProvidersRepositoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ScmProviderRepositoriesLinkagesResponse**](ScmProviderRepositoriesLinkagesResponse.md)

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

