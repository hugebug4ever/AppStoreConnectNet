# AppStoreConnect.Net.Api.WebhooksApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**WebhooksCreateInstance**](WebhooksApi.md#webhookscreateinstance) | **POST** /v1/webhooks |  |
| [**WebhooksDeleteInstance**](WebhooksApi.md#webhooksdeleteinstance) | **DELETE** /v1/webhooks/{id} |  |
| [**WebhooksDeliveriesGetToManyRelated**](WebhooksApi.md#webhooksdeliveriesgettomanyrelated) | **GET** /v1/webhooks/{id}/deliveries |  |
| [**WebhooksDeliveriesGetToManyRelationship**](WebhooksApi.md#webhooksdeliveriesgettomanyrelationship) | **GET** /v1/webhooks/{id}/relationships/deliveries |  |
| [**WebhooksGetInstance**](WebhooksApi.md#webhooksgetinstance) | **GET** /v1/webhooks/{id} |  |
| [**WebhooksUpdateInstance**](WebhooksApi.md#webhooksupdateinstance) | **PATCH** /v1/webhooks/{id} |  |

<a id="webhookscreateinstance"></a>
# **WebhooksCreateInstance**
> WebhookResponse WebhooksCreateInstance (WebhookCreateRequest webhookCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **webhookCreateRequest** | [**WebhookCreateRequest**](WebhookCreateRequest.md) | Webhook representation |  |

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
| **201** | Single Webhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="webhooksdeleteinstance"></a>
# **WebhooksDeleteInstance**
> void WebhooksDeleteInstance (string id)




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

<a id="webhooksdeliveriesgettomanyrelated"></a>
# **WebhooksDeliveriesGetToManyRelated**
> WebhookDeliveriesResponse WebhooksDeliveriesGetToManyRelated (string id, List<string> filterDeliveryState = null, List<string> filterCreatedDateGreaterThanOrEqualTo = null, List<string> filterCreatedDateLessThan = null, List<string> fieldsWebhookDeliveries = null, List<string> fieldsWebhookEvents = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterDeliveryState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;deliveryState&#39; | [optional]  |
| **filterCreatedDateGreaterThanOrEqualTo** | [**List&lt;string&gt;**](string.md) | filter by createdDateGreaterThanOrEqualTo | [optional]  |
| **filterCreatedDateLessThan** | [**List&lt;string&gt;**](string.md) | filter by createdDateLessThan | [optional]  |
| **fieldsWebhookDeliveries** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type webhookDeliveries | [optional]  |
| **fieldsWebhookEvents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type webhookEvents | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**WebhookDeliveriesResponse**](WebhookDeliveriesResponse.md)

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
| **200** | List of WebhookDeliveries |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="webhooksdeliveriesgettomanyrelationship"></a>
# **WebhooksDeliveriesGetToManyRelationship**
> WebhookDeliveriesLinkagesResponse WebhooksDeliveriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**WebhookDeliveriesLinkagesResponse**](WebhookDeliveriesLinkagesResponse.md)

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

<a id="webhooksgetinstance"></a>
# **WebhooksGetInstance**
> WebhookResponse WebhooksGetInstance (string id, List<string> fieldsWebhooks = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsWebhooks** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type webhooks | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
| **200** | Single Webhook |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="webhooksupdateinstance"></a>
# **WebhooksUpdateInstance**
> WebhookResponse WebhooksUpdateInstance (string id, WebhookUpdateRequest webhookUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **webhookUpdateRequest** | [**WebhookUpdateRequest**](WebhookUpdateRequest.md) | Webhook representation |  |

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
| **200** | Single Webhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

