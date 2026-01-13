# AppStoreConnect.Net.Api.AppEventScreenshotsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEventScreenshotsCreateInstance**](AppEventScreenshotsApi.md#appeventscreenshotscreateinstance) | **POST** /v1/appEventScreenshots |  |
| [**AppEventScreenshotsDeleteInstance**](AppEventScreenshotsApi.md#appeventscreenshotsdeleteinstance) | **DELETE** /v1/appEventScreenshots/{id} |  |
| [**AppEventScreenshotsGetInstance**](AppEventScreenshotsApi.md#appeventscreenshotsgetinstance) | **GET** /v1/appEventScreenshots/{id} |  |
| [**AppEventScreenshotsUpdateInstance**](AppEventScreenshotsApi.md#appeventscreenshotsupdateinstance) | **PATCH** /v1/appEventScreenshots/{id} |  |

<a id="appeventscreenshotscreateinstance"></a>
# **AppEventScreenshotsCreateInstance**
> AppEventScreenshotResponse AppEventScreenshotsCreateInstance (AppEventScreenshotCreateRequest appEventScreenshotCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEventScreenshotCreateRequest** | [**AppEventScreenshotCreateRequest**](AppEventScreenshotCreateRequest.md) | AppEventScreenshot representation |  |

### Return type

[**AppEventScreenshotResponse**](AppEventScreenshotResponse.md)

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
| **201** | Single AppEventScreenshot |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventscreenshotsdeleteinstance"></a>
# **AppEventScreenshotsDeleteInstance**
> void AppEventScreenshotsDeleteInstance (string id)




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

<a id="appeventscreenshotsgetinstance"></a>
# **AppEventScreenshotsGetInstance**
> AppEventScreenshotResponse AppEventScreenshotsGetInstance (string id, List<string> fieldsAppEventScreenshots = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEventScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventScreenshots | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppEventScreenshotResponse**](AppEventScreenshotResponse.md)

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
| **200** | Single AppEventScreenshot |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventscreenshotsupdateinstance"></a>
# **AppEventScreenshotsUpdateInstance**
> AppEventScreenshotResponse AppEventScreenshotsUpdateInstance (string id, AppEventScreenshotUpdateRequest appEventScreenshotUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEventScreenshotUpdateRequest** | [**AppEventScreenshotUpdateRequest**](AppEventScreenshotUpdateRequest.md) | AppEventScreenshot representation |  |

### Return type

[**AppEventScreenshotResponse**](AppEventScreenshotResponse.md)

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
| **200** | Single AppEventScreenshot |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

