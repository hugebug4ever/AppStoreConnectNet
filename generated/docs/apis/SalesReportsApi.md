# AppStoreConnect.Net.Api.SalesReportsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SalesReportsGetCollection**](SalesReportsApi.md#salesreportsgetcollection) | **GET** /v1/salesReports |  |

<a id="salesreportsgetcollection"></a>
# **SalesReportsGetCollection**
> System.IO.Stream SalesReportsGetCollection (List<string> filterVendorNumber, List<string> filterReportType, List<string> filterReportSubType, List<string> filterFrequency, List<string> filterReportDate = null, List<string> filterVersion = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterVendorNumber** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;vendorNumber&#39; |  |
| **filterReportType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;reportType&#39; |  |
| **filterReportSubType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;reportSubType&#39; |  |
| **filterFrequency** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;frequency&#39; |  |
| **filterReportDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;reportDate&#39; | [optional]  |
| **filterVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;version&#39; | [optional]  |

### Return type

**System.IO.Stream**

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/a-gzip


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **200** | List of SalesReports |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

