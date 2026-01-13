# AppStoreConnect.Net.Api.SandboxTestersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SandboxTestersV2GetCollection**](SandboxTestersApi.md#sandboxtestersv2getcollection) | **GET** /v2/sandboxTesters |  |
| [**SandboxTestersV2UpdateInstance**](SandboxTestersApi.md#sandboxtestersv2updateinstance) | **PATCH** /v2/sandboxTesters/{id} |  |

<a id="sandboxtestersv2getcollection"></a>
# **SandboxTestersV2GetCollection**
> SandboxTestersV2Response SandboxTestersV2GetCollection (List<string> fieldsSandboxTesters = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsSandboxTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type sandboxTesters | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**SandboxTestersV2Response**](SandboxTestersV2Response.md)

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
| **200** | List of SandboxTesters |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="sandboxtestersv2updateinstance"></a>
# **SandboxTestersV2UpdateInstance**
> SandboxTesterV2Response SandboxTestersV2UpdateInstance (string id, SandboxTesterV2UpdateRequest sandboxTesterV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **sandboxTesterV2UpdateRequest** | [**SandboxTesterV2UpdateRequest**](SandboxTesterV2UpdateRequest.md) | SandboxTester representation |  |

### Return type

[**SandboxTesterV2Response**](SandboxTesterV2Response.md)

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
| **200** | Single SandboxTester |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

