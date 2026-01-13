# AppStoreConnect.Net.Api.SubscriptionIntroductoryOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionIntroductoryOffersCreateInstance**](SubscriptionIntroductoryOffersApi.md#subscriptionintroductoryofferscreateinstance) | **POST** /v1/subscriptionIntroductoryOffers |  |
| [**SubscriptionIntroductoryOffersDeleteInstance**](SubscriptionIntroductoryOffersApi.md#subscriptionintroductoryoffersdeleteinstance) | **DELETE** /v1/subscriptionIntroductoryOffers/{id} |  |
| [**SubscriptionIntroductoryOffersUpdateInstance**](SubscriptionIntroductoryOffersApi.md#subscriptionintroductoryoffersupdateinstance) | **PATCH** /v1/subscriptionIntroductoryOffers/{id} |  |

<a id="subscriptionintroductoryofferscreateinstance"></a>
# **SubscriptionIntroductoryOffersCreateInstance**
> SubscriptionIntroductoryOfferResponse SubscriptionIntroductoryOffersCreateInstance (SubscriptionIntroductoryOfferCreateRequest subscriptionIntroductoryOfferCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionIntroductoryOfferCreateRequest** | [**SubscriptionIntroductoryOfferCreateRequest**](SubscriptionIntroductoryOfferCreateRequest.md) | SubscriptionIntroductoryOffer representation |  |

### Return type

[**SubscriptionIntroductoryOfferResponse**](SubscriptionIntroductoryOfferResponse.md)

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
| **201** | Single SubscriptionIntroductoryOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionintroductoryoffersdeleteinstance"></a>
# **SubscriptionIntroductoryOffersDeleteInstance**
> void SubscriptionIntroductoryOffersDeleteInstance (string id)




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

<a id="subscriptionintroductoryoffersupdateinstance"></a>
# **SubscriptionIntroductoryOffersUpdateInstance**
> SubscriptionIntroductoryOfferResponse SubscriptionIntroductoryOffersUpdateInstance (string id, SubscriptionIntroductoryOfferUpdateRequest subscriptionIntroductoryOfferUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionIntroductoryOfferUpdateRequest** | [**SubscriptionIntroductoryOfferUpdateRequest**](SubscriptionIntroductoryOfferUpdateRequest.md) | SubscriptionIntroductoryOffer representation |  |

### Return type

[**SubscriptionIntroductoryOfferResponse**](SubscriptionIntroductoryOfferResponse.md)

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
| **200** | Single SubscriptionIntroductoryOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

