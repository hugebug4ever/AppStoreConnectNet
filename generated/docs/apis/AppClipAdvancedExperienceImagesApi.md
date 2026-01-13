# AppStoreConnect.Net.Api.AppClipAdvancedExperienceImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipAdvancedExperienceImagesCreateInstance**](AppClipAdvancedExperienceImagesApi.md#appclipadvancedexperienceimagescreateinstance) | **POST** /v1/appClipAdvancedExperienceImages |  |
| [**AppClipAdvancedExperienceImagesGetInstance**](AppClipAdvancedExperienceImagesApi.md#appclipadvancedexperienceimagesgetinstance) | **GET** /v1/appClipAdvancedExperienceImages/{id} |  |
| [**AppClipAdvancedExperienceImagesUpdateInstance**](AppClipAdvancedExperienceImagesApi.md#appclipadvancedexperienceimagesupdateinstance) | **PATCH** /v1/appClipAdvancedExperienceImages/{id} |  |

<a id="appclipadvancedexperienceimagescreateinstance"></a>
# **AppClipAdvancedExperienceImagesCreateInstance**
> AppClipAdvancedExperienceImageResponse AppClipAdvancedExperienceImagesCreateInstance (AppClipAdvancedExperienceImageCreateRequest appClipAdvancedExperienceImageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appClipAdvancedExperienceImageCreateRequest** | [**AppClipAdvancedExperienceImageCreateRequest**](AppClipAdvancedExperienceImageCreateRequest.md) | AppClipAdvancedExperienceImage representation |  |

### Return type

[**AppClipAdvancedExperienceImageResponse**](AppClipAdvancedExperienceImageResponse.md)

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
| **201** | Single AppClipAdvancedExperienceImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipadvancedexperienceimagesgetinstance"></a>
# **AppClipAdvancedExperienceImagesGetInstance**
> AppClipAdvancedExperienceImageResponse AppClipAdvancedExperienceImagesGetInstance (string id, List<string> fieldsAppClipAdvancedExperienceImages = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipAdvancedExperienceImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAdvancedExperienceImages | [optional]  |

### Return type

[**AppClipAdvancedExperienceImageResponse**](AppClipAdvancedExperienceImageResponse.md)

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
| **200** | Single AppClipAdvancedExperienceImage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipadvancedexperienceimagesupdateinstance"></a>
# **AppClipAdvancedExperienceImagesUpdateInstance**
> AppClipAdvancedExperienceImageResponse AppClipAdvancedExperienceImagesUpdateInstance (string id, AppClipAdvancedExperienceImageUpdateRequest appClipAdvancedExperienceImageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appClipAdvancedExperienceImageUpdateRequest** | [**AppClipAdvancedExperienceImageUpdateRequest**](AppClipAdvancedExperienceImageUpdateRequest.md) | AppClipAdvancedExperienceImage representation |  |

### Return type

[**AppClipAdvancedExperienceImageResponse**](AppClipAdvancedExperienceImageResponse.md)

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
| **200** | Single AppClipAdvancedExperienceImage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

