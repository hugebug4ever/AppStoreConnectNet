# AppStoreConnect.Net.Api.BackgroundAssetVersionExternalBetaReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionExternalBetaReleasesGetInstance**](BackgroundAssetVersionExternalBetaReleasesApi.md#backgroundassetversionexternalbetareleasesgetinstance) | **GET** /v1/backgroundAssetVersionExternalBetaReleases/{id} |  |

<a id="backgroundassetversionexternalbetareleasesgetinstance"></a>
# **BackgroundAssetVersionExternalBetaReleasesGetInstance**
> BackgroundAssetVersionExternalBetaReleaseResponse BackgroundAssetVersionExternalBetaReleasesGetInstance (string id, List<string> fieldsBackgroundAssetVersionExternalBetaReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersionExternalBetaReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionExternalBetaReleaseResponse**](BackgroundAssetVersionExternalBetaReleaseResponse.md)

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
| **200** | Single BackgroundAssetVersionExternalBetaRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

