# AppStoreConnect.Net.Api.SubscriptionGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionGroupsCreateInstance**](SubscriptionGroupsApi.md#subscriptiongroupscreateinstance) | **POST** /v1/subscriptionGroups |  |
| [**SubscriptionGroupsDeleteInstance**](SubscriptionGroupsApi.md#subscriptiongroupsdeleteinstance) | **DELETE** /v1/subscriptionGroups/{id} |  |
| [**SubscriptionGroupsGetInstance**](SubscriptionGroupsApi.md#subscriptiongroupsgetinstance) | **GET** /v1/subscriptionGroups/{id} |  |
| [**SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelated**](SubscriptionGroupsApi.md#subscriptiongroupssubscriptiongrouplocalizationsgettomanyrelated) | **GET** /v1/subscriptionGroups/{id}/subscriptionGroupLocalizations |  |
| [**SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelationship**](SubscriptionGroupsApi.md#subscriptiongroupssubscriptiongrouplocalizationsgettomanyrelationship) | **GET** /v1/subscriptionGroups/{id}/relationships/subscriptionGroupLocalizations |  |
| [**SubscriptionGroupsSubscriptionsGetToManyRelated**](SubscriptionGroupsApi.md#subscriptiongroupssubscriptionsgettomanyrelated) | **GET** /v1/subscriptionGroups/{id}/subscriptions |  |
| [**SubscriptionGroupsSubscriptionsGetToManyRelationship**](SubscriptionGroupsApi.md#subscriptiongroupssubscriptionsgettomanyrelationship) | **GET** /v1/subscriptionGroups/{id}/relationships/subscriptions |  |
| [**SubscriptionGroupsUpdateInstance**](SubscriptionGroupsApi.md#subscriptiongroupsupdateinstance) | **PATCH** /v1/subscriptionGroups/{id} |  |

<a id="subscriptiongroupscreateinstance"></a>
# **SubscriptionGroupsCreateInstance**
> SubscriptionGroupResponse SubscriptionGroupsCreateInstance (SubscriptionGroupCreateRequest subscriptionGroupCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionGroupCreateRequest** | [**SubscriptionGroupCreateRequest**](SubscriptionGroupCreateRequest.md) | SubscriptionGroup representation |  |

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

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
| **201** | Single SubscriptionGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptiongroupsdeleteinstance"></a>
# **SubscriptionGroupsDeleteInstance**
> void SubscriptionGroupsDeleteInstance (string id)




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

<a id="subscriptiongroupsgetinstance"></a>
# **SubscriptionGroupsGetInstance**
> SubscriptionGroupResponse SubscriptionGroupsGetInstance (string id, List<string> fieldsSubscriptionGroups = null, List<string> fieldsSubscriptions = null, List<string> fieldsSubscriptionGroupLocalizations = null, List<string> include = null, int limitSubscriptionGroupLocalizations = null, int limitSubscriptions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroups | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionGroupLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroupLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubscriptionGroupLocalizations** | **int** | maximum number of related subscriptionGroupLocalizations returned (when they are included) | [optional]  |
| **limitSubscriptions** | **int** | maximum number of related subscriptions returned (when they are included) | [optional]  |

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

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
| **200** | Single SubscriptionGroup |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptiongroupssubscriptiongrouplocalizationsgettomanyrelated"></a>
# **SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelated**
> SubscriptionGroupLocalizationsResponse SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelated (string id, List<string> fieldsSubscriptionGroupLocalizations = null, List<string> fieldsSubscriptionGroups = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionGroupLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroupLocalizations | [optional]  |
| **fieldsSubscriptionGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroups | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionGroupLocalizationsResponse**](SubscriptionGroupLocalizationsResponse.md)

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
| **200** | List of SubscriptionGroupLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptiongroupssubscriptiongrouplocalizationsgettomanyrelationship"></a>
# **SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelationship**
> SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse SubscriptionGroupsSubscriptionGroupLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse**](SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse.md)

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

<a id="subscriptiongroupssubscriptionsgettomanyrelated"></a>
# **SubscriptionGroupsSubscriptionsGetToManyRelated**
> SubscriptionsResponse SubscriptionGroupsSubscriptionsGetToManyRelated (string id, List<string> filterProductId = null, List<string> filterName = null, List<string> filterState = null, List<string> sort = null, List<string> fieldsSubscriptions = null, List<string> fieldsSubscriptionLocalizations = null, List<string> fieldsSubscriptionAppStoreReviewScreenshots = null, List<string> fieldsSubscriptionGroups = null, List<string> fieldsSubscriptionIntroductoryOffers = null, List<string> fieldsSubscriptionPromotionalOffers = null, List<string> fieldsSubscriptionOfferCodes = null, List<string> fieldsSubscriptionPrices = null, List<string> fieldsPromotedPurchases = null, List<string> fieldsSubscriptionAvailabilities = null, List<string> fieldsWinBackOffers = null, List<string> fieldsSubscriptionImages = null, int limit = null, List<string> include = null, int limitSubscriptionLocalizations = null, int limitIntroductoryOffers = null, int limitPromotionalOffers = null, int limitOfferCodes = null, int limitPrices = null, int limitWinBackOffers = null, int limitImages = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterProductId** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;productId&#39; | [optional]  |
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionLocalizations | [optional]  |
| **fieldsSubscriptionAppStoreReviewScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional]  |
| **fieldsSubscriptionGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGroups | [optional]  |
| **fieldsSubscriptionIntroductoryOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional]  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptionPrices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionPrices | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsSubscriptionAvailabilities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionAvailabilities | [optional]  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubscriptionLocalizations** | **int** | maximum number of related subscriptionLocalizations returned (when they are included) | [optional]  |
| **limitIntroductoryOffers** | **int** | maximum number of related introductoryOffers returned (when they are included) | [optional]  |
| **limitPromotionalOffers** | **int** | maximum number of related promotionalOffers returned (when they are included) | [optional]  |
| **limitOfferCodes** | **int** | maximum number of related offerCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int** | maximum number of related prices returned (when they are included) | [optional]  |
| **limitWinBackOffers** | **int** | maximum number of related winBackOffers returned (when they are included) | [optional]  |
| **limitImages** | **int** | maximum number of related images returned (when they are included) | [optional]  |

### Return type

[**SubscriptionsResponse**](SubscriptionsResponse.md)

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
| **200** | List of Subscriptions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptiongroupssubscriptionsgettomanyrelationship"></a>
# **SubscriptionGroupsSubscriptionsGetToManyRelationship**
> SubscriptionGroupSubscriptionsLinkagesResponse SubscriptionGroupsSubscriptionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SubscriptionGroupSubscriptionsLinkagesResponse**](SubscriptionGroupSubscriptionsLinkagesResponse.md)

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

<a id="subscriptiongroupsupdateinstance"></a>
# **SubscriptionGroupsUpdateInstance**
> SubscriptionGroupResponse SubscriptionGroupsUpdateInstance (string id, SubscriptionGroupUpdateRequest subscriptionGroupUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionGroupUpdateRequest** | [**SubscriptionGroupUpdateRequest**](SubscriptionGroupUpdateRequest.md) | SubscriptionGroup representation |  |

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

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
| **200** | Single SubscriptionGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

