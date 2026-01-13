# AppStoreConnect.Net.Api.SubscriptionAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesavailableterritoriesgettomanyrelated) | **GET** /v1/subscriptionAvailabilities/{id}/availableTerritories |  |
| [**SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesavailableterritoriesgettomanyrelationship) | **GET** /v1/subscriptionAvailabilities/{id}/relationships/availableTerritories |  |
| [**SubscriptionAvailabilitiesCreateInstance**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiescreateinstance) | **POST** /v1/subscriptionAvailabilities |  |
| [**SubscriptionAvailabilitiesGetInstance**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesgetinstance) | **GET** /v1/subscriptionAvailabilities/{id} |  |

<a id="subscriptionavailabilitiesavailableterritoriesgettomanyrelated"></a>
# **SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated**
> TerritoriesResponse SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated (string id, List<string> fieldsTerritories = null, int limit = null)




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

<a id="subscriptionavailabilitiesavailableterritoriesgettomanyrelationship"></a>
# **SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship**
> SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse**](SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.md)

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

<a id="subscriptionavailabilitiescreateinstance"></a>
# **SubscriptionAvailabilitiesCreateInstance**
> SubscriptionAvailabilityResponse SubscriptionAvailabilitiesCreateInstance (SubscriptionAvailabilityCreateRequest subscriptionAvailabilityCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionAvailabilityCreateRequest** | [**SubscriptionAvailabilityCreateRequest**](SubscriptionAvailabilityCreateRequest.md) | SubscriptionAvailability representation |  |

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
| **201** | Single SubscriptionAvailability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionavailabilitiesgetinstance"></a>
# **SubscriptionAvailabilitiesGetInstance**
> SubscriptionAvailabilityResponse SubscriptionAvailabilitiesGetInstance (string id, List<string> fieldsSubscriptionAvailabilities = null, List<string> fieldsTerritories = null, List<string> include = null, int limitAvailableTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAvailabilities | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAvailableTerritories** | **int** | maximum number of related availableTerritories returned (when they are included) | [optional]  |

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
| **200** | Single SubscriptionAvailability |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

