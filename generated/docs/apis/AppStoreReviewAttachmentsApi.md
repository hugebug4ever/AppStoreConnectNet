# AppStoreConnect.Net.Api.AppStoreReviewAttachmentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreReviewAttachmentsCreateInstance**](AppStoreReviewAttachmentsApi.md#appstorereviewattachmentscreateinstance) | **POST** /v1/appStoreReviewAttachments |  |
| [**AppStoreReviewAttachmentsDeleteInstance**](AppStoreReviewAttachmentsApi.md#appstorereviewattachmentsdeleteinstance) | **DELETE** /v1/appStoreReviewAttachments/{id} |  |
| [**AppStoreReviewAttachmentsGetInstance**](AppStoreReviewAttachmentsApi.md#appstorereviewattachmentsgetinstance) | **GET** /v1/appStoreReviewAttachments/{id} |  |
| [**AppStoreReviewAttachmentsUpdateInstance**](AppStoreReviewAttachmentsApi.md#appstorereviewattachmentsupdateinstance) | **PATCH** /v1/appStoreReviewAttachments/{id} |  |

<a id="appstorereviewattachmentscreateinstance"></a>
# **AppStoreReviewAttachmentsCreateInstance**
> AppStoreReviewAttachmentResponse AppStoreReviewAttachmentsCreateInstance (AppStoreReviewAttachmentCreateRequest appStoreReviewAttachmentCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreReviewAttachmentCreateRequest** | [**AppStoreReviewAttachmentCreateRequest**](AppStoreReviewAttachmentCreateRequest.md) | AppStoreReviewAttachment representation |  |

### Return type

[**AppStoreReviewAttachmentResponse**](AppStoreReviewAttachmentResponse.md)

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
| **201** | Single AppStoreReviewAttachment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstorereviewattachmentsdeleteinstance"></a>
# **AppStoreReviewAttachmentsDeleteInstance**
> void AppStoreReviewAttachmentsDeleteInstance (string id)




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

<a id="appstorereviewattachmentsgetinstance"></a>
# **AppStoreReviewAttachmentsGetInstance**
> AppStoreReviewAttachmentResponse AppStoreReviewAttachmentsGetInstance (string id, List<string> fieldsAppStoreReviewAttachments = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreReviewAttachments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewAttachments | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppStoreReviewAttachmentResponse**](AppStoreReviewAttachmentResponse.md)

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
| **200** | Single AppStoreReviewAttachment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstorereviewattachmentsupdateinstance"></a>
# **AppStoreReviewAttachmentsUpdateInstance**
> AppStoreReviewAttachmentResponse AppStoreReviewAttachmentsUpdateInstance (string id, AppStoreReviewAttachmentUpdateRequest appStoreReviewAttachmentUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreReviewAttachmentUpdateRequest** | [**AppStoreReviewAttachmentUpdateRequest**](AppStoreReviewAttachmentUpdateRequest.md) | AppStoreReviewAttachment representation |  |

### Return type

[**AppStoreReviewAttachmentResponse**](AppStoreReviewAttachmentResponse.md)

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
| **200** | Single AppStoreReviewAttachment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

