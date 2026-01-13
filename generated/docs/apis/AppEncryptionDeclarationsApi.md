# AppStoreConnect.Net.Api.AppEncryptionDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelated) | **GET** /v1/appEncryptionDeclarations/{id}/appEncryptionDeclarationDocument |  |
| [**AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/appEncryptionDeclarationDocument |  |
| [**AppEncryptionDeclarationsAppGetToOneRelated**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappgettoonerelated) | **GET** /v1/appEncryptionDeclarations/{id}/app |  |
| [**AppEncryptionDeclarationsAppGetToOneRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsappgettoonerelationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/app |  |
| [**AppEncryptionDeclarationsBuildsCreateToManyRelationship**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsbuildscreatetomanyrelationship) | **POST** /v1/appEncryptionDeclarations/{id}/relationships/builds |  |
| [**AppEncryptionDeclarationsCreateInstance**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationscreateinstance) | **POST** /v1/appEncryptionDeclarations |  |
| [**AppEncryptionDeclarationsGetCollection**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsgetcollection) | **GET** /v1/appEncryptionDeclarations |  |
| [**AppEncryptionDeclarationsGetInstance**](AppEncryptionDeclarationsApi.md#appencryptiondeclarationsgetinstance) | **GET** /v1/appEncryptionDeclarations/{id} |  |

<a id="appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelated"></a>
# **AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated**
> AppEncryptionDeclarationDocumentResponse AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelated (string id, List<string> fieldsAppEncryptionDeclarationDocuments = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |

### Return type

[**AppEncryptionDeclarationDocumentResponse**](AppEncryptionDeclarationDocumentResponse.md)

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
| **200** | Single AppEncryptionDeclarationDocument |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationsappencryptiondeclarationdocumentgettoonerelationship"></a>
# **AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship**
> AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse AppEncryptionDeclarationsAppEncryptionDeclarationDocumentGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse**](AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse.md)

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

<a id="appencryptiondeclarationsappgettoonerelated"></a>
# **AppEncryptionDeclarationsAppGetToOneRelated**
> AppWithoutIncludesResponse AppEncryptionDeclarationsAppGetToOneRelated (string id, List<string> fieldsApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationsappgettoonerelationship"></a>
# **AppEncryptionDeclarationsAppGetToOneRelationship**
> AppEncryptionDeclarationAppLinkageResponse AppEncryptionDeclarationsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppEncryptionDeclarationAppLinkageResponse**](AppEncryptionDeclarationAppLinkageResponse.md)

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

<a id="appencryptiondeclarationsbuildscreatetomanyrelationship"></a>
# **AppEncryptionDeclarationsBuildsCreateToManyRelationship**
> void AppEncryptionDeclarationsBuildsCreateToManyRelationship (string id, AppEncryptionDeclarationBuildsLinkagesRequest appEncryptionDeclarationBuildsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEncryptionDeclarationBuildsLinkagesRequest** | [**AppEncryptionDeclarationBuildsLinkagesRequest**](AppEncryptionDeclarationBuildsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationscreateinstance"></a>
# **AppEncryptionDeclarationsCreateInstance**
> AppEncryptionDeclarationResponse AppEncryptionDeclarationsCreateInstance (AppEncryptionDeclarationCreateRequest appEncryptionDeclarationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEncryptionDeclarationCreateRequest** | [**AppEncryptionDeclarationCreateRequest**](AppEncryptionDeclarationCreateRequest.md) | AppEncryptionDeclaration representation |  |

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
| **201** | Single AppEncryptionDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationsgetcollection"></a>
# **AppEncryptionDeclarationsGetCollection**
> AppEncryptionDeclarationsResponse AppEncryptionDeclarationsGetCollection (List<string> filterPlatform = null, List<string> filterApp = null, List<string> filterBuilds = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsApps = null, List<string> fieldsAppEncryptionDeclarationDocuments = null, int limit = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**AppEncryptionDeclarationsResponse**](AppEncryptionDeclarationsResponse.md)

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
| **200** | List of AppEncryptionDeclarations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationsgetinstance"></a>
# **AppEncryptionDeclarationsGetInstance**
> AppEncryptionDeclarationResponse AppEncryptionDeclarationsGetInstance (string id, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsApps = null, List<string> fieldsAppEncryptionDeclarationDocuments = null, List<string> include = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAppEncryptionDeclarationDocuments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
| **200** | Single AppEncryptionDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

