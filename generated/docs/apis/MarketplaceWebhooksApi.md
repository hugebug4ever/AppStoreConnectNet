# AppStoreConnect.Net.Api.MarketplaceWebhooksApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MarketplaceWebhooksCreateInstance**](MarketplaceWebhooksApi.md#marketplacewebhookscreateinstance) | **POST** /v1/marketplaceWebhooks |  |
| [**MarketplaceWebhooksDeleteInstance**](MarketplaceWebhooksApi.md#marketplacewebhooksdeleteinstance) | **DELETE** /v1/marketplaceWebhooks/{id} |  |
| [**MarketplaceWebhooksGetCollection**](MarketplaceWebhooksApi.md#marketplacewebhooksgetcollection) | **GET** /v1/marketplaceWebhooks |  |
| [**MarketplaceWebhooksUpdateInstance**](MarketplaceWebhooksApi.md#marketplacewebhooksupdateinstance) | **PATCH** /v1/marketplaceWebhooks/{id} |  |

<a id="marketplacewebhookscreateinstance"></a>
# **MarketplaceWebhooksCreateInstance**
> MarketplaceWebhookResponse MarketplaceWebhooksCreateInstance (MarketplaceWebhookCreateRequest marketplaceWebhookCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **marketplaceWebhookCreateRequest** | [**MarketplaceWebhookCreateRequest**](MarketplaceWebhookCreateRequest.md) | MarketplaceWebhook representation |  |

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
| **201** | Single MarketplaceWebhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="marketplacewebhooksdeleteinstance"></a>
# **MarketplaceWebhooksDeleteInstance**
> void MarketplaceWebhooksDeleteInstance (string id)




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

<a id="marketplacewebhooksgetcollection"></a>
# **MarketplaceWebhooksGetCollection**
> MarketplaceWebhooksResponse MarketplaceWebhooksGetCollection (List<string> fieldsMarketplaceWebhooks = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsMarketplaceWebhooks** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type marketplaceWebhooks | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**MarketplaceWebhooksResponse**](MarketplaceWebhooksResponse.md)

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
| **200** | List of MarketplaceWebhooks |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="marketplacewebhooksupdateinstance"></a>
# **MarketplaceWebhooksUpdateInstance**
> MarketplaceWebhookResponse MarketplaceWebhooksUpdateInstance (string id, MarketplaceWebhookUpdateRequest marketplaceWebhookUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **marketplaceWebhookUpdateRequest** | [**MarketplaceWebhookUpdateRequest**](MarketplaceWebhookUpdateRequest.md) | MarketplaceWebhook representation |  |

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
| **200** | Single MarketplaceWebhook |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

