# AppStoreConnect.Net.Api.BackgroundAssetVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated**](BackgroundAssetVersionsApi.md#backgroundassetversionsbackgroundassetuploadfilesgettomanyrelated) | **GET** /v1/backgroundAssetVersions/{id}/backgroundAssetUploadFiles |  |
| [**BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship**](BackgroundAssetVersionsApi.md#backgroundassetversionsbackgroundassetuploadfilesgettomanyrelationship) | **GET** /v1/backgroundAssetVersions/{id}/relationships/backgroundAssetUploadFiles |  |
| [**BackgroundAssetVersionsCreateInstance**](BackgroundAssetVersionsApi.md#backgroundassetversionscreateinstance) | **POST** /v1/backgroundAssetVersions |  |
| [**BackgroundAssetVersionsGetInstance**](BackgroundAssetVersionsApi.md#backgroundassetversionsgetinstance) | **GET** /v1/backgroundAssetVersions/{id} |  |

<a id="backgroundassetversionsbackgroundassetuploadfilesgettomanyrelated"></a>
# **BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated**
> BackgroundAssetUploadFilesResponse BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelated (string id, List<string> fieldsBackgroundAssetUploadFiles = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BackgroundAssetUploadFilesResponse**](BackgroundAssetUploadFilesResponse.md)

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
| **200** | List of BackgroundAssetUploadFiles |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetversionsbackgroundassetuploadfilesgettomanyrelationship"></a>
# **BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship**
> BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse BackgroundAssetVersionsBackgroundAssetUploadFilesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse**](BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.md)

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

<a id="backgroundassetversionscreateinstance"></a>
# **BackgroundAssetVersionsCreateInstance**
> BackgroundAssetVersionResponse BackgroundAssetVersionsCreateInstance (BackgroundAssetVersionCreateRequest backgroundAssetVersionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetVersionCreateRequest** | [**BackgroundAssetVersionCreateRequest**](BackgroundAssetVersionCreateRequest.md) | BackgroundAssetVersion representation |  |

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
| **201** | Single BackgroundAssetVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetversionsgetinstance"></a>
# **BackgroundAssetVersionsGetInstance**
> BackgroundAssetVersionResponse BackgroundAssetVersionsGetInstance (string id, List<string> fieldsBackgroundAssetVersions = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
| **200** | Single BackgroundAssetVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

