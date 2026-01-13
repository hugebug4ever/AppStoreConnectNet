# AppStoreConnect.Net.Api.BetaAppClipInvocationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaAppClipInvocationsCreateInstance**](BetaAppClipInvocationsApi.md#betaappclipinvocationscreateinstance) | **POST** /v1/betaAppClipInvocations |  |
| [**BetaAppClipInvocationsDeleteInstance**](BetaAppClipInvocationsApi.md#betaappclipinvocationsdeleteinstance) | **DELETE** /v1/betaAppClipInvocations/{id} |  |
| [**BetaAppClipInvocationsGetInstance**](BetaAppClipInvocationsApi.md#betaappclipinvocationsgetinstance) | **GET** /v1/betaAppClipInvocations/{id} |  |
| [**BetaAppClipInvocationsUpdateInstance**](BetaAppClipInvocationsApi.md#betaappclipinvocationsupdateinstance) | **PATCH** /v1/betaAppClipInvocations/{id} |  |

<a id="betaappclipinvocationscreateinstance"></a>
# **BetaAppClipInvocationsCreateInstance**
> BetaAppClipInvocationResponse BetaAppClipInvocationsCreateInstance (BetaAppClipInvocationCreateRequest betaAppClipInvocationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaAppClipInvocationCreateRequest** | [**BetaAppClipInvocationCreateRequest**](BetaAppClipInvocationCreateRequest.md) | BetaAppClipInvocation representation |  |

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
| **201** | Single BetaAppClipInvocation |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betaappclipinvocationsdeleteinstance"></a>
# **BetaAppClipInvocationsDeleteInstance**
> void BetaAppClipInvocationsDeleteInstance (string id)




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

<a id="betaappclipinvocationsgetinstance"></a>
# **BetaAppClipInvocationsGetInstance**
> BetaAppClipInvocationResponse BetaAppClipInvocationsGetInstance (string id, List<string> fieldsBetaAppClipInvocations = null, List<string> include = null, int limitBetaAppClipInvocationLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppClipInvocations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppClipInvocations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaAppClipInvocationLocalizations** | **int** | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) | [optional]  |

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
| **200** | Single BetaAppClipInvocation |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betaappclipinvocationsupdateinstance"></a>
# **BetaAppClipInvocationsUpdateInstance**
> BetaAppClipInvocationResponse BetaAppClipInvocationsUpdateInstance (string id, BetaAppClipInvocationUpdateRequest betaAppClipInvocationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaAppClipInvocationUpdateRequest** | [**BetaAppClipInvocationUpdateRequest**](BetaAppClipInvocationUpdateRequest.md) | BetaAppClipInvocation representation |  |

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
| **200** | Single BetaAppClipInvocation |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

