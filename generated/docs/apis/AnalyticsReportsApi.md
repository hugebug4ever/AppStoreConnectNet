# AppStoreConnect.Net.Api.AnalyticsReportsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportsGetInstance**](AnalyticsReportsApi.md#analyticsreportsgetinstance) | **GET** /v1/analyticsReports/{id} |  |
| [**AnalyticsReportsInstancesGetToManyRelated**](AnalyticsReportsApi.md#analyticsreportsinstancesgettomanyrelated) | **GET** /v1/analyticsReports/{id}/instances |  |
| [**AnalyticsReportsInstancesGetToManyRelationship**](AnalyticsReportsApi.md#analyticsreportsinstancesgettomanyrelationship) | **GET** /v1/analyticsReports/{id}/relationships/instances |  |

<a id="analyticsreportsgetinstance"></a>
# **AnalyticsReportsGetInstance**
> AnalyticsReportResponse AnalyticsReportsGetInstance (string id, List<string> fieldsAnalyticsReports = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |

### Return type

[**AnalyticsReportResponse**](AnalyticsReportResponse.md)

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
| **200** | Single AnalyticsReport |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportsinstancesgettomanyrelated"></a>
# **AnalyticsReportsInstancesGetToManyRelated**
> AnalyticsReportInstancesResponse AnalyticsReportsInstancesGetToManyRelated (string id, List<string> filterGranularity = null, List<string> filterProcessingDate = null, List<string> fieldsAnalyticsReportInstances = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterGranularity** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;granularity&#39; | [optional]  |
| **filterProcessingDate** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;processingDate&#39; | [optional]  |
| **fieldsAnalyticsReportInstances** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReportInstances | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportInstancesResponse**](AnalyticsReportInstancesResponse.md)

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
| **200** | List of AnalyticsReportInstances |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportsinstancesgettomanyrelationship"></a>
# **AnalyticsReportsInstancesGetToManyRelationship**
> AnalyticsReportInstancesLinkagesResponse AnalyticsReportsInstancesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportInstancesLinkagesResponse**](AnalyticsReportInstancesLinkagesResponse.md)

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
| **200** | List of related linkages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

