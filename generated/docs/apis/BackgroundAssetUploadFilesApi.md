# AppStoreConnect.Net.Api.BackgroundAssetUploadFilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetUploadFilesCreateInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilescreateinstance) | **POST** /v1/backgroundAssetUploadFiles |  |
| [**BackgroundAssetUploadFilesGetInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilesgetinstance) | **GET** /v1/backgroundAssetUploadFiles/{id} |  |
| [**BackgroundAssetUploadFilesUpdateInstance**](BackgroundAssetUploadFilesApi.md#backgroundassetuploadfilesupdateinstance) | **PATCH** /v1/backgroundAssetUploadFiles/{id} |  |

<a id="backgroundassetuploadfilescreateinstance"></a>
# **BackgroundAssetUploadFilesCreateInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesCreateInstance (BackgroundAssetUploadFileCreateRequest backgroundAssetUploadFileCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetUploadFileCreateRequest** | [**BackgroundAssetUploadFileCreateRequest**](BackgroundAssetUploadFileCreateRequest.md) | BackgroundAssetUploadFile representation |  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **201** | Single BackgroundAssetUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetuploadfilesgetinstance"></a>
# **BackgroundAssetUploadFilesGetInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesGetInstance (string id, List<string> fieldsBackgroundAssetUploadFiles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **200** | Single BackgroundAssetUploadFile |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetuploadfilesupdateinstance"></a>
# **BackgroundAssetUploadFilesUpdateInstance**
> BackgroundAssetUploadFileResponse BackgroundAssetUploadFilesUpdateInstance (string id, BackgroundAssetUploadFileUpdateRequest backgroundAssetUploadFileUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **backgroundAssetUploadFileUpdateRequest** | [**BackgroundAssetUploadFileUpdateRequest**](BackgroundAssetUploadFileUpdateRequest.md) | BackgroundAssetUploadFile representation |  |

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
| **200** | Single BackgroundAssetUploadFile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

