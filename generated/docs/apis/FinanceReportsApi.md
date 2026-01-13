# AppStoreConnect.Net.Api.FinanceReportsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**FinanceReportsGetCollection**](FinanceReportsApi.md#financereportsgetcollection) | **GET** /v1/financeReports |  |

<a id="financereportsgetcollection"></a>
# **FinanceReportsGetCollection**
> System.IO.Stream FinanceReportsGetCollection (List<string> filterVendorNumber, List<string> filterReportType, List<string> filterRegionCode, List<string> filterReportDate)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterVendorNumber** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;vendorNumber&#39; |  |
| **filterReportType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;reportType&#39; |  |
| **filterRegionCode** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;regionCode&#39; |  |
| **filterReportDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;reportDate&#39; |  |

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
| **200** | List of FinanceReports |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

