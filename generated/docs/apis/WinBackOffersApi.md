# AppStoreConnect.Net.Api.WinBackOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**WinBackOffersCreateInstance**](WinBackOffersApi.md#winbackofferscreateinstance) | **POST** /v1/winBackOffers |  |
| [**WinBackOffersDeleteInstance**](WinBackOffersApi.md#winbackoffersdeleteinstance) | **DELETE** /v1/winBackOffers/{id} |  |
| [**WinBackOffersGetInstance**](WinBackOffersApi.md#winbackoffersgetinstance) | **GET** /v1/winBackOffers/{id} |  |
| [**WinBackOffersPricesGetToManyRelated**](WinBackOffersApi.md#winbackofferspricesgettomanyrelated) | **GET** /v1/winBackOffers/{id}/prices |  |
| [**WinBackOffersPricesGetToManyRelationship**](WinBackOffersApi.md#winbackofferspricesgettomanyrelationship) | **GET** /v1/winBackOffers/{id}/relationships/prices |  |
| [**WinBackOffersUpdateInstance**](WinBackOffersApi.md#winbackoffersupdateinstance) | **PATCH** /v1/winBackOffers/{id} |  |

<a id="winbackofferscreateinstance"></a>
# **WinBackOffersCreateInstance**
> WinBackOfferResponse WinBackOffersCreateInstance (WinBackOfferCreateRequest winBackOfferCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **winBackOfferCreateRequest** | [**WinBackOfferCreateRequest**](WinBackOfferCreateRequest.md) | WinBackOffer representation |  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **201** | Single WinBackOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="winbackoffersdeleteinstance"></a>
# **WinBackOffersDeleteInstance**
> void WinBackOffersDeleteInstance (string id)




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

<a id="winbackoffersgetinstance"></a>
# **WinBackOffersGetInstance**
> WinBackOfferResponse WinBackOffersGetInstance (string id, List<string> fieldsWinBackOffers = null, List<string> fieldsWinBackOfferPrices = null, List<string> include = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **200** | Single WinBackOffer |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="winbackofferspricesgettomanyrelated"></a>
# **WinBackOffersPricesGetToManyRelated**
> WinBackOfferPricesResponse WinBackOffersPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsWinBackOfferPrices = null, List<string> fieldsTerritories = null, List<string> fieldsSubscriptionPricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**WinBackOfferPricesResponse**](WinBackOfferPricesResponse.md)

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
| **200** | List of WinBackOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="winbackofferspricesgettomanyrelationship"></a>
# **WinBackOffersPricesGetToManyRelationship**
> WinBackOfferPricesLinkagesResponse WinBackOffersPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**WinBackOfferPricesLinkagesResponse**](WinBackOfferPricesLinkagesResponse.md)

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

<a id="winbackoffersupdateinstance"></a>
# **WinBackOffersUpdateInstance**
> WinBackOfferResponse WinBackOffersUpdateInstance (string id, WinBackOfferUpdateRequest winBackOfferUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **winBackOfferUpdateRequest** | [**WinBackOfferUpdateRequest**](WinBackOfferUpdateRequest.md) | WinBackOffer representation |  |

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
| **200** | Single WinBackOffer |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

