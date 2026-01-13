# AppStoreConnect.Net.Api.BetaAppReviewSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaAppReviewSubmissionsBuildGetToOneRelated**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsbuildgettoonerelated) | **GET** /v1/betaAppReviewSubmissions/{id}/build |  |
| [**BetaAppReviewSubmissionsBuildGetToOneRelationship**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsbuildgettoonerelationship) | **GET** /v1/betaAppReviewSubmissions/{id}/relationships/build |  |
| [**BetaAppReviewSubmissionsCreateInstance**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionscreateinstance) | **POST** /v1/betaAppReviewSubmissions |  |
| [**BetaAppReviewSubmissionsGetCollection**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsgetcollection) | **GET** /v1/betaAppReviewSubmissions |  |
| [**BetaAppReviewSubmissionsGetInstance**](BetaAppReviewSubmissionsApi.md#betaappreviewsubmissionsgetinstance) | **GET** /v1/betaAppReviewSubmissions/{id} |  |

<a id="betaappreviewsubmissionsbuildgettoonerelated"></a>
# **BetaAppReviewSubmissionsBuildGetToOneRelated**
> BuildWithoutIncludesResponse BetaAppReviewSubmissionsBuildGetToOneRelated (string id, List<string> fieldsBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |

### Return type

[**BuildWithoutIncludesResponse**](BuildWithoutIncludesResponse.md)

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
| **200** | Single Build with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betaappreviewsubmissionsbuildgettoonerelationship"></a>
# **BetaAppReviewSubmissionsBuildGetToOneRelationship**
> BetaAppReviewSubmissionBuildLinkageResponse BetaAppReviewSubmissionsBuildGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaAppReviewSubmissionBuildLinkageResponse**](BetaAppReviewSubmissionBuildLinkageResponse.md)

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

<a id="betaappreviewsubmissionscreateinstance"></a>
# **BetaAppReviewSubmissionsCreateInstance**
> BetaAppReviewSubmissionResponse BetaAppReviewSubmissionsCreateInstance (BetaAppReviewSubmissionCreateRequest betaAppReviewSubmissionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaAppReviewSubmissionCreateRequest** | [**BetaAppReviewSubmissionCreateRequest**](BetaAppReviewSubmissionCreateRequest.md) | BetaAppReviewSubmission representation |  |

### Return type

[**BetaAppReviewSubmissionResponse**](BetaAppReviewSubmissionResponse.md)

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
| **201** | Single BetaAppReviewSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betaappreviewsubmissionsgetcollection"></a>
# **BetaAppReviewSubmissionsGetCollection**
> BetaAppReviewSubmissionsResponse BetaAppReviewSubmissionsGetCollection (List<string> filterBuild, List<string> filterBetaReviewState = null, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsBuilds = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuild** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;build&#39; |  |
| **filterBetaReviewState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;betaReviewState&#39; | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewSubmissionsResponse**](BetaAppReviewSubmissionsResponse.md)

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
| **200** | List of BetaAppReviewSubmissions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betaappreviewsubmissionsgetinstance"></a>
# **BetaAppReviewSubmissionsGetInstance**
> BetaAppReviewSubmissionResponse BetaAppReviewSubmissionsGetInstance (string id, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsBuilds = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaAppReviewSubmissionResponse**](BetaAppReviewSubmissionResponse.md)

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
| **200** | Single BetaAppReviewSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

