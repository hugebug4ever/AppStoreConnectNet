# AppStoreConnect.Net.Api.AppEncryptionDeclarationDocumentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEncryptionDeclarationDocumentsCreateInstance**](AppEncryptionDeclarationDocumentsApi.md#appencryptiondeclarationdocumentscreateinstance) | **POST** /v1/appEncryptionDeclarationDocuments |  |
| [**AppEncryptionDeclarationDocumentsGetInstance**](AppEncryptionDeclarationDocumentsApi.md#appencryptiondeclarationdocumentsgetinstance) | **GET** /v1/appEncryptionDeclarationDocuments/{id} |  |
| [**AppEncryptionDeclarationDocumentsUpdateInstance**](AppEncryptionDeclarationDocumentsApi.md#appencryptiondeclarationdocumentsupdateinstance) | **PATCH** /v1/appEncryptionDeclarationDocuments/{id} |  |

<a id="appencryptiondeclarationdocumentscreateinstance"></a>
# **AppEncryptionDeclarationDocumentsCreateInstance**
> AppEncryptionDeclarationDocumentResponse AppEncryptionDeclarationDocumentsCreateInstance (AppEncryptionDeclarationDocumentCreateRequest appEncryptionDeclarationDocumentCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEncryptionDeclarationDocumentCreateRequest** | [**AppEncryptionDeclarationDocumentCreateRequest**](AppEncryptionDeclarationDocumentCreateRequest.md) | AppEncryptionDeclarationDocument representation |  |

### Return type

[**AppEncryptionDeclarationDocumentResponse**](AppEncryptionDeclarationDocumentResponse.md)

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
| **201** | Single AppEncryptionDeclarationDocument |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appencryptiondeclarationdocumentsgetinstance"></a>
# **AppEncryptionDeclarationDocumentsGetInstance**
> AppEncryptionDeclarationDocumentResponse AppEncryptionDeclarationDocumentsGetInstance (string id, List<string> fieldsAppEncryptionDeclarationDocuments = null)




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

<a id="appencryptiondeclarationdocumentsupdateinstance"></a>
# **AppEncryptionDeclarationDocumentsUpdateInstance**
> AppEncryptionDeclarationDocumentResponse AppEncryptionDeclarationDocumentsUpdateInstance (string id, AppEncryptionDeclarationDocumentUpdateRequest appEncryptionDeclarationDocumentUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEncryptionDeclarationDocumentUpdateRequest** | [**AppEncryptionDeclarationDocumentUpdateRequest**](AppEncryptionDeclarationDocumentUpdateRequest.md) | AppEncryptionDeclarationDocument representation |  |

### Return type

[**AppEncryptionDeclarationDocumentResponse**](AppEncryptionDeclarationDocumentResponse.md)

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
| **200** | Single AppEncryptionDeclarationDocument |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

