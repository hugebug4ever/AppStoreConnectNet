# AppStoreConnect.Net.Api.InAppPurchasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InAppPurchasesGetInstance**](InAppPurchasesApi.md#inapppurchasesgetinstance) | **GET** /v1/inAppPurchases/{id} |  |
| [**InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelated**](InAppPurchasesApi.md#inapppurchasesv2appstorereviewscreenshotgettoonerelated) | **GET** /v2/inAppPurchases/{id}/appStoreReviewScreenshot |  |
| [**InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelationship**](InAppPurchasesApi.md#inapppurchasesv2appstorereviewscreenshotgettoonerelationship) | **GET** /v2/inAppPurchases/{id}/relationships/appStoreReviewScreenshot |  |
| [**InAppPurchasesV2ContentGetToOneRelated**](InAppPurchasesApi.md#inapppurchasesv2contentgettoonerelated) | **GET** /v2/inAppPurchases/{id}/content |  |
| [**InAppPurchasesV2ContentGetToOneRelationship**](InAppPurchasesApi.md#inapppurchasesv2contentgettoonerelationship) | **GET** /v2/inAppPurchases/{id}/relationships/content |  |
| [**InAppPurchasesV2CreateInstance**](InAppPurchasesApi.md#inapppurchasesv2createinstance) | **POST** /v2/inAppPurchases |  |
| [**InAppPurchasesV2DeleteInstance**](InAppPurchasesApi.md#inapppurchasesv2deleteinstance) | **DELETE** /v2/inAppPurchases/{id} |  |
| [**InAppPurchasesV2GetInstance**](InAppPurchasesApi.md#inapppurchasesv2getinstance) | **GET** /v2/inAppPurchases/{id} |  |
| [**InAppPurchasesV2IapPriceScheduleGetToOneRelated**](InAppPurchasesApi.md#inapppurchasesv2iappriceschedulegettoonerelated) | **GET** /v2/inAppPurchases/{id}/iapPriceSchedule |  |
| [**InAppPurchasesV2IapPriceScheduleGetToOneRelationship**](InAppPurchasesApi.md#inapppurchasesv2iappriceschedulegettoonerelationship) | **GET** /v2/inAppPurchases/{id}/relationships/iapPriceSchedule |  |
| [**InAppPurchasesV2ImagesGetToManyRelated**](InAppPurchasesApi.md#inapppurchasesv2imagesgettomanyrelated) | **GET** /v2/inAppPurchases/{id}/images |  |
| [**InAppPurchasesV2ImagesGetToManyRelationship**](InAppPurchasesApi.md#inapppurchasesv2imagesgettomanyrelationship) | **GET** /v2/inAppPurchases/{id}/relationships/images |  |
| [**InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelated**](InAppPurchasesApi.md#inapppurchasesv2inapppurchaseavailabilitygettoonerelated) | **GET** /v2/inAppPurchases/{id}/inAppPurchaseAvailability |  |
| [**InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelationship**](InAppPurchasesApi.md#inapppurchasesv2inapppurchaseavailabilitygettoonerelationship) | **GET** /v2/inAppPurchases/{id}/relationships/inAppPurchaseAvailability |  |
| [**InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelated**](InAppPurchasesApi.md#inapppurchasesv2inapppurchaselocalizationsgettomanyrelated) | **GET** /v2/inAppPurchases/{id}/inAppPurchaseLocalizations |  |
| [**InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelationship**](InAppPurchasesApi.md#inapppurchasesv2inapppurchaselocalizationsgettomanyrelationship) | **GET** /v2/inAppPurchases/{id}/relationships/inAppPurchaseLocalizations |  |
| [**InAppPurchasesV2OfferCodesGetToManyRelated**](InAppPurchasesApi.md#inapppurchasesv2offercodesgettomanyrelated) | **GET** /v2/inAppPurchases/{id}/offerCodes |  |
| [**InAppPurchasesV2OfferCodesGetToManyRelationship**](InAppPurchasesApi.md#inapppurchasesv2offercodesgettomanyrelationship) | **GET** /v2/inAppPurchases/{id}/relationships/offerCodes |  |
| [**InAppPurchasesV2PricePointsGetToManyRelated**](InAppPurchasesApi.md#inapppurchasesv2pricepointsgettomanyrelated) | **GET** /v2/inAppPurchases/{id}/pricePoints |  |
| [**InAppPurchasesV2PricePointsGetToManyRelationship**](InAppPurchasesApi.md#inapppurchasesv2pricepointsgettomanyrelationship) | **GET** /v2/inAppPurchases/{id}/relationships/pricePoints |  |
| [**InAppPurchasesV2PromotedPurchaseGetToOneRelated**](InAppPurchasesApi.md#inapppurchasesv2promotedpurchasegettoonerelated) | **GET** /v2/inAppPurchases/{id}/promotedPurchase |  |
| [**InAppPurchasesV2PromotedPurchaseGetToOneRelationship**](InAppPurchasesApi.md#inapppurchasesv2promotedpurchasegettoonerelationship) | **GET** /v2/inAppPurchases/{id}/relationships/promotedPurchase |  |
| [**InAppPurchasesV2UpdateInstance**](InAppPurchasesApi.md#inapppurchasesv2updateinstance) | **PATCH** /v2/inAppPurchases/{id} |  |

<a id="inapppurchasesgetinstance"></a>
# **InAppPurchasesGetInstance**
> InAppPurchaseResponse InAppPurchasesGetInstance (string id, List<string> fieldsInAppPurchases = null, List<string> include = null, int limitApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitApps** | **int** | maximum number of related apps returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseResponse**](InAppPurchaseResponse.md)

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
| **200** | Single InAppPurchase |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2appstorereviewscreenshotgettoonerelated"></a>
# **InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelated**
> InAppPurchaseAppStoreReviewScreenshotResponse InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelated (string id, List<string> fieldsInAppPurchaseAppStoreReviewScreenshots = null, List<string> fieldsInAppPurchases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseAppStoreReviewScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseAppStoreReviewScreenshotResponse**](InAppPurchaseAppStoreReviewScreenshotResponse.md)

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
| **200** | Single InAppPurchaseAppStoreReviewScreenshot |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2appstorereviewscreenshotgettoonerelationship"></a>
# **InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelationship**
> InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse InAppPurchasesV2AppStoreReviewScreenshotGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse**](InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse.md)

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

<a id="inapppurchasesv2contentgettoonerelated"></a>
# **InAppPurchasesV2ContentGetToOneRelated**
> InAppPurchaseContentResponse InAppPurchasesV2ContentGetToOneRelated (string id, List<string> fieldsInAppPurchaseContents = null, List<string> fieldsInAppPurchases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseContents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseContents | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseContentResponse**](InAppPurchaseContentResponse.md)

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
| **200** | Single InAppPurchaseContent |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2contentgettoonerelationship"></a>
# **InAppPurchasesV2ContentGetToOneRelationship**
> InAppPurchaseV2ContentLinkageResponse InAppPurchasesV2ContentGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchaseV2ContentLinkageResponse**](InAppPurchaseV2ContentLinkageResponse.md)

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

<a id="inapppurchasesv2createinstance"></a>
# **InAppPurchasesV2CreateInstance**
> InAppPurchaseV2Response InAppPurchasesV2CreateInstance (InAppPurchaseV2CreateRequest inAppPurchaseV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inAppPurchaseV2CreateRequest** | [**InAppPurchaseV2CreateRequest**](InAppPurchaseV2CreateRequest.md) | InAppPurchase representation |  |

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

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
| **201** | Single InAppPurchase |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2deleteinstance"></a>
# **InAppPurchasesV2DeleteInstance**
> void InAppPurchasesV2DeleteInstance (string id)




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

<a id="inapppurchasesv2getinstance"></a>
# **InAppPurchasesV2GetInstance**
> InAppPurchaseV2Response InAppPurchasesV2GetInstance (string id, List<string> fieldsInAppPurchases = null, List<string> fieldsInAppPurchaseLocalizations = null, List<string> fieldsInAppPurchasePricePoints = null, List<string> fieldsInAppPurchaseContents = null, List<string> fieldsInAppPurchaseAppStoreReviewScreenshots = null, List<string> fieldsPromotedPurchases = null, List<string> fieldsInAppPurchasePriceSchedules = null, List<string> fieldsInAppPurchaseAvailabilities = null, List<string> fieldsInAppPurchaseImages = null, List<string> fieldsInAppPurchaseOfferCodes = null, List<string> include = null, int limitImages = null, int limitInAppPurchaseLocalizations = null, int limitOfferCodes = null, int limitPricePoints = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **fieldsInAppPurchaseLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseLocalizations | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **fieldsInAppPurchaseContents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseContents | [optional]  |
| **fieldsInAppPurchaseAppStoreReviewScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsInAppPurchasePriceSchedules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional]  |
| **fieldsInAppPurchaseAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseAvailabilities | [optional]  |
| **fieldsInAppPurchaseImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseImages | [optional]  |
| **fieldsInAppPurchaseOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodes | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitImages** | **int** | maximum number of related images returned (when they are included) | [optional]  |
| **limitInAppPurchaseLocalizations** | **int** | maximum number of related inAppPurchaseLocalizations returned (when they are included) | [optional]  |
| **limitOfferCodes** | **int** | maximum number of related offerCodes returned (when they are included) | [optional]  |
| **limitPricePoints** | **int** | maximum number of related pricePoints returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

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
| **200** | Single InAppPurchase |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2iappriceschedulegettoonerelated"></a>
# **InAppPurchasesV2IapPriceScheduleGetToOneRelated**
> InAppPurchasePriceScheduleResponse InAppPurchasesV2IapPriceScheduleGetToOneRelated (string id, List<string> fieldsInAppPurchasePriceSchedules = null, List<string> fieldsTerritories = null, List<string> fieldsInAppPurchasePrices = null, List<string> include = null, int limitManualPrices = null, int limitAutomaticPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchasePriceSchedules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsInAppPurchasePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePrices | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitManualPrices** | **int** | maximum number of related manualPrices returned (when they are included) | [optional]  |
| **limitAutomaticPrices** | **int** | maximum number of related automaticPrices returned (when they are included) | [optional]  |

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

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
| **200** | Single InAppPurchasePriceSchedule |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2iappriceschedulegettoonerelationship"></a>
# **InAppPurchasesV2IapPriceScheduleGetToOneRelationship**
> InAppPurchaseV2IapPriceScheduleLinkageResponse InAppPurchasesV2IapPriceScheduleGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchaseV2IapPriceScheduleLinkageResponse**](InAppPurchaseV2IapPriceScheduleLinkageResponse.md)

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

<a id="inapppurchasesv2imagesgettomanyrelated"></a>
# **InAppPurchasesV2ImagesGetToManyRelated**
> InAppPurchaseImagesResponse InAppPurchasesV2ImagesGetToManyRelated (string id, List<string> fieldsInAppPurchaseImages = null, List<string> fieldsInAppPurchases = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseImages | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseImagesResponse**](InAppPurchaseImagesResponse.md)

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
| **200** | List of InAppPurchaseImages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2imagesgettomanyrelationship"></a>
# **InAppPurchasesV2ImagesGetToManyRelationship**
> InAppPurchaseV2ImagesLinkagesResponse InAppPurchasesV2ImagesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseV2ImagesLinkagesResponse**](InAppPurchaseV2ImagesLinkagesResponse.md)

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

<a id="inapppurchasesv2inapppurchaseavailabilitygettoonerelated"></a>
# **InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelated**
> InAppPurchaseAvailabilityResponse InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelated (string id, List<string> fieldsInAppPurchaseAvailabilities = null, List<string> fieldsTerritories = null, List<string> include = null, int limitAvailableTerritories = null)




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

<a id="inapppurchasesv2inapppurchaseavailabilitygettoonerelationship"></a>
# **InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelationship**
> InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse InAppPurchasesV2InAppPurchaseAvailabilityGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse**](InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse.md)

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

<a id="inapppurchasesv2inapppurchaselocalizationsgettomanyrelated"></a>
# **InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelated**
> InAppPurchaseLocalizationsResponse InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelated (string id, List<string> fieldsInAppPurchaseLocalizations = null, List<string> fieldsInAppPurchases = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsInAppPurchaseLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseLocalizations | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchaseLocalizationsResponse**](InAppPurchaseLocalizationsResponse.md)

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
| **200** | List of InAppPurchaseLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2inapppurchaselocalizationsgettomanyrelationship"></a>
# **InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelationship**
> InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse InAppPurchasesV2InAppPurchaseLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse**](InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse.md)

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

<a id="inapppurchasesv2offercodesgettomanyrelated"></a>
# **InAppPurchasesV2OfferCodesGetToManyRelated**
> InAppPurchaseOfferCodesResponse InAppPurchasesV2OfferCodesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsInAppPurchaseOfferCodes = null, List<string> fieldsInAppPurchaseOfferCodeOneTimeUseCodes = null, List<string> fieldsInAppPurchaseOfferCodeCustomCodes = null, List<string> fieldsInAppPurchaseOfferPrices = null, int limit = null, List<string> include = null, int limitOneTimeUseCodes = null, int limitCustomCodes = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by territory | [optional]  |
| **fieldsInAppPurchaseOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsInAppPurchaseOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferCodeCustomCodes | [optional]  |
| **fieldsInAppPurchaseOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchaseOfferPrices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitOneTimeUseCodes** | **int** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitCustomCodes** | **int** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**InAppPurchaseOfferCodesResponse**](InAppPurchaseOfferCodesResponse.md)

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
| **200** | List of InAppPurchaseOfferCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2offercodesgettomanyrelationship"></a>
# **InAppPurchasesV2OfferCodesGetToManyRelationship**
> InAppPurchaseV2OfferCodesLinkagesResponse InAppPurchasesV2OfferCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseV2OfferCodesLinkagesResponse**](InAppPurchaseV2OfferCodesLinkagesResponse.md)

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

<a id="inapppurchasesv2pricepointsgettomanyrelated"></a>
# **InAppPurchasesV2PricePointsGetToManyRelated**
> InAppPurchasePricePointsResponse InAppPurchasesV2PricePointsGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsInAppPurchasePricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsInAppPurchasePricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchasePricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**InAppPurchasePricePointsResponse**](InAppPurchasePricePointsResponse.md)

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
| **200** | List of InAppPurchasePricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2pricepointsgettomanyrelationship"></a>
# **InAppPurchasesV2PricePointsGetToManyRelationship**
> InAppPurchaseV2PricePointsLinkagesResponse InAppPurchasesV2PricePointsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**InAppPurchaseV2PricePointsLinkagesResponse**](InAppPurchaseV2PricePointsLinkagesResponse.md)

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

<a id="inapppurchasesv2promotedpurchasegettoonerelated"></a>
# **InAppPurchasesV2PromotedPurchaseGetToOneRelated**
> PromotedPurchaseResponse InAppPurchasesV2PromotedPurchaseGetToOneRelated (string id, List<string> fieldsPromotedPurchases = null, List<string> fieldsInAppPurchases = null, List<string> fieldsSubscriptions = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**PromotedPurchaseResponse**](PromotedPurchaseResponse.md)

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
| **200** | Single PromotedPurchase |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="inapppurchasesv2promotedpurchasegettoonerelationship"></a>
# **InAppPurchasesV2PromotedPurchaseGetToOneRelationship**
> InAppPurchaseV2PromotedPurchaseLinkageResponse InAppPurchasesV2PromotedPurchaseGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**InAppPurchaseV2PromotedPurchaseLinkageResponse**](InAppPurchaseV2PromotedPurchaseLinkageResponse.md)

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

<a id="inapppurchasesv2updateinstance"></a>
# **InAppPurchasesV2UpdateInstance**
> InAppPurchaseV2Response InAppPurchasesV2UpdateInstance (string id, InAppPurchaseV2UpdateRequest inAppPurchaseV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **inAppPurchaseV2UpdateRequest** | [**InAppPurchaseV2UpdateRequest**](InAppPurchaseV2UpdateRequest.md) | InAppPurchase representation |  |

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

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
| **200** | Single InAppPurchase |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

