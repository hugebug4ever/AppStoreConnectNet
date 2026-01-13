# AppStoreConnect.Net.Api.AppCategoriesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCategoriesGetCollection**](AppCategoriesApi.md#appcategoriesgetcollection) | **GET** /v1/appCategories |  |
| [**AppCategoriesGetInstance**](AppCategoriesApi.md#appcategoriesgetinstance) | **GET** /v1/appCategories/{id} |  |
| [**AppCategoriesParentGetToOneRelated**](AppCategoriesApi.md#appcategoriesparentgettoonerelated) | **GET** /v1/appCategories/{id}/parent |  |
| [**AppCategoriesParentGetToOneRelationship**](AppCategoriesApi.md#appcategoriesparentgettoonerelationship) | **GET** /v1/appCategories/{id}/relationships/parent |  |
| [**AppCategoriesSubcategoriesGetToManyRelated**](AppCategoriesApi.md#appcategoriessubcategoriesgettomanyrelated) | **GET** /v1/appCategories/{id}/subcategories |  |
| [**AppCategoriesSubcategoriesGetToManyRelationship**](AppCategoriesApi.md#appcategoriessubcategoriesgettomanyrelationship) | **GET** /v1/appCategories/{id}/relationships/subcategories |  |

<a id="appcategoriesgetcollection"></a>
# **AppCategoriesGetCollection**
> AppCategoriesResponse AppCategoriesGetCollection (List<string> filterPlatforms = null, bool existsParent = null, List<string> fieldsAppCategories = null, int limit = null, List<string> include = null, int limitSubcategories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterPlatforms** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platforms&#39; | [optional]  |
| **existsParent** | **bool** | filter by existence or non-existence of related &#39;parent&#39; | [optional]  |
| **fieldsAppCategories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoriesResponse**](AppCategoriesResponse.md)

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
| **200** | List of AppCategories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcategoriesgetinstance"></a>
# **AppCategoriesGetInstance**
> AppCategoryResponse AppCategoriesGetInstance (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcategoriesparentgettoonerelated"></a>
# **AppCategoriesParentGetToOneRelated**
> AppCategoryWithoutIncludesResponse AppCategoriesParentGetToOneRelated (string id, List<string> fieldsAppCategories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |

### Return type

[**AppCategoryWithoutIncludesResponse**](AppCategoryWithoutIncludesResponse.md)

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
| **200** | Single AppCategory with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcategoriesparentgettoonerelationship"></a>
# **AppCategoriesParentGetToOneRelationship**
> AppCategoryParentLinkageResponse AppCategoriesParentGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppCategoryParentLinkageResponse**](AppCategoryParentLinkageResponse.md)

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
| **200** | Related linkage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcategoriessubcategoriesgettomanyrelated"></a>
# **AppCategoriesSubcategoriesGetToManyRelated**
> AppCategoriesWithoutIncludesResponse AppCategoriesSubcategoriesGetToManyRelated (string id, List<string> fieldsAppCategories = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCategoriesWithoutIncludesResponse**](AppCategoriesWithoutIncludesResponse.md)

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
| **200** | List of AppCategories with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcategoriessubcategoriesgettomanyrelationship"></a>
# **AppCategoriesSubcategoriesGetToManyRelationship**
> AppCategorySubcategoriesLinkagesResponse AppCategoriesSubcategoriesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCategorySubcategoriesLinkagesResponse**](AppCategorySubcategoriesLinkagesResponse.md)

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

