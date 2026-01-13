# AppStoreConnect.Net.Api.EndUserLicenseAgreementsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**EndUserLicenseAgreementsCreateInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementscreateinstance) | **POST** /v1/endUserLicenseAgreements |  |
| [**EndUserLicenseAgreementsDeleteInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsdeleteinstance) | **DELETE** /v1/endUserLicenseAgreements/{id} |  |
| [**EndUserLicenseAgreementsGetInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsgetinstance) | **GET** /v1/endUserLicenseAgreements/{id} |  |
| [**EndUserLicenseAgreementsTerritoriesGetToManyRelated**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsterritoriesgettomanyrelated) | **GET** /v1/endUserLicenseAgreements/{id}/territories |  |
| [**EndUserLicenseAgreementsTerritoriesGetToManyRelationship**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsterritoriesgettomanyrelationship) | **GET** /v1/endUserLicenseAgreements/{id}/relationships/territories |  |
| [**EndUserLicenseAgreementsUpdateInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsupdateinstance) | **PATCH** /v1/endUserLicenseAgreements/{id} |  |

<a id="enduserlicenseagreementscreateinstance"></a>
# **EndUserLicenseAgreementsCreateInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsCreateInstance (EndUserLicenseAgreementCreateRequest endUserLicenseAgreementCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **endUserLicenseAgreementCreateRequest** | [**EndUserLicenseAgreementCreateRequest**](EndUserLicenseAgreementCreateRequest.md) | EndUserLicenseAgreement representation |  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **201** | Single EndUserLicenseAgreement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="enduserlicenseagreementsdeleteinstance"></a>
# **EndUserLicenseAgreementsDeleteInstance**
> void EndUserLicenseAgreementsDeleteInstance (string id)




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

<a id="enduserlicenseagreementsgetinstance"></a>
# **EndUserLicenseAgreementsGetInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsGetInstance (string id, List<string> fieldsEndUserLicenseAgreements = null, List<string> fieldsTerritories = null, List<string> include = null, int limitTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsEndUserLicenseAgreements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type endUserLicenseAgreements | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitTerritories** | **int** | maximum number of related territories returned (when they are included) | [optional]  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **200** | Single EndUserLicenseAgreement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="enduserlicenseagreementsterritoriesgettomanyrelated"></a>
# **EndUserLicenseAgreementsTerritoriesGetToManyRelated**
> TerritoriesWithoutIncludesResponse EndUserLicenseAgreementsTerritoriesGetToManyRelated (string id, List<string> fieldsTerritories = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**TerritoriesWithoutIncludesResponse**](TerritoriesWithoutIncludesResponse.md)

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
| **200** | List of Territories with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="enduserlicenseagreementsterritoriesgettomanyrelationship"></a>
# **EndUserLicenseAgreementsTerritoriesGetToManyRelationship**
> EndUserLicenseAgreementTerritoriesLinkagesResponse EndUserLicenseAgreementsTerritoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**EndUserLicenseAgreementTerritoriesLinkagesResponse**](EndUserLicenseAgreementTerritoriesLinkagesResponse.md)

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

<a id="enduserlicenseagreementsupdateinstance"></a>
# **EndUserLicenseAgreementsUpdateInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsUpdateInstance (string id, EndUserLicenseAgreementUpdateRequest endUserLicenseAgreementUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **endUserLicenseAgreementUpdateRequest** | [**EndUserLicenseAgreementUpdateRequest**](EndUserLicenseAgreementUpdateRequest.md) | EndUserLicenseAgreement representation |  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **200** | Single EndUserLicenseAgreement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

