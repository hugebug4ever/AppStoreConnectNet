# AppStoreConnect.Net.Api.CustomerReviewResponsesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CustomerReviewResponsesCreateInstance**](CustomerReviewResponsesApi.md#customerreviewresponsescreateinstance) | **POST** /v1/customerReviewResponses |  |
| [**CustomerReviewResponsesDeleteInstance**](CustomerReviewResponsesApi.md#customerreviewresponsesdeleteinstance) | **DELETE** /v1/customerReviewResponses/{id} |  |
| [**CustomerReviewResponsesGetInstance**](CustomerReviewResponsesApi.md#customerreviewresponsesgetinstance) | **GET** /v1/customerReviewResponses/{id} |  |

<a id="customerreviewresponsescreateinstance"></a>
# **CustomerReviewResponsesCreateInstance**
> CustomerReviewResponseV1Response CustomerReviewResponsesCreateInstance (CustomerReviewResponseV1CreateRequest customerReviewResponseV1CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **customerReviewResponseV1CreateRequest** | [**CustomerReviewResponseV1CreateRequest**](CustomerReviewResponseV1CreateRequest.md) | CustomerReviewResponse representation |  |

### Return type

[**CustomerReviewResponseV1Response**](CustomerReviewResponseV1Response.md)

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
| **201** | Single CustomerReviewResponse |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="customerreviewresponsesdeleteinstance"></a>
# **CustomerReviewResponsesDeleteInstance**
> void CustomerReviewResponsesDeleteInstance (string id)




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

<a id="customerreviewresponsesgetinstance"></a>
# **CustomerReviewResponsesGetInstance**
> CustomerReviewResponseV1Response CustomerReviewResponsesGetInstance (string id, List<string> fieldsCustomerReviewResponses = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCustomerReviewResponses** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type customerReviewResponses | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CustomerReviewResponseV1Response**](CustomerReviewResponseV1Response.md)

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
| **200** | Single CustomerReviewResponse |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

