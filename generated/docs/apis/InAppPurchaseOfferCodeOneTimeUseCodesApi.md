# AppStoreConnect.Net.Api.InAppPurchaseOfferCodeOneTimeUseCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodeOneTimeUseCodes |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesGetInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id} |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id} |  |
| [**InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated**](InAppPurchaseOfferCodeOneTimeUseCodesApi.md#inapppurchaseoffercodeonetimeusecodesvaluesgettoonerelated) | **GET** /v1/inAppPurchaseOfferCodeOneTimeUseCodes/{id}/values |  |

<a id="inapppurchaseoffercodeonetimeusecodescreateinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesCreateInstance (InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeOneTimeUseCodeCreateRequest** | [**InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest**](InAppPurchaseOfferCodeOneTimeUseCodeCreateRequest.md) | InAppPurchaseOfferCodeOneTimeUseCode representation |  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesgetinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesGetInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesGetInstance (string id, List<string> fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesupdateinstance"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance**
> InAppPurchaseOfferCodeOneTimeUseCodeResponse InAppPurchaseOfferCodeOneTimeUseCodesUpdateInstance (string id, InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest** | [**InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest**](InAppPurchaseOfferCodeOneTimeUseCodeUpdateRequest.md) | InAppPurchaseOfferCodeOneTimeUseCode representation |  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodeResponse**](InAppPurchaseOfferCodeOneTimeUseCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodeonetimeusecodesvaluesgettoonerelated"></a>
# **InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated**
> string InAppPurchaseOfferCodeOneTimeUseCodesValuesGetToOneRelated (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

**string**

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
| **200** | Single InAppPurchaseOfferCodeOneTimeUseCodeValue |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

