# AppStoreConnect.Net.Api.BackgroundAssetVersionAppStoreReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionAppStoreReleasesGetInstance**](BackgroundAssetVersionAppStoreReleasesApi.md#backgroundassetversionappstorereleasesgetinstance) | **GET** /v1/backgroundAssetVersionAppStoreReleases/{id} |  |

<a id="backgroundassetversionappstorereleasesgetinstance"></a>
# **BackgroundAssetVersionAppStoreReleasesGetInstance**
> BackgroundAssetVersionAppStoreReleaseResponse BackgroundAssetVersionAppStoreReleasesGetInstance (string id, List<string> fieldsBackgroundAssetVersionAppStoreReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersionAppStoreReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionAppStoreReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionAppStoreReleaseResponse**](BackgroundAssetVersionAppStoreReleaseResponse.md)

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
| **200** | Single BackgroundAssetVersionAppStoreRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

