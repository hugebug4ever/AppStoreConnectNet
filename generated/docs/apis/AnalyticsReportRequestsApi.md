# AppStoreConnect.Net.Api.AnalyticsReportRequestsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AnalyticsReportRequestsCreateInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestscreateinstance) | **POST** /v1/analyticsReportRequests |  |
| [**AnalyticsReportRequestsDeleteInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestsdeleteinstance) | **DELETE** /v1/analyticsReportRequests/{id} |  |
| [**AnalyticsReportRequestsGetInstance**](AnalyticsReportRequestsApi.md#analyticsreportrequestsgetinstance) | **GET** /v1/analyticsReportRequests/{id} |  |
| [**AnalyticsReportRequestsReportsGetToManyRelated**](AnalyticsReportRequestsApi.md#analyticsreportrequestsreportsgettomanyrelated) | **GET** /v1/analyticsReportRequests/{id}/reports |  |
| [**AnalyticsReportRequestsReportsGetToManyRelationship**](AnalyticsReportRequestsApi.md#analyticsreportrequestsreportsgettomanyrelationship) | **GET** /v1/analyticsReportRequests/{id}/relationships/reports |  |

<a id="analyticsreportrequestscreateinstance"></a>
# **AnalyticsReportRequestsCreateInstance**
> AnalyticsReportRequestResponse AnalyticsReportRequestsCreateInstance (AnalyticsReportRequestCreateRequest analyticsReportRequestCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **analyticsReportRequestCreateRequest** | [**AnalyticsReportRequestCreateRequest**](AnalyticsReportRequestCreateRequest.md) | AnalyticsReportRequest representation |  |

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
| **201** | Single AnalyticsReportRequest |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportrequestsdeleteinstance"></a>
# **AnalyticsReportRequestsDeleteInstance**
> void AnalyticsReportRequestsDeleteInstance (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

void (empty response body)

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
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportrequestsgetinstance"></a>
# **AnalyticsReportRequestsGetInstance**
> AnalyticsReportRequestResponse AnalyticsReportRequestsGetInstance (string id, List<string> fieldsAnalyticsReportRequests = null, List<string> fieldsAnalyticsReports = null, List<string> include = null, int limitReports = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAnalyticsReportRequests** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReportRequests | [optional]  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitReports** | **int** | maximum number of related reports returned (when they are included) | [optional]  |

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
| **200** | Single AnalyticsReportRequest |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportrequestsreportsgettomanyrelated"></a>
# **AnalyticsReportRequestsReportsGetToManyRelated**
> AnalyticsReportsResponse AnalyticsReportRequestsReportsGetToManyRelated (string id, List<string> filterName = null, List<string> filterCategory = null, List<string> fieldsAnalyticsReports = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterCategory** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;category&#39; | [optional]  |
| **fieldsAnalyticsReports** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type analyticsReports | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportsResponse**](AnalyticsReportsResponse.md)

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
| **200** | List of AnalyticsReports |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="analyticsreportrequestsreportsgettomanyrelationship"></a>
# **AnalyticsReportRequestsReportsGetToManyRelationship**
> AnalyticsReportRequestReportsLinkagesResponse AnalyticsReportRequestsReportsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AnalyticsReportRequestReportsLinkagesResponse**](AnalyticsReportRequestReportsLinkagesResponse.md)

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

