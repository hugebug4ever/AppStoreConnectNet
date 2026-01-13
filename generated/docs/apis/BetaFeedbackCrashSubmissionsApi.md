# AppStoreConnect.Net.Api.BetaFeedbackCrashSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionscrashloggettoonerelated) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/crashLog |  |
| [**BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionscrashloggettoonerelationship) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/relationships/crashLog |  |
| [**BetaFeedbackCrashSubmissionsDeleteInstance**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionsdeleteinstance) | **DELETE** /v1/betaFeedbackCrashSubmissions/{id} |  |
| [**BetaFeedbackCrashSubmissionsGetInstance**](BetaFeedbackCrashSubmissionsApi.md#betafeedbackcrashsubmissionsgetinstance) | **GET** /v1/betaFeedbackCrashSubmissions/{id} |  |

<a id="betafeedbackcrashsubmissionscrashloggettoonerelated"></a>
# **BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated**
> BetaCrashLogResponse BetaFeedbackCrashSubmissionsCrashLogGetToOneRelated (string id, List<string> fieldsBetaCrashLogs = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaCrashLogs** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaCrashLogs | [optional]  |

### Return type

[**BetaCrashLogResponse**](BetaCrashLogResponse.md)

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
| **200** | Single BetaCrashLog |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betafeedbackcrashsubmissionscrashloggettoonerelationship"></a>
# **BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship**
> BetaFeedbackCrashSubmissionCrashLogLinkageResponse BetaFeedbackCrashSubmissionsCrashLogGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaFeedbackCrashSubmissionCrashLogLinkageResponse**](BetaFeedbackCrashSubmissionCrashLogLinkageResponse.md)

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

<a id="betafeedbackcrashsubmissionsdeleteinstance"></a>
# **BetaFeedbackCrashSubmissionsDeleteInstance**
> void BetaFeedbackCrashSubmissionsDeleteInstance (string id)




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

<a id="betafeedbackcrashsubmissionsgetinstance"></a>
# **BetaFeedbackCrashSubmissionsGetInstance**
> BetaFeedbackCrashSubmissionResponse BetaFeedbackCrashSubmissionsGetInstance (string id, List<string> fieldsBetaFeedbackCrashSubmissions = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaFeedbackCrashSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaFeedbackCrashSubmissions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaFeedbackCrashSubmissionResponse**](BetaFeedbackCrashSubmissionResponse.md)

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
| **200** | Single BetaFeedbackCrashSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

