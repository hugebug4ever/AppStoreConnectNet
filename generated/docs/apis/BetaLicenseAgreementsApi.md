# AppStoreConnect.Net.Api.BetaLicenseAgreementsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaLicenseAgreementsAppGetToOneRelated**](BetaLicenseAgreementsApi.md#betalicenseagreementsappgettoonerelated) | **GET** /v1/betaLicenseAgreements/{id}/app |  |
| [**BetaLicenseAgreementsAppGetToOneRelationship**](BetaLicenseAgreementsApi.md#betalicenseagreementsappgettoonerelationship) | **GET** /v1/betaLicenseAgreements/{id}/relationships/app |  |
| [**BetaLicenseAgreementsGetCollection**](BetaLicenseAgreementsApi.md#betalicenseagreementsgetcollection) | **GET** /v1/betaLicenseAgreements |  |
| [**BetaLicenseAgreementsGetInstance**](BetaLicenseAgreementsApi.md#betalicenseagreementsgetinstance) | **GET** /v1/betaLicenseAgreements/{id} |  |
| [**BetaLicenseAgreementsUpdateInstance**](BetaLicenseAgreementsApi.md#betalicenseagreementsupdateinstance) | **PATCH** /v1/betaLicenseAgreements/{id} |  |

<a id="betalicenseagreementsappgettoonerelated"></a>
# **BetaLicenseAgreementsAppGetToOneRelated**
> AppWithoutIncludesResponse BetaLicenseAgreementsAppGetToOneRelated (string id, List<string> fieldsApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betalicenseagreementsappgettoonerelationship"></a>
# **BetaLicenseAgreementsAppGetToOneRelationship**
> BetaLicenseAgreementAppLinkageResponse BetaLicenseAgreementsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaLicenseAgreementAppLinkageResponse**](BetaLicenseAgreementAppLinkageResponse.md)

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

<a id="betalicenseagreementsgetcollection"></a>
# **BetaLicenseAgreementsGetCollection**
> BetaLicenseAgreementsResponse BetaLicenseAgreementsGetCollection (List<string> filterApp = null, List<string> fieldsBetaLicenseAgreements = null, List<string> fieldsApps = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **fieldsBetaLicenseAgreements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaLicenseAgreements | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaLicenseAgreementsResponse**](BetaLicenseAgreementsResponse.md)

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
| **200** | List of BetaLicenseAgreements |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betalicenseagreementsgetinstance"></a>
# **BetaLicenseAgreementsGetInstance**
> BetaLicenseAgreementResponse BetaLicenseAgreementsGetInstance (string id, List<string> fieldsBetaLicenseAgreements = null, List<string> fieldsApps = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaLicenseAgreements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaLicenseAgreements | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaLicenseAgreementResponse**](BetaLicenseAgreementResponse.md)

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
| **200** | Single BetaLicenseAgreement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betalicenseagreementsupdateinstance"></a>
# **BetaLicenseAgreementsUpdateInstance**
> BetaLicenseAgreementResponse BetaLicenseAgreementsUpdateInstance (string id, BetaLicenseAgreementUpdateRequest betaLicenseAgreementUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaLicenseAgreementUpdateRequest** | [**BetaLicenseAgreementUpdateRequest**](BetaLicenseAgreementUpdateRequest.md) | BetaLicenseAgreement representation |  |

### Return type

[**BetaLicenseAgreementResponse**](BetaLicenseAgreementResponse.md)

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
| **200** | Single BetaLicenseAgreement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

