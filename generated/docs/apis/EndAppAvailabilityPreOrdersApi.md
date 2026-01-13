# AppStoreConnect.Net.Api.EndAppAvailabilityPreOrdersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**EndAppAvailabilityPreOrdersCreateInstance**](EndAppAvailabilityPreOrdersApi.md#endappavailabilitypreorderscreateinstance) | **POST** /v1/endAppAvailabilityPreOrders |  |

<a id="endappavailabilitypreorderscreateinstance"></a>
# **EndAppAvailabilityPreOrdersCreateInstance**
> EndAppAvailabilityPreOrderResponse EndAppAvailabilityPreOrdersCreateInstance (EndAppAvailabilityPreOrderCreateRequest endAppAvailabilityPreOrderCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **endAppAvailabilityPreOrderCreateRequest** | [**EndAppAvailabilityPreOrderCreateRequest**](EndAppAvailabilityPreOrderCreateRequest.md) | EndAppAvailabilityPreOrder representation |  |

### Return type

[**EndAppAvailabilityPreOrderResponse**](EndAppAvailabilityPreOrderResponse.md)

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
| **201** | Single EndAppAvailabilityPreOrder |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

