# AppStoreConnect.Net.Api.AccessibilityDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AccessibilityDeclarationsCreateInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationscreateinstance) | **POST** /v1/accessibilityDeclarations |  |
| [**AccessibilityDeclarationsDeleteInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsdeleteinstance) | **DELETE** /v1/accessibilityDeclarations/{id} |  |
| [**AccessibilityDeclarationsGetInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsgetinstance) | **GET** /v1/accessibilityDeclarations/{id} |  |
| [**AccessibilityDeclarationsUpdateInstance**](AccessibilityDeclarationsApi.md#accessibilitydeclarationsupdateinstance) | **PATCH** /v1/accessibilityDeclarations/{id} |  |

<a id="accessibilitydeclarationscreateinstance"></a>
# **AccessibilityDeclarationsCreateInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsCreateInstance (AccessibilityDeclarationCreateRequest accessibilityDeclarationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **accessibilityDeclarationCreateRequest** | [**AccessibilityDeclarationCreateRequest**](AccessibilityDeclarationCreateRequest.md) | AccessibilityDeclaration representation |  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **201** | Single AccessibilityDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="accessibilitydeclarationsdeleteinstance"></a>
# **AccessibilityDeclarationsDeleteInstance**
> void AccessibilityDeclarationsDeleteInstance (string id)




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

<a id="accessibilitydeclarationsgetinstance"></a>
# **AccessibilityDeclarationsGetInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsGetInstance (string id, List<string> fieldsAccessibilityDeclarations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAccessibilityDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type accessibilityDeclarations | [optional]  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **200** | Single AccessibilityDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="accessibilitydeclarationsupdateinstance"></a>
# **AccessibilityDeclarationsUpdateInstance**
> AccessibilityDeclarationResponse AccessibilityDeclarationsUpdateInstance (string id, AccessibilityDeclarationUpdateRequest accessibilityDeclarationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **accessibilityDeclarationUpdateRequest** | [**AccessibilityDeclarationUpdateRequest**](AccessibilityDeclarationUpdateRequest.md) | AccessibilityDeclaration representation |  |

### Return type

[**AccessibilityDeclarationResponse**](AccessibilityDeclarationResponse.md)

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
| **200** | Single AccessibilityDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

