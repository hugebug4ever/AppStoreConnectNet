# AppStoreConnect.Net.Api.AppPreviewSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppPreviewSetsAppPreviewsGetToManyRelated**](AppPreviewSetsApi.md#apppreviewsetsapppreviewsgettomanyrelated) | **GET** /v1/appPreviewSets/{id}/appPreviews |  |
| [**AppPreviewSetsAppPreviewsGetToManyRelationship**](AppPreviewSetsApi.md#apppreviewsetsapppreviewsgettomanyrelationship) | **GET** /v1/appPreviewSets/{id}/relationships/appPreviews |  |
| [**AppPreviewSetsAppPreviewsReplaceToManyRelationship**](AppPreviewSetsApi.md#apppreviewsetsapppreviewsreplacetomanyrelationship) | **PATCH** /v1/appPreviewSets/{id}/relationships/appPreviews |  |
| [**AppPreviewSetsCreateInstance**](AppPreviewSetsApi.md#apppreviewsetscreateinstance) | **POST** /v1/appPreviewSets |  |
| [**AppPreviewSetsDeleteInstance**](AppPreviewSetsApi.md#apppreviewsetsdeleteinstance) | **DELETE** /v1/appPreviewSets/{id} |  |
| [**AppPreviewSetsGetInstance**](AppPreviewSetsApi.md#apppreviewsetsgetinstance) | **GET** /v1/appPreviewSets/{id} |  |

<a id="apppreviewsetsapppreviewsgettomanyrelated"></a>
# **AppPreviewSetsAppPreviewsGetToManyRelated**
> AppPreviewsResponse AppPreviewSetsAppPreviewsGetToManyRelated (string id, List<string> fieldsAppPreviews = null, List<string> fieldsAppPreviewSets = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppPreviews** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviews | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPreviewsResponse**](AppPreviewsResponse.md)

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
| **200** | List of AppPreviews |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppreviewsetsapppreviewsgettomanyrelationship"></a>
# **AppPreviewSetsAppPreviewsGetToManyRelationship**
> AppPreviewSetAppPreviewsLinkagesResponse AppPreviewSetsAppPreviewsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppPreviewSetAppPreviewsLinkagesResponse**](AppPreviewSetAppPreviewsLinkagesResponse.md)

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

<a id="apppreviewsetsapppreviewsreplacetomanyrelationship"></a>
# **AppPreviewSetsAppPreviewsReplaceToManyRelationship**
> void AppPreviewSetsAppPreviewsReplaceToManyRelationship (string id, AppPreviewSetAppPreviewsLinkagesRequest appPreviewSetAppPreviewsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appPreviewSetAppPreviewsLinkagesRequest** | [**AppPreviewSetAppPreviewsLinkagesRequest**](AppPreviewSetAppPreviewsLinkagesRequest.md) | List of related linkages |  |

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

<a id="apppreviewsetscreateinstance"></a>
# **AppPreviewSetsCreateInstance**
> AppPreviewSetResponse AppPreviewSetsCreateInstance (AppPreviewSetCreateRequest appPreviewSetCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appPreviewSetCreateRequest** | [**AppPreviewSetCreateRequest**](AppPreviewSetCreateRequest.md) | AppPreviewSet representation |  |

### Return type

[**AppPreviewSetResponse**](AppPreviewSetResponse.md)

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
| **201** | Single AppPreviewSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppreviewsetsdeleteinstance"></a>
# **AppPreviewSetsDeleteInstance**
> void AppPreviewSetsDeleteInstance (string id)




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

<a id="apppreviewsetsgetinstance"></a>
# **AppPreviewSetsGetInstance**
> AppPreviewSetResponse AppPreviewSetsGetInstance (string id, List<string> fieldsAppPreviewSets = null, List<string> fieldsAppPreviews = null, List<string> include = null, int limitAppPreviews = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **fieldsAppPreviews** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviews | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviews** | **int** | maximum number of related appPreviews returned (when they are included) | [optional]  |

### Return type

[**AppPreviewSetResponse**](AppPreviewSetResponse.md)

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
| **200** | Single AppPreviewSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

