# AppStoreConnect.Net.Api.AppStoreVersionPromotionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionPromotionsCreateInstance**](AppStoreVersionPromotionsApi.md#appstoreversionpromotionscreateinstance) | **POST** /v1/appStoreVersionPromotions |  |

<a id="appstoreversionpromotionscreateinstance"></a>
# **AppStoreVersionPromotionsCreateInstance**
> AppStoreVersionPromotionResponse AppStoreVersionPromotionsCreateInstance (AppStoreVersionPromotionCreateRequest appStoreVersionPromotionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionPromotionCreateRequest** | [**AppStoreVersionPromotionCreateRequest**](AppStoreVersionPromotionCreateRequest.md) | AppStoreVersionPromotion representation |  |

### Return type

[**AppStoreVersionPromotionResponse**](AppStoreVersionPromotionResponse.md)

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
| **201** | Single AppStoreVersionPromotion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

