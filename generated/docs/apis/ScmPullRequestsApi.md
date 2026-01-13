# AppStoreConnect.Net.Api.ScmPullRequestsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ScmPullRequestsGetInstance**](ScmPullRequestsApi.md#scmpullrequestsgetinstance) | **GET** /v1/scmPullRequests/{id} |  |

<a id="scmpullrequestsgetinstance"></a>
# **ScmPullRequestsGetInstance**
> ScmPullRequestResponse ScmPullRequestsGetInstance (string id, List<string> fieldsScmPullRequests = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsScmPullRequests** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type scmPullRequests | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ScmPullRequestResponse**](ScmPullRequestResponse.md)

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
| **200** | Single ScmPullRequest |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

