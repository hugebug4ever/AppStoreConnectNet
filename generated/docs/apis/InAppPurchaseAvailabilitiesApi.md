# AppStoreConnect.Net.Api.InAppPurchaseAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelated**](InAppPurchaseAvailabilitiesApi.md#inapppurchaseavailabilitiesavailableterritoriesgettomanyrelated) | **GET** /v1/inAppPurchaseAvailabilities/{id}/availableTerritories |  |
| [**InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelationship**](InAppPurchaseAvailabilitiesApi.md#inapppurchaseavailabilitiesavailableterritoriesgettomanyrelationship) | **GET** /v1/inAppPurchaseAvailabilities/{id}/relationships/availableTerritories |  |
| [**InAppPurchaseAvailabilitiesCreateInstance**](InAppPurchaseAvailabilitiesApi.md#inapppurchaseavailabilitiescreateinstance) | **POST** /v1/inAppPurchaseAvailabilities |  |
| [**InAppPurchaseAvailabilitiesGetInstance**](InAppPurchaseAvailabilitiesApi.md#inapppurchaseavailabilitiesgetinstance) | **GET** /v1/inAppPurchaseAvailabilities/{id} |  |

<a id="inapppurchaseavailabilitiesavailableterritoriesgettomanyrelated"></a>
# **InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelated**
> TerritoriesResponse InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelated (string id, List<string> fieldsTerritories = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**TerritoriesResponse**](TerritoriesResponse.md)

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
| **200** | List of Territories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseavailabilitiesavailableterritoriesgettomanyrelationship"></a>
# **InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelationship**
> InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse InAppPurchaseAvailabilitiesAvailableTerritoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse**](InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse.md)

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

<a id="inapppurchaseavailabilitiescreateinstance"></a>
# **InAppPurchaseAvailabilitiesCreateInstance**
> InAppPurchaseAvailabilityResponse InAppPurchaseAvailabilitiesCreateInstance (InAppPurchaseAvailabilityCreateRequest inAppPurchaseAvailabilityCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseAvailabilityCreateRequest** | [**InAppPurchaseAvailabilityCreateRequest**](InAppPurchaseAvailabilityCreateRequest.md) | InAppPurchaseAvailability representation |  |

### Return type

[**InAppPurchaseAvailabilityResponse**](InAppPurchaseAvailabilityResponse.md)

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
| **201** | Single InAppPurchaseAvailability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseavailabilitiesgetinstance"></a>
# **InAppPurchaseAvailabilitiesGetInstance**
> InAppPurchaseAvailabilityResponse InAppPurchaseAvailabilitiesGetInstance (string id, List<string> fieldsInAppPurchaseAvailabilities = null, List<string> fieldsTerritories = null, List<string> include = null, int limitAvailableTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseAvailabilities | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAvailableTerritories** | **int** | maximum number of related availableTerritories returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseAvailabilityResponse**](InAppPurchaseAvailabilityResponse.md)

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
| **200** | Single InAppPurchaseAvailability |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

