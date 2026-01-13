# AppStoreConnect.Net.Api.AndroidToIosAppMappingDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AndroidToIosAppMappingDetailsCreateInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailscreateinstance) | **POST** /v1/androidToIosAppMappingDetails |  |
| [**AndroidToIosAppMappingDetailsDeleteInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsdeleteinstance) | **DELETE** /v1/androidToIosAppMappingDetails/{id} |  |
| [**AndroidToIosAppMappingDetailsGetInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsgetinstance) | **GET** /v1/androidToIosAppMappingDetails/{id} |  |
| [**AndroidToIosAppMappingDetailsUpdateInstance**](AndroidToIosAppMappingDetailsApi.md#androidtoiosappmappingdetailsupdateinstance) | **PATCH** /v1/androidToIosAppMappingDetails/{id} |  |

<a id="androidtoiosappmappingdetailscreateinstance"></a>
# **AndroidToIosAppMappingDetailsCreateInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsCreateInstance (AndroidToIosAppMappingDetailCreateRequest androidToIosAppMappingDetailCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **androidToIosAppMappingDetailCreateRequest** | [**AndroidToIosAppMappingDetailCreateRequest**](AndroidToIosAppMappingDetailCreateRequest.md) | AndroidToIosAppMappingDetail representation |  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **201** | Single AndroidToIosAppMappingDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="androidtoiosappmappingdetailsdeleteinstance"></a>
# **AndroidToIosAppMappingDetailsDeleteInstance**
> void AndroidToIosAppMappingDetailsDeleteInstance (string id)




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

<a id="androidtoiosappmappingdetailsgetinstance"></a>
# **AndroidToIosAppMappingDetailsGetInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsGetInstance (string id, List<string> fieldsAndroidToIosAppMappingDetails = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAndroidToIosAppMappingDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type androidToIosAppMappingDetails | [optional]  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **200** | Single AndroidToIosAppMappingDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="androidtoiosappmappingdetailsupdateinstance"></a>
# **AndroidToIosAppMappingDetailsUpdateInstance**
> AndroidToIosAppMappingDetailResponse AndroidToIosAppMappingDetailsUpdateInstance (string id, AndroidToIosAppMappingDetailUpdateRequest androidToIosAppMappingDetailUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **androidToIosAppMappingDetailUpdateRequest** | [**AndroidToIosAppMappingDetailUpdateRequest**](AndroidToIosAppMappingDetailUpdateRequest.md) | AndroidToIosAppMappingDetail representation |  |

### Return type

[**AndroidToIosAppMappingDetailResponse**](AndroidToIosAppMappingDetailResponse.md)

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
| **200** | Single AndroidToIosAppMappingDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

