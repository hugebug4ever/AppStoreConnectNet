# AppStoreConnect.Net.Api.InAppPurchaseOfferCodeCustomCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodeCustomCodesCreateInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodeCustomCodes |  |
| [**InAppPurchaseOfferCodeCustomCodesGetInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodeCustomCodes/{id} |  |
| [**InAppPurchaseOfferCodeCustomCodesUpdateInstance**](InAppPurchaseOfferCodeCustomCodesApi.md#inapppurchaseoffercodecustomcodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodeCustomCodes/{id} |  |

<a id="inapppurchaseoffercodecustomcodescreateinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesCreateInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesCreateInstance (InAppPurchaseOfferCodeCustomCodeCreateRequest inAppPurchaseOfferCodeCustomCodeCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeCustomCodeCreateRequest** | [**InAppPurchaseOfferCodeCustomCodeCreateRequest**](InAppPurchaseOfferCodeCustomCodeCreateRequest.md) | InAppPurchaseOfferCodeCustomCode representation |  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodecustomcodesgetinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesGetInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesGetInstance (string id, List<string> fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodecustomcodesupdateinstance"></a>
# **InAppPurchaseOfferCodeCustomCodesUpdateInstance**
> InAppPurchaseOfferCodeCustomCodeResponse InAppPurchaseOfferCodeCustomCodesUpdateInstance (string id, InAppPurchaseOfferCodeCustomCodeUpdateRequest inAppPurchaseOfferCodeCustomCodeUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeCustomCodeUpdateRequest** | [**InAppPurchaseOfferCodeCustomCodeUpdateRequest**](InAppPurchaseOfferCodeCustomCodeUpdateRequest.md) | InAppPurchaseOfferCodeCustomCode representation |  |

### Return type

[**InAppPurchaseOfferCodeCustomCodeResponse**](InAppPurchaseOfferCodeCustomCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCodeCustomCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

