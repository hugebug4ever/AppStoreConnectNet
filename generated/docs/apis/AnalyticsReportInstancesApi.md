# AppStoreConnect.Net.Api.AnalyticsReportInstancesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportInstancesGetInstance**](AnalyticsReportInstancesApi.md#analyticsreportinstancesgetinstance) | **GET** /v1/analyticsReportInstances/{id} |  |
| [**AnalyticsReportInstancesSegmentsGetToManyRelated**](AnalyticsReportInstancesApi.md#analyticsreportinstancessegmentsgettomanyrelated) | **GET** /v1/analyticsReportInstances/{id}/segments |  |
| [**AnalyticsReportInstancesSegmentsGetToManyRelationship**](AnalyticsReportInstancesApi.md#analyticsreportinstancessegmentsgettomanyrelationship) | **GET** /v1/analyticsReportInstances/{id}/relationships/segments |  |

<a id="analyticsreportinstancesgetinstance"></a>
# **AnalyticsReportInstancesGetInstance**
> AnalyticsReportInstanceResponse AnalyticsReportInstancesGetInstance (string id, List<string> fieldsAnalyticsReportInstances = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportInstances** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReportInstances | [optional]  |

### Return type

[**AnalyticsReportInstanceResponse**](AnalyticsReportInstanceResponse.md)

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
| **200** | Single AnalyticsReportInstance |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportinstancessegmentsgettomanyrelated"></a>
# **AnalyticsReportInstancesSegmentsGetToManyRelated**
> AnalyticsReportSegmentsResponse AnalyticsReportInstancesSegmentsGetToManyRelated (string id, List<string> fieldsAnalyticsReportSegments = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportSegments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReportSegments | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportSegmentsResponse**](AnalyticsReportSegmentsResponse.md)

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
| **200** | List of AnalyticsReportSegments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportinstancessegmentsgettomanyrelationship"></a>
# **AnalyticsReportInstancesSegmentsGetToManyRelationship**
> AnalyticsReportInstanceSegmentsLinkagesResponse AnalyticsReportInstancesSegmentsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportInstanceSegmentsLinkagesResponse**](AnalyticsReportInstanceSegmentsLinkagesResponse.md)

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

