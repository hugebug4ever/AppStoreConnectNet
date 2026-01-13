# AppStoreConnect.Net.Api.InAppPurchaseOfferCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchaseOfferCodesCreateInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescreateinstance) | **POST** /v1/inAppPurchaseOfferCodes |  |
| [**InAppPurchaseOfferCodesCustomCodesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescustomcodesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/customCodes |  |
| [**InAppPurchaseOfferCodesCustomCodesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodescustomcodesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/customCodes |  |
| [**InAppPurchaseOfferCodesGetInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesgetinstance) | **GET** /v1/inAppPurchaseOfferCodes/{id} |  |
| [**InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesonetimeusecodesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/oneTimeUseCodes |  |
| [**InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesonetimeusecodesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/oneTimeUseCodes |  |
| [**InAppPurchaseOfferCodesPricesGetToManyRelated**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodespricesgettomanyrelated) | **GET** /v1/inAppPurchaseOfferCodes/{id}/prices |  |
| [**InAppPurchaseOfferCodesPricesGetToManyRelationship**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodespricesgettomanyrelationship) | **GET** /v1/inAppPurchaseOfferCodes/{id}/relationships/prices |  |
| [**InAppPurchaseOfferCodesUpdateInstance**](InAppPurchaseOfferCodesApi.md#inapppurchaseoffercodesupdateinstance) | **PATCH** /v1/inAppPurchaseOfferCodes/{id} |  |

<a id="inapppurchaseoffercodescreateinstance"></a>
# **InAppPurchaseOfferCodesCreateInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesCreateInstance (InAppPurchaseOfferCodeCreateRequest inAppPurchaseOfferCodeCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseOfferCodeCreateRequest** | [**InAppPurchaseOfferCodeCreateRequest**](InAppPurchaseOfferCodeCreateRequest.md) | InAppPurchaseOfferCode representation |  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **201** | Single InAppPurchaseOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodescustomcodesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesCustomCodesGetToManyRelated**
> InAppPurchaseOfferCodeCustomCodesResponse InAppPurchaseOfferCodesCustomCodesGetToManyRelated (string id, List<string> fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string> fieldsActors = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **fieldsActors** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type actors | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeCustomCodesResponse**](InAppPurchaseOfferCodeCustomCodesResponse.md)

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
| **200** | List of InAppPurchaseOfferCodeCustomCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodescustomcodesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesCustomCodesGetToManyRelationship**
> InAppPurchaseOfferCodeCustomCodesLinkagesResponse InAppPurchaseOfferCodesCustomCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseOfferCodeCustomCodesLinkagesResponse**](InAppPurchaseOfferCodeCustomCodesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodesgetinstance"></a>
# **InAppPurchaseOfferCodesGetInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesGetInstance (string id, List<string> fieldsInAppPurchaseOfferCodes = null, List<string> fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string> fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string> fieldsInAppPurchaseOfferPrices = null, List<string> include = null, int limitCustomCodes = null, int limitOneTimeUseCodes = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **fieldsInAppPurchaseOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferPrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCustomCodes** | **int** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitOneTimeUseCodes** | **int** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodesonetimeusecodesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated**
> InAppPurchaseOfferCodeOneTimeUseCodesResponse InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelated (string id, List<string> fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string> fieldsActors = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsActors** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type actors | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodesResponse**](InAppPurchaseOfferCodeOneTimeUseCodesResponse.md)

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
| **200** | List of InAppPurchaseOfferCodeOneTimeUseCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodesonetimeusecodesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship**
> InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse InAppPurchaseOfferCodesOneTimeUseCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse**](InAppPurchaseOfferCodeOneTimeUseCodesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodespricesgettomanyrelated"></a>
# **InAppPurchaseOfferCodesPricesGetToManyRelated**
> InAppPurchaseOfferPricesResponse InAppPurchaseOfferCodesPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsInAppPurchaseOfferPrices = null, List<string> fieldsTerritories = null, List<string> fieldsInAppPurchasePricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsInAppPurchaseOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseOfferPricesResponse**](InAppPurchaseOfferPricesResponse.md)

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
| **200** | List of InAppPurchaseOfferPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchaseoffercodespricesgettomanyrelationship"></a>
# **InAppPurchaseOfferCodesPricesGetToManyRelationship**
> InAppPurchaseOfferCodePricesLinkagesResponse InAppPurchaseOfferCodesPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseOfferCodePricesLinkagesResponse**](InAppPurchaseOfferCodePricesLinkagesResponse.md)

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

<a id="inapppurchaseoffercodesupdateinstance"></a>
# **InAppPurchaseOfferCodesUpdateInstance**
> InAppPurchaseOfferCodeResponse InAppPurchaseOfferCodesUpdateInstance (string id, InAppPurchaseOfferCodeUpdateRequest inAppPurchaseOfferCodeUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseOfferCodeUpdateRequest** | [**InAppPurchaseOfferCodeUpdateRequest**](InAppPurchaseOfferCodeUpdateRequest.md) | InAppPurchaseOfferCode representation |  |

### Return type

[**InAppPurchaseOfferCodeResponse**](InAppPurchaseOfferCodeResponse.md)

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
| **200** | Single InAppPurchaseOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

