# AppStoreConnect.Net.Api.AppCustomProductPagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated**](AppCustomProductPagesApi.md#appcustomproductpagesappcustomproductpageversionsgettomanyrelated) | **GET** /v1/appCustomProductPages/{id}/appCustomProductPageVersions |  |
| [**AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship**](AppCustomProductPagesApi.md#appcustomproductpagesappcustomproductpageversionsgettomanyrelationship) | **GET** /v1/appCustomProductPages/{id}/relationships/appCustomProductPageVersions |  |
| [**AppCustomProductPagesCreateInstance**](AppCustomProductPagesApi.md#appcustomproductpagescreateinstance) | **POST** /v1/appCustomProductPages |  |
| [**AppCustomProductPagesDeleteInstance**](AppCustomProductPagesApi.md#appcustomproductpagesdeleteinstance) | **DELETE** /v1/appCustomProductPages/{id} |  |
| [**AppCustomProductPagesGetInstance**](AppCustomProductPagesApi.md#appcustomproductpagesgetinstance) | **GET** /v1/appCustomProductPages/{id} |  |
| [**AppCustomProductPagesUpdateInstance**](AppCustomProductPagesApi.md#appcustomproductpagesupdateinstance) | **PATCH** /v1/appCustomProductPages/{id} |  |

<a id="appcustomproductpagesappcustomproductpageversionsgettomanyrelated"></a>
# **AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated**
> AppCustomProductPageVersionsResponse AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelated (string id, List<string> filterState = null, List<string> fieldsAppCustomProductPageVersions = null, List<string> fieldsAppCustomProductPages = null, List<string> fieldsAppCustomProductPageLocalizations = null, int limit = null, List<string> include = null, int limitAppCustomProductPageLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageLocalizations** | **int** | maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageVersionsResponse**](AppCustomProductPageVersionsResponse.md)

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
| **200** | List of AppCustomProductPageVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpagesappcustomproductpageversionsgettomanyrelationship"></a>
# **AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship**
> AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse AppCustomProductPagesAppCustomProductPageVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse**](AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.md)

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

<a id="appcustomproductpagescreateinstance"></a>
# **AppCustomProductPagesCreateInstance**
> AppCustomProductPageResponse AppCustomProductPagesCreateInstance (AppCustomProductPageCreateRequest appCustomProductPageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageCreateRequest** | [**AppCustomProductPageCreateRequest**](AppCustomProductPageCreateRequest.md) | AppCustomProductPage representation |  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **201** | Single AppCustomProductPage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpagesdeleteinstance"></a>
# **AppCustomProductPagesDeleteInstance**
> void AppCustomProductPagesDeleteInstance (string id)




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

<a id="appcustomproductpagesgetinstance"></a>
# **AppCustomProductPagesGetInstance**
> AppCustomProductPageResponse AppCustomProductPagesGetInstance (string id, List<string> fieldsAppCustomProductPages = null, List<string> fieldsAppCustomProductPageVersions = null, List<string> include = null, int limitAppCustomProductPageVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPages | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppCustomProductPageVersions** | **int** | maximum number of related appCustomProductPageVersions returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **200** | Single AppCustomProductPage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpagesupdateinstance"></a>
# **AppCustomProductPagesUpdateInstance**
> AppCustomProductPageResponse AppCustomProductPagesUpdateInstance (string id, AppCustomProductPageUpdateRequest appCustomProductPageUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageUpdateRequest** | [**AppCustomProductPageUpdateRequest**](AppCustomProductPageUpdateRequest.md) | AppCustomProductPage representation |  |

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
| **200** | Single AppCustomProductPage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

