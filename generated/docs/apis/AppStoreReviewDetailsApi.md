# AppStoreConnect.Net.Api.AppStoreReviewDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelated**](AppStoreReviewDetailsApi.md#appstorereviewdetailsappstorereviewattachmentsgettomanyrelated) | **GET** /v1/appStoreReviewDetails/{id}/appStoreReviewAttachments |  |
| [**AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelationship**](AppStoreReviewDetailsApi.md#appstorereviewdetailsappstorereviewattachmentsgettomanyrelationship) | **GET** /v1/appStoreReviewDetails/{id}/relationships/appStoreReviewAttachments |  |
| [**AppStoreReviewDetailsCreateInstance**](AppStoreReviewDetailsApi.md#appstorereviewdetailscreateinstance) | **POST** /v1/appStoreReviewDetails |  |
| [**AppStoreReviewDetailsGetInstance**](AppStoreReviewDetailsApi.md#appstorereviewdetailsgetinstance) | **GET** /v1/appStoreReviewDetails/{id} |  |
| [**AppStoreReviewDetailsUpdateInstance**](AppStoreReviewDetailsApi.md#appstorereviewdetailsupdateinstance) | **PATCH** /v1/appStoreReviewDetails/{id} |  |

<a id="appstorereviewdetailsappstorereviewattachmentsgettomanyrelated"></a>
# **AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelated**
> AppStoreReviewAttachmentsResponse AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelated (string id, List<string> fieldsAppStoreReviewAttachments = null, List<string> fieldsAppStoreReviewDetails = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreReviewAttachments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewAttachments | [optional]  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppStoreReviewAttachmentsResponse**](AppStoreReviewAttachmentsResponse.md)

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
| **200** | List of AppStoreReviewAttachments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstorereviewdetailsappstorereviewattachmentsgettomanyrelationship"></a>
# **AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelationship**
> AppStoreReviewDetailAppStoreReviewAttachmentsLinkagesResponse AppStoreReviewDetailsAppStoreReviewAttachmentsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreReviewDetailAppStoreReviewAttachmentsLinkagesResponse**](AppStoreReviewDetailAppStoreReviewAttachmentsLinkagesResponse.md)

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

<a id="appstorereviewdetailscreateinstance"></a>
# **AppStoreReviewDetailsCreateInstance**
> AppStoreReviewDetailResponse AppStoreReviewDetailsCreateInstance (AppStoreReviewDetailCreateRequest appStoreReviewDetailCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreReviewDetailCreateRequest** | [**AppStoreReviewDetailCreateRequest**](AppStoreReviewDetailCreateRequest.md) | AppStoreReviewDetail representation |  |

### Return type

[**AppStoreReviewDetailResponse**](AppStoreReviewDetailResponse.md)

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
| **201** | Single AppStoreReviewDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstorereviewdetailsgetinstance"></a>
# **AppStoreReviewDetailsGetInstance**
> AppStoreReviewDetailResponse AppStoreReviewDetailsGetInstance (string id, List<string> fieldsAppStoreReviewDetails = null, List<string> fieldsAppStoreReviewAttachments = null, List<string> include = null, int limitAppStoreReviewAttachments = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **fieldsAppStoreReviewAttachments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewAttachments | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreReviewAttachments** | **int** | maximum number of related appStoreReviewAttachments returned (when they are included) | [optional]  |

### Return type

[**AppStoreReviewDetailResponse**](AppStoreReviewDetailResponse.md)

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
| **200** | Single AppStoreReviewDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstorereviewdetailsupdateinstance"></a>
# **AppStoreReviewDetailsUpdateInstance**
> AppStoreReviewDetailResponse AppStoreReviewDetailsUpdateInstance (string id, AppStoreReviewDetailUpdateRequest appStoreReviewDetailUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreReviewDetailUpdateRequest** | [**AppStoreReviewDetailUpdateRequest**](AppStoreReviewDetailUpdateRequest.md) | AppStoreReviewDetail representation |  |

### Return type

[**AppStoreReviewDetailResponse**](AppStoreReviewDetailResponse.md)

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
| **200** | Single AppStoreReviewDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

