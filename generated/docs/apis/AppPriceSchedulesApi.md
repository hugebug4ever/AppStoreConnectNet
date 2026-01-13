# AppStoreConnect.Net.Api.AppPriceSchedulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppPriceSchedulesAutomaticPricesGetToManyRelated**](AppPriceSchedulesApi.md#apppriceschedulesautomaticpricesgettomanyrelated) | **GET** /v1/appPriceSchedules/{id}/automaticPrices |  |
| [**AppPriceSchedulesAutomaticPricesGetToManyRelationship**](AppPriceSchedulesApi.md#apppriceschedulesautomaticpricesgettomanyrelationship) | **GET** /v1/appPriceSchedules/{id}/relationships/automaticPrices |  |
| [**AppPriceSchedulesBaseTerritoryGetToOneRelated**](AppPriceSchedulesApi.md#apppriceschedulesbaseterritorygettoonerelated) | **GET** /v1/appPriceSchedules/{id}/baseTerritory |  |
| [**AppPriceSchedulesBaseTerritoryGetToOneRelationship**](AppPriceSchedulesApi.md#apppriceschedulesbaseterritorygettoonerelationship) | **GET** /v1/appPriceSchedules/{id}/relationships/baseTerritory |  |
| [**AppPriceSchedulesCreateInstance**](AppPriceSchedulesApi.md#apppriceschedulescreateinstance) | **POST** /v1/appPriceSchedules |  |
| [**AppPriceSchedulesGetInstance**](AppPriceSchedulesApi.md#apppriceschedulesgetinstance) | **GET** /v1/appPriceSchedules/{id} |  |
| [**AppPriceSchedulesManualPricesGetToManyRelated**](AppPriceSchedulesApi.md#apppriceschedulesmanualpricesgettomanyrelated) | **GET** /v1/appPriceSchedules/{id}/manualPrices |  |
| [**AppPriceSchedulesManualPricesGetToManyRelationship**](AppPriceSchedulesApi.md#apppriceschedulesmanualpricesgettomanyrelationship) | **GET** /v1/appPriceSchedules/{id}/relationships/manualPrices |  |

<a id="apppriceschedulesautomaticpricesgettomanyrelated"></a>
# **AppPriceSchedulesAutomaticPricesGetToManyRelated**
> AppPricesV2Response AppPriceSchedulesAutomaticPricesGetToManyRelated (string id, List<string> filterStartDate = null, List<string> filterEndDate = null, List<string> filterTerritory = null, List<string> fieldsAppPrices = null, List<string> fieldsAppPricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterStartDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;startDate&#39; | [optional]  |
| **filterEndDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;endDate&#39; | [optional]  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsAppPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPrices | [optional]  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricesV2Response**](AppPricesV2Response.md)

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
| **200** | List of AppPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppriceschedulesautomaticpricesgettomanyrelationship"></a>
# **AppPriceSchedulesAutomaticPricesGetToManyRelationship**
> AppPriceScheduleAutomaticPricesLinkagesResponse AppPriceSchedulesAutomaticPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppPriceScheduleAutomaticPricesLinkagesResponse**](AppPriceScheduleAutomaticPricesLinkagesResponse.md)

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

<a id="apppriceschedulesbaseterritorygettoonerelated"></a>
# **AppPriceSchedulesBaseTerritoryGetToOneRelated**
> TerritoryResponse AppPriceSchedulesBaseTerritoryGetToOneRelated (string id, List<string> fieldsTerritories = null)




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

<a id="apppriceschedulesbaseterritorygettoonerelationship"></a>
# **AppPriceSchedulesBaseTerritoryGetToOneRelationship**
> AppPriceScheduleBaseTerritoryLinkageResponse AppPriceSchedulesBaseTerritoryGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppPriceScheduleBaseTerritoryLinkageResponse**](AppPriceScheduleBaseTerritoryLinkageResponse.md)

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

<a id="apppriceschedulescreateinstance"></a>
# **AppPriceSchedulesCreateInstance**
> AppPriceScheduleResponse AppPriceSchedulesCreateInstance (AppPriceScheduleCreateRequest appPriceScheduleCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appPriceScheduleCreateRequest** | [**AppPriceScheduleCreateRequest**](AppPriceScheduleCreateRequest.md) | AppPriceSchedule representation |  |

### Return type

[**AppPriceScheduleResponse**](AppPriceScheduleResponse.md)

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
| **201** | Single AppPriceSchedule |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppriceschedulesgetinstance"></a>
# **AppPriceSchedulesGetInstance**
> AppPriceScheduleResponse AppPriceSchedulesGetInstance (string id, List<string> fieldsAppPriceSchedules = null, List<string> fieldsTerritories = null, List<string> fieldsAppPrices = null, List<string> include = null, int limitAutomaticPrices = null, int limitManualPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppPriceSchedules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPriceSchedules | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsAppPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAutomaticPrices** | **int** | maximum number of related automaticPrices returned (when they are included) | [optional]  |
| **limitManualPrices** | **int** | maximum number of related manualPrices returned (when they are included) | [optional]  |

### Return type

[**AppPriceScheduleResponse**](AppPriceScheduleResponse.md)

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
| **200** | Single AppPriceSchedule |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppriceschedulesmanualpricesgettomanyrelated"></a>
# **AppPriceSchedulesManualPricesGetToManyRelated**
> AppPricesV2Response AppPriceSchedulesManualPricesGetToManyRelated (string id, List<string> filterStartDate = null, List<string> filterEndDate = null, List<string> filterTerritory = null, List<string> fieldsAppPrices = null, List<string> fieldsAppPricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterStartDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;startDate&#39; | [optional]  |
| **filterEndDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;endDate&#39; | [optional]  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsAppPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPrices | [optional]  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricesV2Response**](AppPricesV2Response.md)

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
| **200** | List of AppPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppriceschedulesmanualpricesgettomanyrelationship"></a>
# **AppPriceSchedulesManualPricesGetToManyRelationship**
> AppPriceScheduleManualPricesLinkagesResponse AppPriceSchedulesManualPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppPriceScheduleManualPricesLinkagesResponse**](AppPriceScheduleManualPricesLinkagesResponse.md)

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

