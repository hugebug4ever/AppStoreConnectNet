# AppStoreConnect.Net.Api.BackgroundAssetVersionInternalBetaReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionInternalBetaReleasesGetInstance**](BackgroundAssetVersionInternalBetaReleasesApi.md#backgroundassetversioninternalbetareleasesgetinstance) | **GET** /v1/backgroundAssetVersionInternalBetaReleases/{id} |  |

<a id="backgroundassetversioninternalbetareleasesgetinstance"></a>
# **BackgroundAssetVersionInternalBetaReleasesGetInstance**
> BackgroundAssetVersionInternalBetaReleaseResponse BackgroundAssetVersionInternalBetaReleasesGetInstance (string id, List<string> fieldsBackgroundAssetVersionInternalBetaReleases = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersionInternalBetaReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionInternalBetaReleaseResponse**](BackgroundAssetVersionInternalBetaReleaseResponse.md)

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
| **200** | Single BackgroundAssetVersionInternalBetaRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

