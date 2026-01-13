# AppStoreConnect.Net.Api.SubscriptionPromotionalOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionPromotionalOffersCreateInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferscreateinstance) | **POST** /v1/subscriptionPromotionalOffers |  |
| [**SubscriptionPromotionalOffersDeleteInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersdeleteinstance) | **DELETE** /v1/subscriptionPromotionalOffers/{id} |  |
| [**SubscriptionPromotionalOffersGetInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersgetinstance) | **GET** /v1/subscriptionPromotionalOffers/{id} |  |
| [**SubscriptionPromotionalOffersPricesGetToManyRelated**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferspricesgettomanyrelated) | **GET** /v1/subscriptionPromotionalOffers/{id}/prices |  |
| [**SubscriptionPromotionalOffersPricesGetToManyRelationship**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionalofferspricesgettomanyrelationship) | **GET** /v1/subscriptionPromotionalOffers/{id}/relationships/prices |  |
| [**SubscriptionPromotionalOffersUpdateInstance**](SubscriptionPromotionalOffersApi.md#subscriptionpromotionaloffersupdateinstance) | **PATCH** /v1/subscriptionPromotionalOffers/{id} |  |

<a id="subscriptionpromotionalofferscreateinstance"></a>
# **SubscriptionPromotionalOffersCreateInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersCreateInstance (SubscriptionPromotionalOfferCreateRequest subscriptionPromotionalOfferCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionPromotionalOfferCreateRequest** | [**SubscriptionPromotionalOfferCreateRequest**](SubscriptionPromotionalOfferCreateRequest.md) | SubscriptionPromotionalOffer representation |  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **201** | Single SubscriptionPromotionalOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionpromotionaloffersdeleteinstance"></a>
# **SubscriptionPromotionalOffersDeleteInstance**
> void SubscriptionPromotionalOffersDeleteInstance (string id)




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

<a id="subscriptionpromotionaloffersgetinstance"></a>
# **SubscriptionPromotionalOffersGetInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersGetInstance (string id, List<string> fieldsSubscriptionPromotionalOffers = null, List<string> fieldsSubscriptionPromotionalOfferPrices = null, List<string> include = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **200** | Single SubscriptionPromotionalOffer |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionpromotionalofferspricesgettomanyrelated"></a>
# **SubscriptionPromotionalOffersPricesGetToManyRelated**
> SubscriptionPromotionalOfferPricesResponse SubscriptionPromotionalOffersPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionPromotionalOfferPrices = null, List<string> fieldsTerritories = null, List<string> fieldsSubscriptionPricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPromotionalOfferPricesResponse**](SubscriptionPromotionalOfferPricesResponse.md)

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
| **200** | List of SubscriptionPromotionalOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionpromotionalofferspricesgettomanyrelationship"></a>
# **SubscriptionPromotionalOffersPricesGetToManyRelationship**
> SubscriptionPromotionalOfferPricesLinkagesResponse SubscriptionPromotionalOffersPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionPromotionalOfferPricesLinkagesResponse**](SubscriptionPromotionalOfferPricesLinkagesResponse.md)

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

<a id="subscriptionpromotionaloffersupdateinstance"></a>
# **SubscriptionPromotionalOffersUpdateInstance**
> SubscriptionPromotionalOfferResponse SubscriptionPromotionalOffersUpdateInstance (string id, SubscriptionPromotionalOfferUpdateRequest subscriptionPromotionalOfferUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionPromotionalOfferUpdateRequest** | [**SubscriptionPromotionalOfferUpdateRequest**](SubscriptionPromotionalOfferUpdateRequest.md) | SubscriptionPromotionalOffer representation |  |

### Return type

[**SubscriptionPromotionalOfferResponse**](SubscriptionPromotionalOfferResponse.md)

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
| **200** | Single SubscriptionPromotionalOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

