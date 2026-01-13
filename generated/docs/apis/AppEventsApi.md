# AppStoreConnect.Net.Api.AppEventsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEventsCreateInstance**](AppEventsApi.md#appeventscreateinstance) | **POST** /v1/appEvents |  |
| [**AppEventsDeleteInstance**](AppEventsApi.md#appeventsdeleteinstance) | **DELETE** /v1/appEvents/{id} |  |
| [**AppEventsGetInstance**](AppEventsApi.md#appeventsgetinstance) | **GET** /v1/appEvents/{id} |  |
| [**AppEventsLocalizationsGetToManyRelated**](AppEventsApi.md#appeventslocalizationsgettomanyrelated) | **GET** /v1/appEvents/{id}/localizations |  |
| [**AppEventsLocalizationsGetToManyRelationship**](AppEventsApi.md#appeventslocalizationsgettomanyrelationship) | **GET** /v1/appEvents/{id}/relationships/localizations |  |
| [**AppEventsUpdateInstance**](AppEventsApi.md#appeventsupdateinstance) | **PATCH** /v1/appEvents/{id} |  |

<a id="appeventscreateinstance"></a>
# **AppEventsCreateInstance**
> AppEventResponse AppEventsCreateInstance (AppEventCreateRequest appEventCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEventCreateRequest** | [**AppEventCreateRequest**](AppEventCreateRequest.md) | AppEvent representation |  |

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
| **201** | Single AppEvent |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventsdeleteinstance"></a>
# **AppEventsDeleteInstance**
> void AppEventsDeleteInstance (string id)




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

<a id="appeventsgetinstance"></a>
# **AppEventsGetInstance**
> AppEventResponse AppEventsGetInstance (string id, List<string> fieldsAppEvents = null, List<string> fieldsAppEventLocalizations = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEvents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEvents | [optional]  |
| **fieldsAppEventLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
| **200** | Single AppEvent |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventslocalizationsgettomanyrelated"></a>
# **AppEventsLocalizationsGetToManyRelated**
> AppEventLocalizationsResponse AppEventsLocalizationsGetToManyRelated (string id, List<string> fieldsAppEventLocalizations = null, List<string> fieldsAppEvents = null, List<string> fieldsAppEventScreenshots = null, List<string> fieldsAppEventVideoClips = null, int limit = null, List<string> include = null, int limitAppEventScreenshots = null, int limitAppEventVideoClips = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEventLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventLocalizations | [optional]  |
| **fieldsAppEvents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEvents | [optional]  |
| **fieldsAppEventScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventScreenshots | [optional]  |
| **fieldsAppEventVideoClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventVideoClips | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppEventScreenshots** | **int** | maximum number of related appEventScreenshots returned (when they are included) | [optional]  |
| **limitAppEventVideoClips** | **int** | maximum number of related appEventVideoClips returned (when they are included) | [optional]  |

### Return type

[**AppEventLocalizationsResponse**](AppEventLocalizationsResponse.md)

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
| **200** | List of AppEventLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventslocalizationsgettomanyrelationship"></a>
# **AppEventsLocalizationsGetToManyRelationship**
> AppEventLocalizationsLinkagesResponse AppEventsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppEventLocalizationsLinkagesResponse**](AppEventLocalizationsLinkagesResponse.md)

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

<a id="appeventsupdateinstance"></a>
# **AppEventsUpdateInstance**
> AppEventResponse AppEventsUpdateInstance (string id, AppEventUpdateRequest appEventUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEventUpdateRequest** | [**AppEventUpdateRequest**](AppEventUpdateRequest.md) | AppEvent representation |  |

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
| **200** | Single AppEvent |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

