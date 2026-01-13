# AppStoreConnect.Net.Api.SandboxTestersClearPurchaseHistoryRequestApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SandboxTestersClearPurchaseHistoryRequestV2CreateInstance**](SandboxTestersClearPurchaseHistoryRequestApi.md#sandboxtestersclearpurchasehistoryrequestv2createinstance) | **POST** /v2/sandboxTestersClearPurchaseHistoryRequest |  |

<a id="sandboxtestersclearpurchasehistoryrequestv2createinstance"></a>
# **SandboxTestersClearPurchaseHistoryRequestV2CreateInstance**
> SandboxTestersClearPurchaseHistoryRequestV2Response SandboxTestersClearPurchaseHistoryRequestV2CreateInstance (SandboxTestersClearPurchaseHistoryRequestV2CreateRequest sandboxTestersClearPurchaseHistoryRequestV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **sandboxTestersClearPurchaseHistoryRequestV2CreateRequest** | [**SandboxTestersClearPurchaseHistoryRequestV2CreateRequest**](SandboxTestersClearPurchaseHistoryRequestV2CreateRequest.md) | SandboxTestersClearPurchaseHistoryRequest representation |  |

### Return type

[**SandboxTestersClearPurchaseHistoryRequestV2Response**](SandboxTestersClearPurchaseHistoryRequestV2Response.md)

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
| **201** | Single SandboxTestersClearPurchaseHistoryRequest |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

