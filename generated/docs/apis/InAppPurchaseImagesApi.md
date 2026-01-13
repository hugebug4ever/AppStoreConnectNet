# AppStoreConnect.Net.Api.InAppPurchaseImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseImagesCreateInstance**](InAppPurchaseImagesApi.md#inapppurchaseimagescreateinstance) | **POST** /v1/inAppPurchaseImages |  |
| [**InAppPurchaseImagesDeleteInstance**](InAppPurchaseImagesApi.md#inapppurchaseimagesdeleteinstance) | **DELETE** /v1/inAppPurchaseImages/{id} |  |
| [**InAppPurchaseImagesGetInstance**](InAppPurchaseImagesApi.md#inapppurchaseimagesgetinstance) | **GET** /v1/inAppPurchaseImages/{id} |  |
| [**InAppPurchaseImagesUpdateInstance**](InAppPurchaseImagesApi.md#inapppurchaseimagesupdateinstance) | **PATCH** /v1/inAppPurchaseImages/{id} |  |

<a id="inapppurchaseimagescreateinstance"></a>
# **InAppPurchaseImagesCreateInstance**
> InAppPurchaseImageResponse InAppPurchaseImagesCreateInstance (InAppPurchaseImageCreateRequest inAppPurchaseImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseImageCreateRequest** | [**InAppPurchaseImageCreateRequest**](InAppPurchaseImageCreateRequest.md) | InAppPurchaseImage representation |  |

### Return type

[**InAppPurchaseImageResponse**](InAppPurchaseImageResponse.md)

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
| **201** | Single InAppPurchaseImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseimagesdeleteinstance"></a>
# **InAppPurchaseImagesDeleteInstance**
> void InAppPurchaseImagesDeleteInstance (string id)




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

<a id="inapppurchaseimagesgetinstance"></a>
# **InAppPurchaseImagesGetInstance**
> InAppPurchaseImageResponse InAppPurchaseImagesGetInstance (string id, List<string> fieldsInAppPurchaseImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseImageResponse**](InAppPurchaseImageResponse.md)

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
| **200** | Single InAppPurchaseImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseimagesupdateinstance"></a>
# **InAppPurchaseImagesUpdateInstance**
> InAppPurchaseImageResponse InAppPurchaseImagesUpdateInstance (string id, InAppPurchaseImageUpdateRequest inAppPurchaseImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseImageUpdateRequest** | [**InAppPurchaseImageUpdateRequest**](InAppPurchaseImageUpdateRequest.md) | InAppPurchaseImage representation |  |

### Return type

[**InAppPurchaseImageResponse**](InAppPurchaseImageResponse.md)

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
| **200** | Single InAppPurchaseImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

