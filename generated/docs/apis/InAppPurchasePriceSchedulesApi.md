# AppStoreConnect.Net.Api.InAppPurchasePriceSchedulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelated**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesautomaticpricesgettomanyrelated) | **GET** /v1/inAppPurchasePriceSchedules/{id}/automaticPrices |  |
| [**InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelationship**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesautomaticpricesgettomanyrelationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/automaticPrices |  |
| [**InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelated**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesbaseterritorygettoonerelated) | **GET** /v1/inAppPurchasePriceSchedules/{id}/baseTerritory |  |
| [**InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelationship**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesbaseterritorygettoonerelationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/baseTerritory |  |
| [**InAppPurchasePriceSchedulesCreateInstance**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulescreateinstance) | **POST** /v1/inAppPurchasePriceSchedules |  |
| [**InAppPurchasePriceSchedulesGetInstance**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesgetinstance) | **GET** /v1/inAppPurchasePriceSchedules/{id} |  |
| [**InAppPurchasePriceSchedulesManualPricesGetToManyRelated**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesmanualpricesgettomanyrelated) | **GET** /v1/inAppPurchasePriceSchedules/{id}/manualPrices |  |
| [**InAppPurchasePriceSchedulesManualPricesGetToManyRelationship**](InAppPurchasePriceSchedulesApi.md#inapppurchasepriceschedulesmanualpricesgettomanyrelationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/manualPrices |  |

<a id="inapppurchasepriceschedulesautomaticpricesgettomanyrelated"></a>
# **InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelated**
> InAppPurchasePricesResponse InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsInAppPurchasePrices = null, List<string> fieldsInAppPurchasePricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsInAppPurchasePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePrices | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchasePricesResponse**](InAppPurchasePricesResponse.md)

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
| **200** | List of InAppPurchasePrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepriceschedulesautomaticpricesgettomanyrelationship"></a>
# **InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelationship**
> InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse InAppPurchasePriceSchedulesAutomaticPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse**](InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse.md)

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

<a id="inapppurchasepriceschedulesbaseterritorygettoonerelated"></a>
# **InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelated**
> TerritoryResponse InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelated (string id, List<string> fieldsTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |

### Return type

[**TerritoryResponse**](TerritoryResponse.md)

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
| **200** | Single Territory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepriceschedulesbaseterritorygettoonerelationship"></a>
# **InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelationship**
> InAppPurchasePriceScheduleBaseTerritoryLinkageResponse InAppPurchasePriceSchedulesBaseTerritoryGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchasePriceScheduleBaseTerritoryLinkageResponse**](InAppPurchasePriceScheduleBaseTerritoryLinkageResponse.md)

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

<a id="inapppurchasepriceschedulescreateinstance"></a>
# **InAppPurchasePriceSchedulesCreateInstance**
> InAppPurchasePriceScheduleResponse InAppPurchasePriceSchedulesCreateInstance (InAppPurchasePriceScheduleCreateRequest inAppPurchasePriceScheduleCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchasePriceScheduleCreateRequest** | [**InAppPurchasePriceScheduleCreateRequest**](InAppPurchasePriceScheduleCreateRequest.md) | InAppPurchasePriceSchedule representation |  |

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

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
| **201** | Single InAppPurchasePriceSchedule |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepriceschedulesgetinstance"></a>
# **InAppPurchasePriceSchedulesGetInstance**
> InAppPurchasePriceScheduleResponse InAppPurchasePriceSchedulesGetInstance (string id, List<string> fieldsInAppPurchasePriceSchedules = null, List<string> fieldsTerritories = null, List<string> fieldsInAppPurchasePrices = null, List<string> include = null, int limitAutomaticPrices = null, int limitManualPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchasePriceSchedules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsInAppPurchasePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAutomaticPrices** | **int** | maximum number of related automaticPrices returned (when they are included) | [optional]  |
| **limitManualPrices** | **int** | maximum number of related manualPrices returned (when they are included) | [optional]  |

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

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
| **200** | Single InAppPurchasePriceSchedule |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepriceschedulesmanualpricesgettomanyrelated"></a>
# **InAppPurchasePriceSchedulesManualPricesGetToManyRelated**
> InAppPurchasePricesResponse InAppPurchasePriceSchedulesManualPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsInAppPurchasePrices = null, List<string> fieldsInAppPurchasePricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsInAppPurchasePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePrices | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchasePricesResponse**](InAppPurchasePricesResponse.md)

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
| **200** | List of InAppPurchasePrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasepriceschedulesmanualpricesgettomanyrelationship"></a>
# **InAppPurchasePriceSchedulesManualPricesGetToManyRelationship**
> InAppPurchasePriceScheduleManualPricesLinkagesResponse InAppPurchasePriceSchedulesManualPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchasePriceScheduleManualPricesLinkagesResponse**](InAppPurchasePriceScheduleManualPricesLinkagesResponse.md)

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

