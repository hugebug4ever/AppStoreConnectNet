# AppStoreConnect.Net.Api.BetaFeedbackScreenshotSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaFeedbackScreenshotSubmissionsDeleteInstance**](BetaFeedbackScreenshotSubmissionsApi.md#betafeedbackscreenshotsubmissionsdeleteinstance) | **DELETE** /v1/betaFeedbackScreenshotSubmissions/{id} |  |
| [**BetaFeedbackScreenshotSubmissionsGetInstance**](BetaFeedbackScreenshotSubmissionsApi.md#betafeedbackscreenshotsubmissionsgetinstance) | **GET** /v1/betaFeedbackScreenshotSubmissions/{id} |  |

<a id="betafeedbackscreenshotsubmissionsdeleteinstance"></a>
# **BetaFeedbackScreenshotSubmissionsDeleteInstance**
> void BetaFeedbackScreenshotSubmissionsDeleteInstance (string id)




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

<a id="betafeedbackscreenshotsubmissionsgetinstance"></a>
# **BetaFeedbackScreenshotSubmissionsGetInstance**
> BetaFeedbackScreenshotSubmissionResponse BetaFeedbackScreenshotSubmissionsGetInstance (string id, List<string> fieldsBetaFeedbackScreenshotSubmissions = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaFeedbackScreenshotSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaFeedbackScreenshotSubmissions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaFeedbackScreenshotSubmissionResponse**](BetaFeedbackScreenshotSubmissionResponse.md)

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
| **200** | Single BetaFeedbackScreenshotSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

