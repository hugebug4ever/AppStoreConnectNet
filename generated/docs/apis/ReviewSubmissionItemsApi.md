# AppStoreConnect.Net.Api.ReviewSubmissionItemsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ReviewSubmissionItemsCreateInstance**](ReviewSubmissionItemsApi.md#reviewsubmissionitemscreateinstance) | **POST** /v1/reviewSubmissionItems |  |
| [**ReviewSubmissionItemsDeleteInstance**](ReviewSubmissionItemsApi.md#reviewsubmissionitemsdeleteinstance) | **DELETE** /v1/reviewSubmissionItems/{id} |  |
| [**ReviewSubmissionItemsUpdateInstance**](ReviewSubmissionItemsApi.md#reviewsubmissionitemsupdateinstance) | **PATCH** /v1/reviewSubmissionItems/{id} |  |

<a id="reviewsubmissionitemscreateinstance"></a>
# **ReviewSubmissionItemsCreateInstance**
> ReviewSubmissionItemResponse ReviewSubmissionItemsCreateInstance (ReviewSubmissionItemCreateRequest reviewSubmissionItemCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **reviewSubmissionItemCreateRequest** | [**ReviewSubmissionItemCreateRequest**](ReviewSubmissionItemCreateRequest.md) | ReviewSubmissionItem representation |  |

### Return type

[**ReviewSubmissionItemResponse**](ReviewSubmissionItemResponse.md)

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
| **201** | Single ReviewSubmissionItem |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reviewsubmissionitemsdeleteinstance"></a>
# **ReviewSubmissionItemsDeleteInstance**
> void ReviewSubmissionItemsDeleteInstance (string id)




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

<a id="reviewsubmissionitemsupdateinstance"></a>
# **ReviewSubmissionItemsUpdateInstance**
> ReviewSubmissionItemResponse ReviewSubmissionItemsUpdateInstance (string id, ReviewSubmissionItemUpdateRequest reviewSubmissionItemUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **reviewSubmissionItemUpdateRequest** | [**ReviewSubmissionItemUpdateRequest**](ReviewSubmissionItemUpdateRequest.md) | ReviewSubmissionItem representation |  |

### Return type

[**ReviewSubmissionItemResponse**](ReviewSubmissionItemResponse.md)

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
| **200** | Single ReviewSubmissionItem |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

