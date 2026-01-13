# AppStoreConnect.Net.Api.InAppPurchaseSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseSubmissionsCreateInstance**](InAppPurchaseSubmissionsApi.md#inapppurchasesubmissionscreateinstance) | **POST** /v1/inAppPurchaseSubmissions |  |

<a id="inapppurchasesubmissionscreateinstance"></a>
# **InAppPurchaseSubmissionsCreateInstance**
> InAppPurchaseSubmissionResponse InAppPurchaseSubmissionsCreateInstance (InAppPurchaseSubmissionCreateRequest inAppPurchaseSubmissionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseSubmissionCreateRequest** | [**InAppPurchaseSubmissionCreateRequest**](InAppPurchaseSubmissionCreateRequest.md) | InAppPurchaseSubmission representation |  |

### Return type

[**InAppPurchaseSubmissionResponse**](InAppPurchaseSubmissionResponse.md)

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
| **201** | Single InAppPurchaseSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

