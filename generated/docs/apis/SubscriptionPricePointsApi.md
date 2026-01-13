# AppStoreConnect.Net.Api.SubscriptionPricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionPricePointsEqualizationsGetToManyRelated**](SubscriptionPricePointsApi.md#subscriptionpricepointsequalizationsgettomanyrelated) | **GET** /v1/subscriptionPricePoints/{id}/equalizations |  |
| [**SubscriptionPricePointsEqualizationsGetToManyRelationship**](SubscriptionPricePointsApi.md#subscriptionpricepointsequalizationsgettomanyrelationship) | **GET** /v1/subscriptionPricePoints/{id}/relationships/equalizations |  |
| [**SubscriptionPricePointsGetInstance**](SubscriptionPricePointsApi.md#subscriptionpricepointsgetinstance) | **GET** /v1/subscriptionPricePoints/{id} |  |

<a id="subscriptionpricepointsequalizationsgettomanyrelated"></a>
# **SubscriptionPricePointsEqualizationsGetToManyRelated**
> SubscriptionPricePointsResponse SubscriptionPricePointsEqualizationsGetToManyRelated (string id, List<string> filterTerritory = null, List<string> filterSubscription = null, List<string> fieldsSubscriptionPricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **filterSubscription** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;subscription&#39; | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricePointsResponse**](SubscriptionPricePointsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of SubscriptionPricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionpricepointsequalizationsgettomanyrelationship"></a>
# **SubscriptionPricePointsEqualizationsGetToManyRelationship**
> SubscriptionPricePointEqualizationsLinkagesResponse SubscriptionPricePointsEqualizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionPricePointEqualizationsLinkagesResponse**](SubscriptionPricePointEqualizationsLinkagesResponse.md)

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

<a id="subscriptionpricepointsgetinstance"></a>
# **SubscriptionPricePointsGetInstance**
> SubscriptionPricePointResponse SubscriptionPricePointsGetInstance (string id, List<string> fieldsSubscriptionPricePoints = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricePointResponse**](SubscriptionPricePointResponse.md)

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
| **200** | Single SubscriptionPricePoint |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

