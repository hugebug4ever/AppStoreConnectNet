# AppStoreConnect.Net.Api.CertificatesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CertificatesCreateInstance**](CertificatesApi.md#certificatescreateinstance) | **POST** /v1/certificates |  |
| [**CertificatesDeleteInstance**](CertificatesApi.md#certificatesdeleteinstance) | **DELETE** /v1/certificates/{id} |  |
| [**CertificatesGetCollection**](CertificatesApi.md#certificatesgetcollection) | **GET** /v1/certificates |  |
| [**CertificatesGetInstance**](CertificatesApi.md#certificatesgetinstance) | **GET** /v1/certificates/{id} |  |
| [**CertificatesPassTypeIdGetToOneRelated**](CertificatesApi.md#certificatespasstypeidgettoonerelated) | **GET** /v1/certificates/{id}/passTypeId |  |
| [**CertificatesPassTypeIdGetToOneRelationship**](CertificatesApi.md#certificatespasstypeidgettoonerelationship) | **GET** /v1/certificates/{id}/relationships/passTypeId |  |
| [**CertificatesUpdateInstance**](CertificatesApi.md#certificatesupdateinstance) | **PATCH** /v1/certificates/{id} |  |

<a id="certificatescreateinstance"></a>
# **CertificatesCreateInstance**
> CertificateResponse CertificatesCreateInstance (CertificateCreateRequest certificateCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **certificateCreateRequest** | [**CertificateCreateRequest**](CertificateCreateRequest.md) | Certificate representation |  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **201** | Single Certificate |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="certificatesdeleteinstance"></a>
# **CertificatesDeleteInstance**
> void CertificatesDeleteInstance (string id)




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

<a id="certificatesgetcollection"></a>
# **CertificatesGetCollection**
> CertificatesResponse CertificatesGetCollection (List<string> filterDisplayName = null, List<string> filterCertificateType = null, List<string> filterSerialNumber = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsCertificates = null, List<string> fieldsPassTypeIds = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterDisplayName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;displayName&#39; | [optional]  |
| **filterCertificateType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;certificateType&#39; | [optional]  |
| **filterSerialNumber** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;serialNumber&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CertificatesResponse**](CertificatesResponse.md)

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
| **200** | List of Certificates |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="certificatesgetinstance"></a>
# **CertificatesGetInstance**
> CertificateResponse CertificatesGetInstance (string id, List<string> fieldsCertificates = null, List<string> fieldsPassTypeIds = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **200** | Single Certificate |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="certificatespasstypeidgettoonerelated"></a>
# **CertificatesPassTypeIdGetToOneRelated**
> PassTypeIdResponse CertificatesPassTypeIdGetToOneRelated (string id, List<string> fieldsPassTypeIds = null, List<string> fieldsCertificates = null, List<string> include = null, int limitCertificates = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **200** | Single PassTypeId |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="certificatespasstypeidgettoonerelationship"></a>
# **CertificatesPassTypeIdGetToOneRelationship**
> CertificatePassTypeIdLinkageResponse CertificatesPassTypeIdGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CertificatePassTypeIdLinkageResponse**](CertificatePassTypeIdLinkageResponse.md)

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

<a id="certificatesupdateinstance"></a>
# **CertificatesUpdateInstance**
> CertificateResponse CertificatesUpdateInstance (string id, CertificateUpdateRequest certificateUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **certificateUpdateRequest** | [**CertificateUpdateRequest**](CertificateUpdateRequest.md) | Certificate representation |  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **200** | Single Certificate |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

