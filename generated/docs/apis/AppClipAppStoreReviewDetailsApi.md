# AppStoreConnect.Net.Api.AppClipAppStoreReviewDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipAppStoreReviewDetailsCreateInstance**](AppClipAppStoreReviewDetailsApi.md#appclipappstorereviewdetailscreateinstance) | **POST** /v1/appClipAppStoreReviewDetails |  |
| [**AppClipAppStoreReviewDetailsGetInstance**](AppClipAppStoreReviewDetailsApi.md#appclipappstorereviewdetailsgetinstance) | **GET** /v1/appClipAppStoreReviewDetails/{id} |  |
| [**AppClipAppStoreReviewDetailsUpdateInstance**](AppClipAppStoreReviewDetailsApi.md#appclipappstorereviewdetailsupdateinstance) | **PATCH** /v1/appClipAppStoreReviewDetails/{id} |  |

<a id="appclipappstorereviewdetailscreateinstance"></a>
# **AppClipAppStoreReviewDetailsCreateInstance**
> AppClipAppStoreReviewDetailResponse AppClipAppStoreReviewDetailsCreateInstance (AppClipAppStoreReviewDetailCreateRequest appClipAppStoreReviewDetailCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appClipAppStoreReviewDetailCreateRequest** | [**AppClipAppStoreReviewDetailCreateRequest**](AppClipAppStoreReviewDetailCreateRequest.md) | AppClipAppStoreReviewDetail representation |  |

### Return type

[**AppClipAppStoreReviewDetailResponse**](AppClipAppStoreReviewDetailResponse.md)

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
| **201** | Single AppClipAppStoreReviewDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipappstorereviewdetailsgetinstance"></a>
# **AppClipAppStoreReviewDetailsGetInstance**
> AppClipAppStoreReviewDetailResponse AppClipAppStoreReviewDetailsGetInstance (string id, List<string> fieldsAppClipAppStoreReviewDetails = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppClipAppStoreReviewDetailResponse**](AppClipAppStoreReviewDetailResponse.md)

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
| **200** | Single AppClipAppStoreReviewDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipappstorereviewdetailsupdateinstance"></a>
# **AppClipAppStoreReviewDetailsUpdateInstance**
> AppClipAppStoreReviewDetailResponse AppClipAppStoreReviewDetailsUpdateInstance (string id, AppClipAppStoreReviewDetailUpdateRequest appClipAppStoreReviewDetailUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appClipAppStoreReviewDetailUpdateRequest** | [**AppClipAppStoreReviewDetailUpdateRequest**](AppClipAppStoreReviewDetailUpdateRequest.md) | AppClipAppStoreReviewDetail representation |  |

### Return type

[**AppClipAppStoreReviewDetailResponse**](AppClipAppStoreReviewDetailResponse.md)

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
| **200** | Single AppClipAppStoreReviewDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

