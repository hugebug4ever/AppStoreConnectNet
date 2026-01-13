# AppStoreConnect.Net.Api.CustomerReviewsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CustomerReviewsGetInstance**](CustomerReviewsApi.md#customerreviewsgetinstance) | **GET** /v1/customerReviews/{id} |  |
| [**CustomerReviewsResponseGetToOneRelated**](CustomerReviewsApi.md#customerreviewsresponsegettoonerelated) | **GET** /v1/customerReviews/{id}/response |  |
| [**CustomerReviewsResponseGetToOneRelationship**](CustomerReviewsApi.md#customerreviewsresponsegettoonerelationship) | **GET** /v1/customerReviews/{id}/relationships/response |  |

<a id="customerreviewsgetinstance"></a>
# **CustomerReviewsGetInstance**
> CustomerReviewResponse CustomerReviewsGetInstance (string id, List<string> fieldsCustomerReviews = null, List<string> fieldsCustomerReviewResponses = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCustomerReviews** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type customerReviews | [optional]  |
| **fieldsCustomerReviewResponses** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type customerReviewResponses | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CustomerReviewResponse**](CustomerReviewResponse.md)

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
| **200** | Single CustomerReview |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="customerreviewsresponsegettoonerelated"></a>
# **CustomerReviewsResponseGetToOneRelated**
> CustomerReviewResponseV1Response CustomerReviewsResponseGetToOneRelated (string id, List<string> fieldsCustomerReviewResponses = null, List<string> fieldsCustomerReviews = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCustomerReviewResponses** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type customerReviewResponses | [optional]  |
| **fieldsCustomerReviews** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type customerReviews | [optional]  |
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

<a id="customerreviewsresponsegettoonerelationship"></a>
# **CustomerReviewsResponseGetToOneRelationship**
> CustomerReviewResponseLinkageResponse CustomerReviewsResponseGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CustomerReviewResponseLinkageResponse**](CustomerReviewResponseLinkageResponse.md)

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

