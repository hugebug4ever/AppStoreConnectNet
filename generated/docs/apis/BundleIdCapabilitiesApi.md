# AppStoreConnect.Net.Api.BundleIdCapabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BundleIdCapabilitiesCreateInstance**](BundleIdCapabilitiesApi.md#bundleidcapabilitiescreateinstance) | **POST** /v1/bundleIdCapabilities |  |
| [**BundleIdCapabilitiesDeleteInstance**](BundleIdCapabilitiesApi.md#bundleidcapabilitiesdeleteinstance) | **DELETE** /v1/bundleIdCapabilities/{id} |  |
| [**BundleIdCapabilitiesUpdateInstance**](BundleIdCapabilitiesApi.md#bundleidcapabilitiesupdateinstance) | **PATCH** /v1/bundleIdCapabilities/{id} |  |

<a id="bundleidcapabilitiescreateinstance"></a>
# **BundleIdCapabilitiesCreateInstance**
> BundleIdCapabilityResponse BundleIdCapabilitiesCreateInstance (BundleIdCapabilityCreateRequest bundleIdCapabilityCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **bundleIdCapabilityCreateRequest** | [**BundleIdCapabilityCreateRequest**](BundleIdCapabilityCreateRequest.md) | BundleIdCapability representation |  |

### Return type

[**BundleIdCapabilityResponse**](BundleIdCapabilityResponse.md)

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
| **201** | Single BundleIdCapability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="bundleidcapabilitiesdeleteinstance"></a>
# **BundleIdCapabilitiesDeleteInstance**
> void BundleIdCapabilitiesDeleteInstance (string id)




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

<a id="bundleidcapabilitiesupdateinstance"></a>
# **BundleIdCapabilitiesUpdateInstance**
> BundleIdCapabilityResponse BundleIdCapabilitiesUpdateInstance (string id, BundleIdCapabilityUpdateRequest bundleIdCapabilityUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **bundleIdCapabilityUpdateRequest** | [**BundleIdCapabilityUpdateRequest**](BundleIdCapabilityUpdateRequest.md) | BundleIdCapability representation |  |

### Return type

[**BundleIdCapabilityResponse**](BundleIdCapabilityResponse.md)

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
| **200** | Single BundleIdCapability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

