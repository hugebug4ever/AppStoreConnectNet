# AppStoreConnect.Net.Api.AppCustomProductPageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelated) | **GET** /v1/appCustomProductPageVersions/{id}/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelationship) | **GET** /v1/appCustomProductPageVersions/{id}/relationships/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageVersionsCreateInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionscreateinstance) | **POST** /v1/appCustomProductPageVersions |  |
| [**AppCustomProductPageVersionsGetInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsgetinstance) | **GET** /v1/appCustomProductPageVersions/{id} |  |
| [**AppCustomProductPageVersionsUpdateInstance**](AppCustomProductPageVersionsApi.md#appcustomproductpageversionsupdateinstance) | **PATCH** /v1/appCustomProductPageVersions/{id} |  |

<a id="appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelated"></a>
# **AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated**
> AppCustomProductPageLocalizationsResponse AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelated (string id, List<string> filterLocale = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppCustomProductPageVersions = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppPreviewSets = null, List<string> fieldsAppKeywords = null, int limit = null, List<string> include = null, int limitAppScreenshotSets = null, int limitAppPreviewSets = null, int limitSearchKeywords = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLocale** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **fieldsAppKeywords** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appKeywords | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppScreenshotSets** | **int** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitAppPreviewSets** | **int** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageLocalizationsResponse**](AppCustomProductPageLocalizationsResponse.md)

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
| **200** | List of AppCustomProductPageLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpageversionsappcustomproductpagelocalizationsgettomanyrelationship"></a>
# **AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship**
> AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse AppCustomProductPageVersionsAppCustomProductPageLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse**](AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.md)

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

<a id="appcustomproductpageversionscreateinstance"></a>
# **AppCustomProductPageVersionsCreateInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsCreateInstance (AppCustomProductPageVersionCreateRequest appCustomProductPageVersionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageVersionCreateRequest** | [**AppCustomProductPageVersionCreateRequest**](AppCustomProductPageVersionCreateRequest.md) | AppCustomProductPageVersion representation |  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **201** | Single AppCustomProductPageVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpageversionsgetinstance"></a>
# **AppCustomProductPageVersionsGetInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsGetInstance (string id, List<string> fieldsAppCustomProductPageVersions = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> include = null, int limitAppCustomProductPageLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageLocalizations** | **int** | maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **200** | Single AppCustomProductPageVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpageversionsupdateinstance"></a>
# **AppCustomProductPageVersionsUpdateInstance**
> AppCustomProductPageVersionResponse AppCustomProductPageVersionsUpdateInstance (string id, AppCustomProductPageVersionUpdateRequest appCustomProductPageVersionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageVersionUpdateRequest** | [**AppCustomProductPageVersionUpdateRequest**](AppCustomProductPageVersionUpdateRequest.md) | AppCustomProductPageVersion representation |  |

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
| **200** | Single AppCustomProductPageVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

