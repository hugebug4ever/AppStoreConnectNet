# AppStoreConnect.Net.Api.SubscriptionGracePeriodsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionGracePeriodsGetInstance**](SubscriptionGracePeriodsApi.md#subscriptiongraceperiodsgetinstance) | **GET** /v1/subscriptionGracePeriods/{id} |  |
| [**SubscriptionGracePeriodsUpdateInstance**](SubscriptionGracePeriodsApi.md#subscriptiongraceperiodsupdateinstance) | **PATCH** /v1/subscriptionGracePeriods/{id} |  |

<a id="subscriptiongraceperiodsgetinstance"></a>
# **SubscriptionGracePeriodsGetInstance**
> SubscriptionGracePeriodResponse SubscriptionGracePeriodsGetInstance (string id, List<string> fieldsSubscriptionGracePeriods = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionGracePeriods** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type subscriptionGracePeriods | [optional]  |

### Return type

[**SubscriptionGracePeriodResponse**](SubscriptionGracePeriodResponse.md)

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
| **200** | Single SubscriptionGracePeriod |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="subscriptiongraceperiodsupdateinstance"></a>
# **SubscriptionGracePeriodsUpdateInstance**
> SubscriptionGracePeriodResponse SubscriptionGracePeriodsUpdateInstance (string id, SubscriptionGracePeriodUpdateRequest subscriptionGracePeriodUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionGracePeriodUpdateRequest** | [**SubscriptionGracePeriodUpdateRequest**](SubscriptionGracePeriodUpdateRequest.md) | SubscriptionGracePeriod representation |  |

### Return type

[**SubscriptionGracePeriodResponse**](SubscriptionGracePeriodResponse.md)

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
| **200** | Single SubscriptionGracePeriod |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

