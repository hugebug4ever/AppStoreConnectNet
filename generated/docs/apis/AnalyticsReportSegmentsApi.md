# AppStoreConnect.Net.Api.AnalyticsReportSegmentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportSegmentsGetInstance**](AnalyticsReportSegmentsApi.md#analyticsreportsegmentsgetinstance) | **GET** /v1/analyticsReportSegments/{id} |  |

<a id="analyticsreportsegmentsgetinstance"></a>
# **AnalyticsReportSegmentsGetInstance**
> AnalyticsReportSegmentResponse AnalyticsReportSegmentsGetInstance (string id, List<string> fieldsAnalyticsReportSegments = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportSegments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReportSegments | [optional]  |

### Return type

[**AnalyticsReportSegmentResponse**](AnalyticsReportSegmentResponse.md)

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
| **200** | Single AnalyticsReportSegment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

