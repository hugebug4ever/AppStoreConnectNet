# AppStoreConnect.Net.Api.CiTestResultsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiTestResultsGetInstance**](CiTestResultsApi.md#citestresultsgetinstance) | **GET** /v1/ciTestResults/{id} |  |

<a id="citestresultsgetinstance"></a>
# **CiTestResultsGetInstance**
> CiTestResultResponse CiTestResultsGetInstance (string id, List<string> fieldsCiTestResults = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiTestResults** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciTestResults | [optional]  |

### Return type

[**CiTestResultResponse**](CiTestResultResponse.md)

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
| **200** | Single CiTestResult |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

