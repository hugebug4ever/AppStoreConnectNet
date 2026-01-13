# AppStoreConnect.Net.Api.SubscriptionImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionImagesCreateInstance**](SubscriptionImagesApi.md#subscriptionimagescreateinstance) | **POST** /v1/subscriptionImages |  |
| [**SubscriptionImagesDeleteInstance**](SubscriptionImagesApi.md#subscriptionimagesdeleteinstance) | **DELETE** /v1/subscriptionImages/{id} |  |
| [**SubscriptionImagesGetInstance**](SubscriptionImagesApi.md#subscriptionimagesgetinstance) | **GET** /v1/subscriptionImages/{id} |  |
| [**SubscriptionImagesUpdateInstance**](SubscriptionImagesApi.md#subscriptionimagesupdateinstance) | **PATCH** /v1/subscriptionImages/{id} |  |

<a id="subscriptionimagescreateinstance"></a>
# **SubscriptionImagesCreateInstance**
> SubscriptionImageResponse SubscriptionImagesCreateInstance (SubscriptionImageCreateRequest subscriptionImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionImageCreateRequest** | [**SubscriptionImageCreateRequest**](SubscriptionImageCreateRequest.md) | SubscriptionImage representation |  |

### Return type

[**SubscriptionImageResponse**](SubscriptionImageResponse.md)

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
| **201** | Single SubscriptionImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionimagesdeleteinstance"></a>
# **SubscriptionImagesDeleteInstance**
> void SubscriptionImagesDeleteInstance (string id)




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

<a id="subscriptionimagesgetinstance"></a>
# **SubscriptionImagesGetInstance**
> SubscriptionImageResponse SubscriptionImagesGetInstance (string id, List<string> fieldsSubscriptionImages = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionImageResponse**](SubscriptionImageResponse.md)

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
| **200** | Single SubscriptionImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionimagesupdateinstance"></a>
# **SubscriptionImagesUpdateInstance**
> SubscriptionImageResponse SubscriptionImagesUpdateInstance (string id, SubscriptionImageUpdateRequest subscriptionImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionImageUpdateRequest** | [**SubscriptionImageUpdateRequest**](SubscriptionImageUpdateRequest.md) | SubscriptionImage representation |  |

### Return type

[**SubscriptionImageResponse**](SubscriptionImageResponse.md)

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
| **200** | Single SubscriptionImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

