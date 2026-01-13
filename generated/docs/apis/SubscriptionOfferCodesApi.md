# AppStoreConnect.Net.Api.SubscriptionOfferCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionOfferCodesCreateInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodescreateinstance) | **POST** /v1/subscriptionOfferCodes |  |
| [**SubscriptionOfferCodesCustomCodesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodescustomcodesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/customCodes |  |
| [**SubscriptionOfferCodesCustomCodesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodescustomcodesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/customCodes |  |
| [**SubscriptionOfferCodesGetInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodesgetinstance) | **GET** /v1/subscriptionOfferCodes/{id} |  |
| [**SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodesonetimeusecodesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/oneTimeUseCodes |  |
| [**SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodesonetimeusecodesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/oneTimeUseCodes |  |
| [**SubscriptionOfferCodesPricesGetToManyRelated**](SubscriptionOfferCodesApi.md#subscriptionoffercodespricesgettomanyrelated) | **GET** /v1/subscriptionOfferCodes/{id}/prices |  |
| [**SubscriptionOfferCodesPricesGetToManyRelationship**](SubscriptionOfferCodesApi.md#subscriptionoffercodespricesgettomanyrelationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/prices |  |
| [**SubscriptionOfferCodesUpdateInstance**](SubscriptionOfferCodesApi.md#subscriptionoffercodesupdateinstance) | **PATCH** /v1/subscriptionOfferCodes/{id} |  |

<a id="subscriptionoffercodescreateinstance"></a>
# **SubscriptionOfferCodesCreateInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesCreateInstance (SubscriptionOfferCodeCreateRequest subscriptionOfferCodeCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionOfferCodeCreateRequest** | [**SubscriptionOfferCodeCreateRequest**](SubscriptionOfferCodeCreateRequest.md) | SubscriptionOfferCode representation |  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **201** | Single SubscriptionOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionoffercodescustomcodesgettomanyrelated"></a>
# **SubscriptionOfferCodesCustomCodesGetToManyRelated**
> SubscriptionOfferCodeCustomCodesResponse SubscriptionOfferCodesCustomCodesGetToManyRelated (string id, List<string> fieldsSubscriptionOfferCodeCustomCodes = null, List<string> fieldsSubscriptionOfferCodes = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodeCustomCodesResponse**](SubscriptionOfferCodeCustomCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodeCustomCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionoffercodescustomcodesgettomanyrelationship"></a>
# **SubscriptionOfferCodesCustomCodesGetToManyRelationship**
> SubscriptionOfferCodeCustomCodesLinkagesResponse SubscriptionOfferCodesCustomCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionOfferCodeCustomCodesLinkagesResponse**](SubscriptionOfferCodeCustomCodesLinkagesResponse.md)

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

<a id="subscriptionoffercodesgetinstance"></a>
# **SubscriptionOfferCodesGetInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesGetInstance (string id, List<string> fieldsSubscriptionOfferCodes = null, List<string> fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string> fieldsSubscriptionOfferCodeCustomCodes = null, List<string> fieldsSubscriptionOfferCodePrices = null, List<string> include = null, int limitCustomCodes = null, int limitOneTimeUseCodes = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCustomCodes** | **int** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitOneTimeUseCodes** | **int** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **200** | Single SubscriptionOfferCode |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionoffercodesonetimeusecodesgettomanyrelated"></a>
# **SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated**
> SubscriptionOfferCodeOneTimeUseCodesResponse SubscriptionOfferCodesOneTimeUseCodesGetToManyRelated (string id, List<string> fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string> fieldsSubscriptionOfferCodes = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodeOneTimeUseCodesResponse**](SubscriptionOfferCodeOneTimeUseCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodeOneTimeUseCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionoffercodesonetimeusecodesgettomanyrelationship"></a>
# **SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship**
> SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse SubscriptionOfferCodesOneTimeUseCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse**](SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.md)

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

<a id="subscriptionoffercodespricesgettomanyrelated"></a>
# **SubscriptionOfferCodesPricesGetToManyRelated**
> SubscriptionOfferCodePricesResponse SubscriptionOfferCodesPricesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionOfferCodePrices = null, List<string> fieldsTerritories = null, List<string> fieldsSubscriptionPricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionOfferCodePricesResponse**](SubscriptionOfferCodePricesResponse.md)

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
| **200** | List of SubscriptionOfferCodePrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionoffercodespricesgettomanyrelationship"></a>
# **SubscriptionOfferCodesPricesGetToManyRelationship**
> SubscriptionOfferCodePricesLinkagesResponse SubscriptionOfferCodesPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionOfferCodePricesLinkagesResponse**](SubscriptionOfferCodePricesLinkagesResponse.md)

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

<a id="subscriptionoffercodesupdateinstance"></a>
# **SubscriptionOfferCodesUpdateInstance**
> SubscriptionOfferCodeResponse SubscriptionOfferCodesUpdateInstance (string id, SubscriptionOfferCodeUpdateRequest subscriptionOfferCodeUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionOfferCodeUpdateRequest** | [**SubscriptionOfferCodeUpdateRequest**](SubscriptionOfferCodeUpdateRequest.md) | SubscriptionOfferCode representation |  |

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
| **200** | Single SubscriptionOfferCode |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

