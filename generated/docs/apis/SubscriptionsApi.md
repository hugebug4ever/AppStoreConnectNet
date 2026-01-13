# AppStoreConnect.Net.Api.SubscriptionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionsAppStoreReviewScreenshotGetToOneRelated**](SubscriptionsApi.md#subscriptionsappstorereviewscreenshotgettoonerelated) | **GET** /v1/subscriptions/{id}/appStoreReviewScreenshot |  |
| [**SubscriptionsAppStoreReviewScreenshotGetToOneRelationship**](SubscriptionsApi.md#subscriptionsappstorereviewscreenshotgettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/appStoreReviewScreenshot |  |
| [**SubscriptionsCreateInstance**](SubscriptionsApi.md#subscriptionscreateinstance) | **POST** /v1/subscriptions |  |
| [**SubscriptionsDeleteInstance**](SubscriptionsApi.md#subscriptionsdeleteinstance) | **DELETE** /v1/subscriptions/{id} |  |
| [**SubscriptionsGetInstance**](SubscriptionsApi.md#subscriptionsgetinstance) | **GET** /v1/subscriptions/{id} |  |
| [**SubscriptionsImagesGetToManyRelated**](SubscriptionsApi.md#subscriptionsimagesgettomanyrelated) | **GET** /v1/subscriptions/{id}/images |  |
| [**SubscriptionsImagesGetToManyRelationship**](SubscriptionsApi.md#subscriptionsimagesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/images |  |
| [**SubscriptionsIntroductoryOffersDeleteToManyRelationship**](SubscriptionsApi.md#subscriptionsintroductoryoffersdeletetomanyrelationship) | **DELETE** /v1/subscriptions/{id}/relationships/introductoryOffers |  |
| [**SubscriptionsIntroductoryOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionsintroductoryoffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/introductoryOffers |  |
| [**SubscriptionsIntroductoryOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionsintroductoryoffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/introductoryOffers |  |
| [**SubscriptionsOfferCodesGetToManyRelated**](SubscriptionsApi.md#subscriptionsoffercodesgettomanyrelated) | **GET** /v1/subscriptions/{id}/offerCodes |  |
| [**SubscriptionsOfferCodesGetToManyRelationship**](SubscriptionsApi.md#subscriptionsoffercodesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/offerCodes |  |
| [**SubscriptionsPricePointsGetToManyRelated**](SubscriptionsApi.md#subscriptionspricepointsgettomanyrelated) | **GET** /v1/subscriptions/{id}/pricePoints |  |
| [**SubscriptionsPricePointsGetToManyRelationship**](SubscriptionsApi.md#subscriptionspricepointsgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/pricePoints |  |
| [**SubscriptionsPricesDeleteToManyRelationship**](SubscriptionsApi.md#subscriptionspricesdeletetomanyrelationship) | **DELETE** /v1/subscriptions/{id}/relationships/prices |  |
| [**SubscriptionsPricesGetToManyRelated**](SubscriptionsApi.md#subscriptionspricesgettomanyrelated) | **GET** /v1/subscriptions/{id}/prices |  |
| [**SubscriptionsPricesGetToManyRelationship**](SubscriptionsApi.md#subscriptionspricesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/prices |  |
| [**SubscriptionsPromotedPurchaseGetToOneRelated**](SubscriptionsApi.md#subscriptionspromotedpurchasegettoonerelated) | **GET** /v1/subscriptions/{id}/promotedPurchase |  |
| [**SubscriptionsPromotedPurchaseGetToOneRelationship**](SubscriptionsApi.md#subscriptionspromotedpurchasegettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/promotedPurchase |  |
| [**SubscriptionsPromotionalOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionspromotionaloffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/promotionalOffers |  |
| [**SubscriptionsPromotionalOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionspromotionaloffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/promotionalOffers |  |
| [**SubscriptionsSubscriptionAvailabilityGetToOneRelated**](SubscriptionsApi.md#subscriptionssubscriptionavailabilitygettoonerelated) | **GET** /v1/subscriptions/{id}/subscriptionAvailability |  |
| [**SubscriptionsSubscriptionAvailabilityGetToOneRelationship**](SubscriptionsApi.md#subscriptionssubscriptionavailabilitygettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionAvailability |  |
| [**SubscriptionsSubscriptionLocalizationsGetToManyRelated**](SubscriptionsApi.md#subscriptionssubscriptionlocalizationsgettomanyrelated) | **GET** /v1/subscriptions/{id}/subscriptionLocalizations |  |
| [**SubscriptionsSubscriptionLocalizationsGetToManyRelationship**](SubscriptionsApi.md#subscriptionssubscriptionlocalizationsgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionLocalizations |  |
| [**SubscriptionsUpdateInstance**](SubscriptionsApi.md#subscriptionsupdateinstance) | **PATCH** /v1/subscriptions/{id} |  |
| [**SubscriptionsWinBackOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionswinbackoffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/winBackOffers |  |
| [**SubscriptionsWinBackOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionswinbackoffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/winBackOffers |  |

<a id="subscriptionsappstorereviewscreenshotgettoonerelated"></a>
# **SubscriptionsAppStoreReviewScreenshotGetToOneRelated**
> SubscriptionAppStoreReviewScreenshotResponse SubscriptionsAppStoreReviewScreenshotGetToOneRelated (string id, List<string> fieldsSubscriptionAppStoreReviewScreenshots = null, List<string> fieldsSubscriptions = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionAppStoreReviewScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionAppStoreReviewScreenshotResponse**](SubscriptionAppStoreReviewScreenshotResponse.md)

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
| **200** | Single SubscriptionAppStoreReviewScreenshot |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsappstorereviewscreenshotgettoonerelationship"></a>
# **SubscriptionsAppStoreReviewScreenshotGetToOneRelationship**
> SubscriptionAppStoreReviewScreenshotLinkageResponse SubscriptionsAppStoreReviewScreenshotGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionAppStoreReviewScreenshotLinkageResponse**](SubscriptionAppStoreReviewScreenshotLinkageResponse.md)

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

<a id="subscriptionscreateinstance"></a>
# **SubscriptionsCreateInstance**
> SubscriptionResponse SubscriptionsCreateInstance (SubscriptionCreateRequest subscriptionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionCreateRequest** | [**SubscriptionCreateRequest**](SubscriptionCreateRequest.md) | Subscription representation |  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **201** | Single Subscription |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsdeleteinstance"></a>
# **SubscriptionsDeleteInstance**
> void SubscriptionsDeleteInstance (string id)




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

<a id="subscriptionsgetinstance"></a>
# **SubscriptionsGetInstance**
> SubscriptionResponse SubscriptionsGetInstance (string id, List<string> fieldsSubscriptions = null, List<string> fieldsSubscriptionLocalizations = null, List<string> fieldsSubscriptionAppStoreReviewScreenshots = null, List<string> fieldsSubscriptionIntroductoryOffers = null, List<string> fieldsSubscriptionPromotionalOffers = null, List<string> fieldsSubscriptionOfferCodes = null, List<string> fieldsSubscriptionPrices = null, List<string> fieldsPromotedPurchases = null, List<string> fieldsSubscriptionAvailabilities = null, List<string> fieldsWinBackOffers = null, List<string> fieldsSubscriptionImages = null, List<string> include = null, int limitImages = null, int limitIntroductoryOffers = null, int limitOfferCodes = null, int limitPrices = null, int limitPromotionalOffers = null, int limitSubscriptionLocalizations = null, int limitWinBackOffers = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionLocalizations | [optional]  |
| **fieldsSubscriptionAppStoreReviewScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional]  |
| **fieldsSubscriptionIntroductoryOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional]  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptionPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPrices | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsSubscriptionAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAvailabilities | [optional]  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitImages** | **int** | maximum number of related images returned (when they are included) | [optional]  |
| **limitIntroductoryOffers** | **int** | maximum number of related introductoryOffers returned (when they are included) | [optional]  |
| **limitOfferCodes** | **int** | maximum number of related offerCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |
| **limitPromotionalOffers** | **int** | maximum number of related promotionalOffers returned (when they are included) | [optional]  |
| **limitSubscriptionLocalizations** | **int** | maximum number of related subscriptionLocalizations returned (when they are included) | [optional]  |
| **limitWinBackOffers** | **int** | maximum number of related winBackOffers returned (when they are included) | [optional]  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **200** | Single Subscription |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsimagesgettomanyrelated"></a>
# **SubscriptionsImagesGetToManyRelated**
> SubscriptionImagesResponse SubscriptionsImagesGetToManyRelated (string id, List<string> fieldsSubscriptionImages = null, List<string> fieldsSubscriptions = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionImagesResponse**](SubscriptionImagesResponse.md)

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
| **200** | List of SubscriptionImages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsimagesgettomanyrelationship"></a>
# **SubscriptionsImagesGetToManyRelationship**
> SubscriptionImagesLinkagesResponse SubscriptionsImagesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionImagesLinkagesResponse**](SubscriptionImagesLinkagesResponse.md)

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

<a id="subscriptionsintroductoryoffersdeletetomanyrelationship"></a>
# **SubscriptionsIntroductoryOffersDeleteToManyRelationship**
> void SubscriptionsIntroductoryOffersDeleteToManyRelationship (string id, SubscriptionIntroductoryOffersLinkagesRequest subscriptionIntroductoryOffersLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionIntroductoryOffersLinkagesRequest** | [**SubscriptionIntroductoryOffersLinkagesRequest**](SubscriptionIntroductoryOffersLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsintroductoryoffersgettomanyrelated"></a>
# **SubscriptionsIntroductoryOffersGetToManyRelated**
> SubscriptionIntroductoryOffersResponse SubscriptionsIntroductoryOffersGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionIntroductoryOffers = null, List<string> fieldsSubscriptions = null, List<string> fieldsTerritories = null, List<string> fieldsSubscriptionPricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionIntroductoryOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionIntroductoryOffersResponse**](SubscriptionIntroductoryOffersResponse.md)

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
| **200** | List of SubscriptionIntroductoryOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsintroductoryoffersgettomanyrelationship"></a>
# **SubscriptionsIntroductoryOffersGetToManyRelationship**
> SubscriptionIntroductoryOffersLinkagesResponse SubscriptionsIntroductoryOffersGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionIntroductoryOffersLinkagesResponse**](SubscriptionIntroductoryOffersLinkagesResponse.md)

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

<a id="subscriptionsoffercodesgettomanyrelated"></a>
# **SubscriptionsOfferCodesGetToManyRelated**
> SubscriptionOfferCodesResponse SubscriptionsOfferCodesGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionOfferCodes = null, List<string> fieldsSubscriptions = null, List<string> fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string> fieldsSubscriptionOfferCodeCustomCodes = null, List<string> fieldsSubscriptionOfferCodePrices = null, int limit = null, List<string> include = null, int limitOneTimeUseCodes = null, int limitCustomCodes = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by territory | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitOneTimeUseCodes** | **int** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitCustomCodes** | **int** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionOfferCodesResponse**](SubscriptionOfferCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionsoffercodesgettomanyrelationship"></a>
# **SubscriptionsOfferCodesGetToManyRelationship**
> SubscriptionOfferCodesLinkagesResponse SubscriptionsOfferCodesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionOfferCodesLinkagesResponse**](SubscriptionOfferCodesLinkagesResponse.md)

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

<a id="subscriptionspricepointsgettomanyrelated"></a>
# **SubscriptionsPricePointsGetToManyRelated**
> SubscriptionPricePointsResponse SubscriptionsPricePointsGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionPricePoints = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricePointsResponse**](SubscriptionPricePointsResponse.md)

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
| **200** | List of SubscriptionPricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionspricepointsgettomanyrelationship"></a>
# **SubscriptionsPricePointsGetToManyRelationship**
> SubscriptionPricePointsLinkagesResponse SubscriptionsPricePointsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionPricePointsLinkagesResponse**](SubscriptionPricePointsLinkagesResponse.md)

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

<a id="subscriptionspricesdeletetomanyrelationship"></a>
# **SubscriptionsPricesDeleteToManyRelationship**
> void SubscriptionsPricesDeleteToManyRelationship (string id, SubscriptionPricesLinkagesRequest subscriptionPricesLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionPricesLinkagesRequest** | [**SubscriptionPricesLinkagesRequest**](SubscriptionPricesLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionspricesgettomanyrelated"></a>
# **SubscriptionsPricesGetToManyRelated**
> SubscriptionPricesResponse SubscriptionsPricesGetToManyRelated (string id, List<string> filterSubscriptionPricePoint = null, List<string> filterTerritory = null, List<string> fieldsSubscriptionPrices = null, List<string> fieldsTerritories = null, List<string> fieldsSubscriptionPricePoints = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterSubscriptionPricePoint** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;subscriptionPricePoint&#39; | [optional]  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricesResponse**](SubscriptionPricesResponse.md)

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
| **200** | List of SubscriptionPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionspricesgettomanyrelationship"></a>
# **SubscriptionsPricesGetToManyRelationship**
> SubscriptionPricesLinkagesResponse SubscriptionsPricesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionPricesLinkagesResponse**](SubscriptionPricesLinkagesResponse.md)

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

<a id="subscriptionspromotedpurchasegettoonerelated"></a>
# **SubscriptionsPromotedPurchaseGetToOneRelated**
> PromotedPurchaseResponse SubscriptionsPromotedPurchaseGetToOneRelated (string id, List<string> fieldsPromotedPurchases = null, List<string> fieldsInAppPurchases = null, List<string> fieldsSubscriptions = null, List<string> include = null)




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

<a id="subscriptionspromotedpurchasegettoonerelationship"></a>
# **SubscriptionsPromotedPurchaseGetToOneRelationship**
> SubscriptionPromotedPurchaseLinkageResponse SubscriptionsPromotedPurchaseGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionPromotedPurchaseLinkageResponse**](SubscriptionPromotedPurchaseLinkageResponse.md)

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

<a id="subscriptionspromotionaloffersgettomanyrelated"></a>
# **SubscriptionsPromotionalOffersGetToManyRelated**
> SubscriptionPromotionalOffersResponse SubscriptionsPromotionalOffersGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsSubscriptionPromotionalOffers = null, List<string> fieldsSubscriptions = null, List<string> fieldsSubscriptionPromotionalOfferPrices = null, int limit = null, List<string> include = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by territory | [optional]  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionPromotionalOffersResponse**](SubscriptionPromotionalOffersResponse.md)

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
| **200** | List of SubscriptionPromotionalOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionspromotionaloffersgettomanyrelationship"></a>
# **SubscriptionsPromotionalOffersGetToManyRelationship**
> SubscriptionPromotionalOffersLinkagesResponse SubscriptionsPromotionalOffersGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionPromotionalOffersLinkagesResponse**](SubscriptionPromotionalOffersLinkagesResponse.md)

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

<a id="subscriptionssubscriptionavailabilitygettoonerelated"></a>
# **SubscriptionsSubscriptionAvailabilityGetToOneRelated**
> SubscriptionAvailabilityResponse SubscriptionsSubscriptionAvailabilityGetToOneRelated (string id, List<string> fieldsSubscriptionAvailabilities = null, List<string> fieldsTerritories = null, List<string> include = null, int limitAvailableTerritories = null)




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

<a id="subscriptionssubscriptionavailabilitygettoonerelationship"></a>
# **SubscriptionsSubscriptionAvailabilityGetToOneRelationship**
> SubscriptionSubscriptionAvailabilityLinkageResponse SubscriptionsSubscriptionAvailabilityGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionSubscriptionAvailabilityLinkageResponse**](SubscriptionSubscriptionAvailabilityLinkageResponse.md)

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

<a id="subscriptionssubscriptionlocalizationsgettomanyrelated"></a>
# **SubscriptionsSubscriptionLocalizationsGetToManyRelated**
> SubscriptionLocalizationsResponse SubscriptionsSubscriptionLocalizationsGetToManyRelated (string id, List<string> fieldsSubscriptionLocalizations = null, List<string> fieldsSubscriptions = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionLocalizations | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionLocalizationsResponse**](SubscriptionLocalizationsResponse.md)

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
| **200** | List of SubscriptionLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionssubscriptionlocalizationsgettomanyrelationship"></a>
# **SubscriptionsSubscriptionLocalizationsGetToManyRelationship**
> SubscriptionSubscriptionLocalizationsLinkagesResponse SubscriptionsSubscriptionLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionSubscriptionLocalizationsLinkagesResponse**](SubscriptionSubscriptionLocalizationsLinkagesResponse.md)

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

<a id="subscriptionsupdateinstance"></a>
# **SubscriptionsUpdateInstance**
> SubscriptionResponse SubscriptionsUpdateInstance (string id, SubscriptionUpdateRequest subscriptionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionUpdateRequest** | [**SubscriptionUpdateRequest**](SubscriptionUpdateRequest.md) | Subscription representation |  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **200** | Single Subscription |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionswinbackoffersgettomanyrelated"></a>
# **SubscriptionsWinBackOffersGetToManyRelated**
> WinBackOffersResponse SubscriptionsWinBackOffersGetToManyRelated (string id, List<string> fieldsWinBackOffers = null, List<string> fieldsWinBackOfferPrices = null, int limit = null, List<string> include = null, int limitPrices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**WinBackOffersResponse**](WinBackOffersResponse.md)

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
| **200** | List of WinBackOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptionswinbackoffersgettomanyrelationship"></a>
# **SubscriptionsWinBackOffersGetToManyRelationship**
> SubscriptionWinBackOffersLinkagesResponse SubscriptionsWinBackOffersGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionWinBackOffersLinkagesResponse**](SubscriptionWinBackOffersLinkagesResponse.md)

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

