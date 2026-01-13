# AppStoreConnect.Net.Api.AppStoreVersionPhasedReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionPhasedReleasesCreateInstance**](AppStoreVersionPhasedReleasesApi.md#appstoreversionphasedreleasescreateinstance) | **POST** /v1/appStoreVersionPhasedReleases |  |
| [**AppStoreVersionPhasedReleasesDeleteInstance**](AppStoreVersionPhasedReleasesApi.md#appstoreversionphasedreleasesdeleteinstance) | **DELETE** /v1/appStoreVersionPhasedReleases/{id} |  |
| [**AppStoreVersionPhasedReleasesUpdateInstance**](AppStoreVersionPhasedReleasesApi.md#appstoreversionphasedreleasesupdateinstance) | **PATCH** /v1/appStoreVersionPhasedReleases/{id} |  |

<a id="appstoreversionphasedreleasescreateinstance"></a>
# **AppStoreVersionPhasedReleasesCreateInstance**
> AppStoreVersionPhasedReleaseResponse AppStoreVersionPhasedReleasesCreateInstance (AppStoreVersionPhasedReleaseCreateRequest appStoreVersionPhasedReleaseCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionPhasedReleaseCreateRequest** | [**AppStoreVersionPhasedReleaseCreateRequest**](AppStoreVersionPhasedReleaseCreateRequest.md) | AppStoreVersionPhasedRelease representation |  |

### Return type

[**AppStoreVersionPhasedReleaseResponse**](AppStoreVersionPhasedReleaseResponse.md)

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
| **201** | Single AppStoreVersionPhasedRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionphasedreleasesdeleteinstance"></a>
# **AppStoreVersionPhasedReleasesDeleteInstance**
> void AppStoreVersionPhasedReleasesDeleteInstance (string id)




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

<a id="appstoreversionphasedreleasesupdateinstance"></a>
# **AppStoreVersionPhasedReleasesUpdateInstance**
> AppStoreVersionPhasedReleaseResponse AppStoreVersionPhasedReleasesUpdateInstance (string id, AppStoreVersionPhasedReleaseUpdateRequest appStoreVersionPhasedReleaseUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionPhasedReleaseUpdateRequest** | [**AppStoreVersionPhasedReleaseUpdateRequest**](AppStoreVersionPhasedReleaseUpdateRequest.md) | AppStoreVersionPhasedRelease representation |  |

### Return type

[**AppStoreVersionPhasedReleaseResponse**](AppStoreVersionPhasedReleaseResponse.md)

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
| **200** | Single AppStoreVersionPhasedRelease |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

