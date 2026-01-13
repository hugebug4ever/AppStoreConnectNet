# AppStoreConnect.Net.Api.AppClipAdvancedExperiencesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipAdvancedExperiencesCreateInstance**](AppClipAdvancedExperiencesApi.md#appclipadvancedexperiencescreateinstance) | **POST** /v1/appClipAdvancedExperiences |  |
| [**AppClipAdvancedExperiencesGetInstance**](AppClipAdvancedExperiencesApi.md#appclipadvancedexperiencesgetinstance) | **GET** /v1/appClipAdvancedExperiences/{id} |  |
| [**AppClipAdvancedExperiencesUpdateInstance**](AppClipAdvancedExperiencesApi.md#appclipadvancedexperiencesupdateinstance) | **PATCH** /v1/appClipAdvancedExperiences/{id} |  |

<a id="appclipadvancedexperiencescreateinstance"></a>
# **AppClipAdvancedExperiencesCreateInstance**
> AppClipAdvancedExperienceResponse AppClipAdvancedExperiencesCreateInstance (AppClipAdvancedExperienceCreateRequest appClipAdvancedExperienceCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appClipAdvancedExperienceCreateRequest** | [**AppClipAdvancedExperienceCreateRequest**](AppClipAdvancedExperienceCreateRequest.md) | AppClipAdvancedExperience representation |  |

### Return type

[**AppClipAdvancedExperienceResponse**](AppClipAdvancedExperienceResponse.md)

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
| **201** | Single AppClipAdvancedExperience |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipadvancedexperiencesgetinstance"></a>
# **AppClipAdvancedExperiencesGetInstance**
> AppClipAdvancedExperienceResponse AppClipAdvancedExperiencesGetInstance (string id, List<string> fieldsAppClipAdvancedExperiences = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipAdvancedExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAdvancedExperiences | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**AppClipAdvancedExperienceResponse**](AppClipAdvancedExperienceResponse.md)

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
| **200** | Single AppClipAdvancedExperience |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipadvancedexperiencesupdateinstance"></a>
# **AppClipAdvancedExperiencesUpdateInstance**
> AppClipAdvancedExperienceResponse AppClipAdvancedExperiencesUpdateInstance (string id, AppClipAdvancedExperienceUpdateRequest appClipAdvancedExperienceUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appClipAdvancedExperienceUpdateRequest** | [**AppClipAdvancedExperienceUpdateRequest**](AppClipAdvancedExperienceUpdateRequest.md) | AppClipAdvancedExperience representation |  |

### Return type

[**AppClipAdvancedExperienceResponse**](AppClipAdvancedExperienceResponse.md)

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
| **200** | Single AppClipAdvancedExperience |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

