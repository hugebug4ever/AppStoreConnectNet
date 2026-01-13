# AppStoreConnect.Net.Api.InAppPurchasePricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchasePricePointsEqualizationsGetToManyRelated**](InAppPurchasePricePointsApi.md#inapppurchasepricepointsequalizationsgettomanyrelated) | **GET** /v1/inAppPurchasePricePoints/{id}/equalizations |  |
| [**InAppPurchasePricePointsEqualizationsGetToManyRelationship**](InAppPurchasePricePointsApi.md#inapppurchasepricepointsequalizationsgettomanyrelationship) | **GET** /v1/inAppPurchasePricePoints/{id}/relationships/equalizations |  |

<a id="inapppurchasepricepointsequalizationsgettomanyrelated"></a>
# **InAppPurchasePricePointsEqualizationsGetToManyRelated**
> InAppPurchasePricePointsResponse InAppPurchasePricePointsEqualizationsGetToManyRelated (string id, List<string> filterTerritory = null, List<string> filterInAppPurchaseV2 = null, List<string> fieldsInAppPurchasePricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **filterInAppPurchaseV2** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;inAppPurchaseV2&#39; | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchasePricePointsResponse**](InAppPurchasePricePointsResponse.md)

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
| **200** | List of InAppPurchasePricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepricepointsequalizationsgettomanyrelationship"></a>
# **InAppPurchasePricePointsEqualizationsGetToManyRelationship**
> InAppPurchasePricePointEqualizationsLinkagesResponse InAppPurchasePricePointsEqualizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchasePricePointEqualizationsLinkagesResponse**](InAppPurchasePricePointEqualizationsLinkagesResponse.md)

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

