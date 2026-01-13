# AppStoreConnect.Net.Api.DiagnosticSignaturesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**DiagnosticSignaturesLogsGetToManyRelated**](DiagnosticSignaturesApi.md#diagnosticsignatureslogsgettomanyrelated) | **GET** /v1/diagnosticSignatures/{id}/logs |  |

<a id="diagnosticsignatureslogsgettomanyrelated"></a>
# **DiagnosticSignaturesLogsGetToManyRelated**
> DiagnosticLogs DiagnosticSignaturesLogsGetToManyRelated (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**DiagnosticLogs**](DiagnosticLogs.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/vnd.apple.diagnostic-logs+json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of DiagnosticLogs |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

