# AppStoreConnect.Net.Api.AppInfosApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppInfosAgeRatingDeclarationGetToOneRelated**](AppInfosApi.md#appinfosageratingdeclarationgettoonerelated) | **GET** /v1/appInfos/{id}/ageRatingDeclaration |  |
| [**AppInfosAgeRatingDeclarationGetToOneRelationship**](AppInfosApi.md#appinfosageratingdeclarationgettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/ageRatingDeclaration |  |
| [**AppInfosAppInfoLocalizationsGetToManyRelated**](AppInfosApi.md#appinfosappinfolocalizationsgettomanyrelated) | **GET** /v1/appInfos/{id}/appInfoLocalizations |  |
| [**AppInfosAppInfoLocalizationsGetToManyRelationship**](AppInfosApi.md#appinfosappinfolocalizationsgettomanyrelationship) | **GET** /v1/appInfos/{id}/relationships/appInfoLocalizations |  |
| [**AppInfosGetInstance**](AppInfosApi.md#appinfosgetinstance) | **GET** /v1/appInfos/{id} |  |
| [**AppInfosPrimaryCategoryGetToOneRelated**](AppInfosApi.md#appinfosprimarycategorygettoonerelated) | **GET** /v1/appInfos/{id}/primaryCategory |  |
| [**AppInfosPrimaryCategoryGetToOneRelationship**](AppInfosApi.md#appinfosprimarycategorygettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primaryCategory |  |
| [**AppInfosPrimarySubcategoryOneGetToOneRelated**](AppInfosApi.md#appinfosprimarysubcategoryonegettoonerelated) | **GET** /v1/appInfos/{id}/primarySubcategoryOne |  |
| [**AppInfosPrimarySubcategoryOneGetToOneRelationship**](AppInfosApi.md#appinfosprimarysubcategoryonegettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryOne |  |
| [**AppInfosPrimarySubcategoryTwoGetToOneRelated**](AppInfosApi.md#appinfosprimarysubcategorytwogettoonerelated) | **GET** /v1/appInfos/{id}/primarySubcategoryTwo |  |
| [**AppInfosPrimarySubcategoryTwoGetToOneRelationship**](AppInfosApi.md#appinfosprimarysubcategorytwogettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryTwo |  |
| [**AppInfosSecondaryCategoryGetToOneRelated**](AppInfosApi.md#appinfossecondarycategorygettoonerelated) | **GET** /v1/appInfos/{id}/secondaryCategory |  |
| [**AppInfosSecondaryCategoryGetToOneRelationship**](AppInfosApi.md#appinfossecondarycategorygettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondaryCategory |  |
| [**AppInfosSecondarySubcategoryOneGetToOneRelated**](AppInfosApi.md#appinfossecondarysubcategoryonegettoonerelated) | **GET** /v1/appInfos/{id}/secondarySubcategoryOne |  |
| [**AppInfosSecondarySubcategoryOneGetToOneRelationship**](AppInfosApi.md#appinfossecondarysubcategoryonegettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryOne |  |
| [**AppInfosSecondarySubcategoryTwoGetToOneRelated**](AppInfosApi.md#appinfossecondarysubcategorytwogettoonerelated) | **GET** /v1/appInfos/{id}/secondarySubcategoryTwo |  |
| [**AppInfosSecondarySubcategoryTwoGetToOneRelationship**](AppInfosApi.md#appinfossecondarysubcategorytwogettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryTwo |  |
| [**AppInfosTerritoryAgeRatingsGetToManyRelated**](AppInfosApi.md#appinfosterritoryageratingsgettomanyrelated) | **GET** /v1/appInfos/{id}/territoryAgeRatings |  |
| [**AppInfosTerritoryAgeRatingsGetToManyRelationship**](AppInfosApi.md#appinfosterritoryageratingsgettomanyrelationship) | **GET** /v1/appInfos/{id}/relationships/territoryAgeRatings |  |
| [**AppInfosUpdateInstance**](AppInfosApi.md#appinfosupdateinstance) | **PATCH** /v1/appInfos/{id} |  |

<a id="appinfosageratingdeclarationgettoonerelated"></a>
# **AppInfosAgeRatingDeclarationGetToOneRelated**
> AgeRatingDeclarationResponse AppInfosAgeRatingDeclarationGetToOneRelated (string id, List<string> fieldsAgeRatingDeclarations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |

### Return type

[**AgeRatingDeclarationResponse**](AgeRatingDeclarationResponse.md)

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
| **200** | Single AgeRatingDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appinfosageratingdeclarationgettoonerelationship"></a>
# **AppInfosAgeRatingDeclarationGetToOneRelationship**
> AppInfoAgeRatingDeclarationLinkageResponse AppInfosAgeRatingDeclarationGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoAgeRatingDeclarationLinkageResponse**](AppInfoAgeRatingDeclarationLinkageResponse.md)

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

<a id="appinfosappinfolocalizationsgettomanyrelated"></a>
# **AppInfosAppInfoLocalizationsGetToManyRelated**
> AppInfoLocalizationsResponse AppInfosAppInfoLocalizationsGetToManyRelated (string id, List<string> filterLocale = null, List<string> fieldsAppInfoLocalizations = null, List<string> fieldsAppInfos = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLocale** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **fieldsAppInfoLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appInfoLocalizations | [optional]  |
| **fieldsAppInfos** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppInfoLocalizationsResponse**](AppInfoLocalizationsResponse.md)

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
| **200** | List of AppInfoLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appinfosappinfolocalizationsgettomanyrelationship"></a>
# **AppInfosAppInfoLocalizationsGetToManyRelationship**
> AppInfoAppInfoLocalizationsLinkagesResponse AppInfosAppInfoLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppInfoAppInfoLocalizationsLinkagesResponse**](AppInfoAppInfoLocalizationsLinkagesResponse.md)

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

<a id="appinfosgetinstance"></a>
# **AppInfosGetInstance**
> AppInfoResponse AppInfosGetInstance (string id, List<string> fieldsAppInfos = null, List<string> fieldsAgeRatingDeclarations = null, List<string> fieldsAppInfoLocalizations = null, List<string> fieldsAppCategories = null, List<string> include = null, int limitAppInfoLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppInfos** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppInfoLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appInfoLocalizations | [optional]  |
| **fieldsAppCategories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppInfoLocalizations** | **int** | maximum number of related appInfoLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
| **200** | Single AppInfo |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appinfosprimarycategorygettoonerelated"></a>
# **AppInfosPrimaryCategoryGetToOneRelated**
> AppCategoryResponse AppInfosPrimaryCategoryGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfosprimarycategorygettoonerelationship"></a>
# **AppInfosPrimaryCategoryGetToOneRelationship**
> AppInfoPrimaryCategoryLinkageResponse AppInfosPrimaryCategoryGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimaryCategoryLinkageResponse**](AppInfoPrimaryCategoryLinkageResponse.md)

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

<a id="appinfosprimarysubcategoryonegettoonerelated"></a>
# **AppInfosPrimarySubcategoryOneGetToOneRelated**
> AppCategoryResponse AppInfosPrimarySubcategoryOneGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfosprimarysubcategoryonegettoonerelationship"></a>
# **AppInfosPrimarySubcategoryOneGetToOneRelationship**
> AppInfoPrimarySubcategoryOneLinkageResponse AppInfosPrimarySubcategoryOneGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimarySubcategoryOneLinkageResponse**](AppInfoPrimarySubcategoryOneLinkageResponse.md)

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

<a id="appinfosprimarysubcategorytwogettoonerelated"></a>
# **AppInfosPrimarySubcategoryTwoGetToOneRelated**
> AppCategoryResponse AppInfosPrimarySubcategoryTwoGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfosprimarysubcategorytwogettoonerelationship"></a>
# **AppInfosPrimarySubcategoryTwoGetToOneRelationship**
> AppInfoPrimarySubcategoryTwoLinkageResponse AppInfosPrimarySubcategoryTwoGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimarySubcategoryTwoLinkageResponse**](AppInfoPrimarySubcategoryTwoLinkageResponse.md)

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

<a id="appinfossecondarycategorygettoonerelated"></a>
# **AppInfosSecondaryCategoryGetToOneRelated**
> AppCategoryResponse AppInfosSecondaryCategoryGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfossecondarycategorygettoonerelationship"></a>
# **AppInfosSecondaryCategoryGetToOneRelationship**
> AppInfoSecondaryCategoryLinkageResponse AppInfosSecondaryCategoryGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondaryCategoryLinkageResponse**](AppInfoSecondaryCategoryLinkageResponse.md)

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

<a id="appinfossecondarysubcategoryonegettoonerelated"></a>
# **AppInfosSecondarySubcategoryOneGetToOneRelated**
> AppCategoryResponse AppInfosSecondarySubcategoryOneGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfossecondarysubcategoryonegettoonerelationship"></a>
# **AppInfosSecondarySubcategoryOneGetToOneRelationship**
> AppInfoSecondarySubcategoryOneLinkageResponse AppInfosSecondarySubcategoryOneGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondarySubcategoryOneLinkageResponse**](AppInfoSecondarySubcategoryOneLinkageResponse.md)

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

<a id="appinfossecondarysubcategorytwogettoonerelated"></a>
# **AppInfosSecondarySubcategoryTwoGetToOneRelated**
> AppCategoryResponse AppInfosSecondarySubcategoryTwoGetToOneRelated (string id, List<string> fieldsAppCategories = null, List<string> include = null, int limitSubcategories = null)




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

<a id="appinfossecondarysubcategorytwogettoonerelationship"></a>
# **AppInfosSecondarySubcategoryTwoGetToOneRelationship**
> AppInfoSecondarySubcategoryTwoLinkageResponse AppInfosSecondarySubcategoryTwoGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondarySubcategoryTwoLinkageResponse**](AppInfoSecondarySubcategoryTwoLinkageResponse.md)

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

<a id="appinfosterritoryageratingsgettomanyrelated"></a>
# **AppInfosTerritoryAgeRatingsGetToManyRelated**
> TerritoryAgeRatingsResponse AppInfosTerritoryAgeRatingsGetToManyRelated (string id, List<string> fieldsTerritoryAgeRatings = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritoryAgeRatings** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territoryAgeRatings | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**TerritoryAgeRatingsResponse**](TerritoryAgeRatingsResponse.md)

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
| **200** | List of TerritoryAgeRatings |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appinfosterritoryageratingsgettomanyrelationship"></a>
# **AppInfosTerritoryAgeRatingsGetToManyRelationship**
> AppInfoTerritoryAgeRatingsLinkagesResponse AppInfosTerritoryAgeRatingsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppInfoTerritoryAgeRatingsLinkagesResponse**](AppInfoTerritoryAgeRatingsLinkagesResponse.md)

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

<a id="appinfosupdateinstance"></a>
# **AppInfosUpdateInstance**
> AppInfoResponse AppInfosUpdateInstance (string id, AppInfoUpdateRequest appInfoUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appInfoUpdateRequest** | [**AppInfoUpdateRequest**](AppInfoUpdateRequest.md) | AppInfo representation |  |

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
| **200** | Single AppInfo |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

