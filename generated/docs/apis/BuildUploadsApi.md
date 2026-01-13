# AppStoreConnect.Net.Api.BuildUploadsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildUploadsBuildUploadFilesGetToManyRelated**](BuildUploadsApi.md#builduploadsbuilduploadfilesgettomanyrelated) | **GET** /v1/buildUploads/{id}/buildUploadFiles |  |
| [**BuildUploadsBuildUploadFilesGetToManyRelationship**](BuildUploadsApi.md#builduploadsbuilduploadfilesgettomanyrelationship) | **GET** /v1/buildUploads/{id}/relationships/buildUploadFiles |  |
| [**BuildUploadsCreateInstance**](BuildUploadsApi.md#builduploadscreateinstance) | **POST** /v1/buildUploads |  |
| [**BuildUploadsDeleteInstance**](BuildUploadsApi.md#builduploadsdeleteinstance) | **DELETE** /v1/buildUploads/{id} |  |
| [**BuildUploadsGetInstance**](BuildUploadsApi.md#builduploadsgetinstance) | **GET** /v1/buildUploads/{id} |  |

<a id="builduploadsbuilduploadfilesgettomanyrelated"></a>
# **BuildUploadsBuildUploadFilesGetToManyRelated**
> BuildUploadFilesResponse BuildUploadsBuildUploadFilesGetToManyRelated (string id, List<string> fieldsBuildUploadFiles = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildUploadFiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildUploadFiles | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildUploadFilesResponse**](BuildUploadFilesResponse.md)

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
| **200** | List of BuildUploadFiles |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="builduploadsbuilduploadfilesgettomanyrelationship"></a>
# **BuildUploadsBuildUploadFilesGetToManyRelationship**
> BuildUploadBuildUploadFilesLinkagesResponse BuildUploadsBuildUploadFilesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildUploadBuildUploadFilesLinkagesResponse**](BuildUploadBuildUploadFilesLinkagesResponse.md)

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

<a id="builduploadscreateinstance"></a>
# **BuildUploadsCreateInstance**
> BuildUploadResponse BuildUploadsCreateInstance (BuildUploadCreateRequest buildUploadCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **buildUploadCreateRequest** | [**BuildUploadCreateRequest**](BuildUploadCreateRequest.md) | BuildUpload representation |  |

### Return type

[**BuildUploadResponse**](BuildUploadResponse.md)

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
| **201** | Single BuildUpload |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="builduploadsdeleteinstance"></a>
# **BuildUploadsDeleteInstance**
> void BuildUploadsDeleteInstance (string id)




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

<a id="builduploadsgetinstance"></a>
# **BuildUploadsGetInstance**
> BuildUploadResponse BuildUploadsGetInstance (string id, List<string> fieldsBuildUploads = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildUploads** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildUploads | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BuildUploadResponse**](BuildUploadResponse.md)

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
| **200** | Single BuildUpload |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

