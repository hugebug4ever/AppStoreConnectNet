# AppStoreConnect.Net.Api.BuildUploadFilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildUploadFilesCreateInstance**](BuildUploadFilesApi.md#builduploadfilescreateinstance) | **POST** /v1/buildUploadFiles |  |
| [**BuildUploadFilesGetInstance**](BuildUploadFilesApi.md#builduploadfilesgetinstance) | **GET** /v1/buildUploadFiles/{id} |  |
| [**BuildUploadFilesUpdateInstance**](BuildUploadFilesApi.md#builduploadfilesupdateinstance) | **PATCH** /v1/buildUploadFiles/{id} |  |

<a id="builduploadfilescreateinstance"></a>
# **BuildUploadFilesCreateInstance**
> BuildUploadFileResponse BuildUploadFilesCreateInstance (BuildUploadFileCreateRequest buildUploadFileCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **buildUploadFileCreateRequest** | [**BuildUploadFileCreateRequest**](BuildUploadFileCreateRequest.md) | BuildUploadFile representation |  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **201** | Single BuildUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="builduploadfilesgetinstance"></a>
# **BuildUploadFilesGetInstance**
> BuildUploadFileResponse BuildUploadFilesGetInstance (string id, List<string> fieldsBuildUploadFiles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildUploadFiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildUploadFiles | [optional]  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **200** | Single BuildUploadFile |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="builduploadfilesupdateinstance"></a>
# **BuildUploadFilesUpdateInstance**
> BuildUploadFileResponse BuildUploadFilesUpdateInstance (string id, BuildUploadFileUpdateRequest buildUploadFileUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildUploadFileUpdateRequest** | [**BuildUploadFileUpdateRequest**](BuildUploadFileUpdateRequest.md) | BuildUploadFile representation |  |

### Return type

[**BuildUploadFileResponse**](BuildUploadFileResponse.md)

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
| **200** | Single BuildUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

