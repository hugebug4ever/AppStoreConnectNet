# AppStoreConnect.Net.Api.AppAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppAvailabilitiesV2CreateInstance**](AppAvailabilitiesApi.md#appavailabilitiesv2createinstance) | **POST** /v2/appAvailabilities |  |
| [**AppAvailabilitiesV2GetInstance**](AppAvailabilitiesApi.md#appavailabilitiesv2getinstance) | **GET** /v2/appAvailabilities/{id} |  |
| [**AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelated**](AppAvailabilitiesApi.md#appavailabilitiesv2territoryavailabilitiesgettomanyrelated) | **GET** /v2/appAvailabilities/{id}/territoryAvailabilities |  |
| [**AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelationship**](AppAvailabilitiesApi.md#appavailabilitiesv2territoryavailabilitiesgettomanyrelationship) | **GET** /v2/appAvailabilities/{id}/relationships/territoryAvailabilities |  |

<a id="appavailabilitiesv2createinstance"></a>
# **AppAvailabilitiesV2CreateInstance**
> AppAvailabilityV2Response AppAvailabilitiesV2CreateInstance (AppAvailabilityV2CreateRequest appAvailabilityV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appAvailabilityV2CreateRequest** | [**AppAvailabilityV2CreateRequest**](AppAvailabilityV2CreateRequest.md) | AppAvailability representation |  |

### Return type

[**AppAvailabilityV2Response**](AppAvailabilityV2Response.md)

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
| **201** | Single AppAvailability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appavailabilitiesv2getinstance"></a>
# **AppAvailabilitiesV2GetInstance**
> AppAvailabilityV2Response AppAvailabilitiesV2GetInstance (string id, List<string> fieldsAppAvailabilities = null, List<string> fieldsTerritoryAvailabilities = null, List<string> include = null, int limitTerritoryAvailabilities = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appAvailabilities | [optional]  |
| **fieldsTerritoryAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territoryAvailabilities | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitTerritoryAvailabilities** | **int** | maximum number of related territoryAvailabilities returned (when they are included) | [optional]  |

### Return type

[**AppAvailabilityV2Response**](AppAvailabilityV2Response.md)

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
| **200** | Single AppAvailability |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appavailabilitiesv2territoryavailabilitiesgettomanyrelated"></a>
# **AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelated**
> TerritoryAvailabilitiesResponse AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelated (string id, List<string> fieldsTerritoryAvailabilities = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritoryAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territoryAvailabilities | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**TerritoryAvailabilitiesResponse**](TerritoryAvailabilitiesResponse.md)

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
| **200** | List of TerritoryAvailabilities |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appavailabilitiesv2territoryavailabilitiesgettomanyrelationship"></a>
# **AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelationship**
> AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse AppAvailabilitiesV2TerritoryAvailabilitiesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse**](AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse.md)

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

