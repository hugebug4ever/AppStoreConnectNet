# AppStoreConnect.Net.Api.AppScreenshotSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppScreenshotSetsAppScreenshotsGetToManyRelated**](AppScreenshotSetsApi.md#appscreenshotsetsappscreenshotsgettomanyrelated) | **GET** /v1/appScreenshotSets/{id}/appScreenshots |  |
| [**AppScreenshotSetsAppScreenshotsGetToManyRelationship**](AppScreenshotSetsApi.md#appscreenshotsetsappscreenshotsgettomanyrelationship) | **GET** /v1/appScreenshotSets/{id}/relationships/appScreenshots |  |
| [**AppScreenshotSetsAppScreenshotsReplaceToManyRelationship**](AppScreenshotSetsApi.md#appscreenshotsetsappscreenshotsreplacetomanyrelationship) | **PATCH** /v1/appScreenshotSets/{id}/relationships/appScreenshots |  |
| [**AppScreenshotSetsCreateInstance**](AppScreenshotSetsApi.md#appscreenshotsetscreateinstance) | **POST** /v1/appScreenshotSets |  |
| [**AppScreenshotSetsDeleteInstance**](AppScreenshotSetsApi.md#appscreenshotsetsdeleteinstance) | **DELETE** /v1/appScreenshotSets/{id} |  |
| [**AppScreenshotSetsGetInstance**](AppScreenshotSetsApi.md#appscreenshotsetsgetinstance) | **GET** /v1/appScreenshotSets/{id} |  |

<a id="appscreenshotsetsappscreenshotsgettomanyrelated"></a>
# **AppScreenshotSetsAppScreenshotsGetToManyRelated**
> AppScreenshotsResponse AppScreenshotSetsAppScreenshotsGetToManyRelated (string id, List<string> fieldsAppScreenshots = null, List<string> fieldsAppScreenshotSets = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshots | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppScreenshotsResponse**](AppScreenshotsResponse.md)

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
| **200** | List of AppScreenshots |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appscreenshotsetsappscreenshotsgettomanyrelationship"></a>
# **AppScreenshotSetsAppScreenshotsGetToManyRelationship**
> AppScreenshotSetAppScreenshotsLinkagesResponse AppScreenshotSetsAppScreenshotsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppScreenshotSetAppScreenshotsLinkagesResponse**](AppScreenshotSetAppScreenshotsLinkagesResponse.md)

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

<a id="appscreenshotsetsappscreenshotsreplacetomanyrelationship"></a>
# **AppScreenshotSetsAppScreenshotsReplaceToManyRelationship**
> void AppScreenshotSetsAppScreenshotsReplaceToManyRelationship (string id, AppScreenshotSetAppScreenshotsLinkagesRequest appScreenshotSetAppScreenshotsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appScreenshotSetAppScreenshotsLinkagesRequest** | [**AppScreenshotSetAppScreenshotsLinkagesRequest**](AppScreenshotSetAppScreenshotsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appscreenshotsetscreateinstance"></a>
# **AppScreenshotSetsCreateInstance**
> AppScreenshotSetResponse AppScreenshotSetsCreateInstance (AppScreenshotSetCreateRequest appScreenshotSetCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appScreenshotSetCreateRequest** | [**AppScreenshotSetCreateRequest**](AppScreenshotSetCreateRequest.md) | AppScreenshotSet representation |  |

### Return type

[**AppScreenshotSetResponse**](AppScreenshotSetResponse.md)

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
| **201** | Single AppScreenshotSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appscreenshotsetsdeleteinstance"></a>
# **AppScreenshotSetsDeleteInstance**
> void AppScreenshotSetsDeleteInstance (string id)




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

<a id="appscreenshotsetsgetinstance"></a>
# **AppScreenshotSetsGetInstance**
> AppScreenshotSetResponse AppScreenshotSetsGetInstance (string id, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppScreenshots = null, List<string> include = null, int limitAppScreenshots = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshots | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppScreenshots** | **int** | maximum number of related appScreenshots returned (when they are included) | [optional]  |

### Return type

[**AppScreenshotSetResponse**](AppScreenshotSetResponse.md)

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
| **200** | Single AppScreenshotSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

