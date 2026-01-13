# AppStoreConnect.Net.Api.BackgroundAssetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetsCreateInstance**](BackgroundAssetsApi.md#backgroundassetscreateinstance) | **POST** /v1/backgroundAssets |  |
| [**BackgroundAssetsGetInstance**](BackgroundAssetsApi.md#backgroundassetsgetinstance) | **GET** /v1/backgroundAssets/{id} |  |
| [**BackgroundAssetsUpdateInstance**](BackgroundAssetsApi.md#backgroundassetsupdateinstance) | **PATCH** /v1/backgroundAssets/{id} |  |
| [**BackgroundAssetsVersionsGetToManyRelated**](BackgroundAssetsApi.md#backgroundassetsversionsgettomanyrelated) | **GET** /v1/backgroundAssets/{id}/versions |  |
| [**BackgroundAssetsVersionsGetToManyRelationship**](BackgroundAssetsApi.md#backgroundassetsversionsgettomanyrelationship) | **GET** /v1/backgroundAssets/{id}/relationships/versions |  |

<a id="backgroundassetscreateinstance"></a>
# **BackgroundAssetsCreateInstance**
> BackgroundAssetResponse BackgroundAssetsCreateInstance (BackgroundAssetCreateRequest backgroundAssetCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **backgroundAssetCreateRequest** | [**BackgroundAssetCreateRequest**](BackgroundAssetCreateRequest.md) | BackgroundAsset representation |  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **201** | Single BackgroundAsset |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetsgetinstance"></a>
# **BackgroundAssetsGetInstance**
> BackgroundAssetResponse BackgroundAssetsGetInstance (string id, List<string> fieldsBackgroundAssets = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssets | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **200** | Single BackgroundAsset |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetsupdateinstance"></a>
# **BackgroundAssetsUpdateInstance**
> BackgroundAssetResponse BackgroundAssetsUpdateInstance (string id, BackgroundAssetUpdateRequest backgroundAssetUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **backgroundAssetUpdateRequest** | [**BackgroundAssetUpdateRequest**](BackgroundAssetUpdateRequest.md) | BackgroundAsset representation |  |

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
| **200** | Single BackgroundAsset |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetsversionsgettomanyrelated"></a>
# **BackgroundAssetsVersionsGetToManyRelated**
> BackgroundAssetVersionsResponse BackgroundAssetsVersionsGetToManyRelated (string id, List<string> filterState = null, List<string> filterVersion = null, List<string> filterInternalBetaReleaseState = null, List<string> filterExternalBetaReleaseState = null, List<string> filterAppStoreReleaseState = null, List<string> sort = null, List<string> fieldsBackgroundAssetVersions = null, List<string> fieldsBackgroundAssets = null, List<string> fieldsBackgroundAssetVersionInternalBetaReleases = null, List<string> fieldsBackgroundAssetVersionExternalBetaReleases = null, List<string> fieldsBackgroundAssetVersionAppStoreReleases = null, List<string> fieldsBackgroundAssetUploadFiles = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **filterVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterInternalBetaReleaseState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;internalBetaRelease.state&#39; | [optional]  |
| **filterExternalBetaReleaseState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;externalBetaRelease.state&#39; | [optional]  |
| **filterAppStoreReleaseState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;appStoreRelease.state&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBackgroundAssetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersions | [optional]  |
| **fieldsBackgroundAssets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssets | [optional]  |
| **fieldsBackgroundAssetVersionInternalBetaReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases | [optional]  |
| **fieldsBackgroundAssetVersionExternalBetaReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases | [optional]  |
| **fieldsBackgroundAssetVersionAppStoreReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionAppStoreReleases | [optional]  |
| **fieldsBackgroundAssetUploadFiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetUploadFiles | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionsResponse**](BackgroundAssetVersionsResponse.md)

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
| **200** | List of BackgroundAssetVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="backgroundassetsversionsgettomanyrelationship"></a>
# **BackgroundAssetsVersionsGetToManyRelationship**
> BackgroundAssetVersionsLinkagesResponse BackgroundAssetsVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BackgroundAssetVersionsLinkagesResponse**](BackgroundAssetVersionsLinkagesResponse.md)

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

