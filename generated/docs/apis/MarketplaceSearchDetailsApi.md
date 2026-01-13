# AppStoreConnect.Net.Api.MarketplaceSearchDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MarketplaceSearchDetailsCreateInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailscreateinstance) | **POST** /v1/marketplaceSearchDetails |  |
| [**MarketplaceSearchDetailsDeleteInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailsdeleteinstance) | **DELETE** /v1/marketplaceSearchDetails/{id} |  |
| [**MarketplaceSearchDetailsUpdateInstance**](MarketplaceSearchDetailsApi.md#marketplacesearchdetailsupdateinstance) | **PATCH** /v1/marketplaceSearchDetails/{id} |  |

<a id="marketplacesearchdetailscreateinstance"></a>
# **MarketplaceSearchDetailsCreateInstance**
> MarketplaceSearchDetailResponse MarketplaceSearchDetailsCreateInstance (MarketplaceSearchDetailCreateRequest marketplaceSearchDetailCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **marketplaceSearchDetailCreateRequest** | [**MarketplaceSearchDetailCreateRequest**](MarketplaceSearchDetailCreateRequest.md) | MarketplaceSearchDetail representation |  |

### Return type

[**MarketplaceSearchDetailResponse**](MarketplaceSearchDetailResponse.md)

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
| **201** | Single MarketplaceSearchDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="marketplacesearchdetailsdeleteinstance"></a>
# **MarketplaceSearchDetailsDeleteInstance**
> void MarketplaceSearchDetailsDeleteInstance (string id)




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

<a id="marketplacesearchdetailsupdateinstance"></a>
# **MarketplaceSearchDetailsUpdateInstance**
> MarketplaceSearchDetailResponse MarketplaceSearchDetailsUpdateInstance (string id, MarketplaceSearchDetailUpdateRequest marketplaceSearchDetailUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **marketplaceSearchDetailUpdateRequest** | [**MarketplaceSearchDetailUpdateRequest**](MarketplaceSearchDetailUpdateRequest.md) | MarketplaceSearchDetail representation |  |

### Return type

[**MarketplaceSearchDetailResponse**](MarketplaceSearchDetailResponse.md)

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
| **200** | Single MarketplaceSearchDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

