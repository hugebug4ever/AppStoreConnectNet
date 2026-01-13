# AppStoreConnect.Net.Api.PassTypeIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**PassTypeIdsCertificatesGetToManyRelated**](PassTypeIdsApi.md#passtypeidscertificatesgettomanyrelated) | **GET** /v1/passTypeIds/{id}/certificates |  |
| [**PassTypeIdsCertificatesGetToManyRelationship**](PassTypeIdsApi.md#passtypeidscertificatesgettomanyrelationship) | **GET** /v1/passTypeIds/{id}/relationships/certificates |  |
| [**PassTypeIdsCreateInstance**](PassTypeIdsApi.md#passtypeidscreateinstance) | **POST** /v1/passTypeIds |  |
| [**PassTypeIdsDeleteInstance**](PassTypeIdsApi.md#passtypeidsdeleteinstance) | **DELETE** /v1/passTypeIds/{id} |  |
| [**PassTypeIdsGetCollection**](PassTypeIdsApi.md#passtypeidsgetcollection) | **GET** /v1/passTypeIds |  |
| [**PassTypeIdsGetInstance**](PassTypeIdsApi.md#passtypeidsgetinstance) | **GET** /v1/passTypeIds/{id} |  |
| [**PassTypeIdsUpdateInstance**](PassTypeIdsApi.md#passtypeidsupdateinstance) | **PATCH** /v1/passTypeIds/{id} |  |

<a id="passtypeidscertificatesgettomanyrelated"></a>
# **PassTypeIdsCertificatesGetToManyRelated**
> CertificatesResponse PassTypeIdsCertificatesGetToManyRelated (string id, List<string> filterDisplayName = null, List<string> filterCertificateType = null, List<string> filterSerialNumber = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsCertificates = null, List<string> fieldsPassTypeIds = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
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
| **404** | Not found error |  -  |
| **200** | List of Certificates |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="passtypeidscertificatesgettomanyrelationship"></a>
# **PassTypeIdsCertificatesGetToManyRelationship**
> PassTypeIdCertificatesLinkagesResponse PassTypeIdsCertificatesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**PassTypeIdCertificatesLinkagesResponse**](PassTypeIdCertificatesLinkagesResponse.md)

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

<a id="passtypeidscreateinstance"></a>
# **PassTypeIdsCreateInstance**
> PassTypeIdResponse PassTypeIdsCreateInstance (PassTypeIdCreateRequest passTypeIdCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **passTypeIdCreateRequest** | [**PassTypeIdCreateRequest**](PassTypeIdCreateRequest.md) | PassTypeId representation |  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **201** | Single PassTypeId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="passtypeidsdeleteinstance"></a>
# **PassTypeIdsDeleteInstance**
> void PassTypeIdsDeleteInstance (string id)




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

<a id="passtypeidsgetcollection"></a>
# **PassTypeIdsGetCollection**
> PassTypeIdsResponse PassTypeIdsGetCollection (List<string> filterName = null, List<string> filterIdentifier = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsPassTypeIds = null, List<string> fieldsCertificates = null, int limit = null, List<string> include = null, int limitCertificates = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIdentifier** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;identifier&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**PassTypeIdsResponse**](PassTypeIdsResponse.md)

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
| **200** | List of PassTypeIds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="passtypeidsgetinstance"></a>
# **PassTypeIdsGetInstance**
> PassTypeIdResponse PassTypeIdsGetInstance (string id, List<string> fieldsPassTypeIds = null, List<string> fieldsCertificates = null, List<string> include = null, int limitCertificates = null)




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

<a id="passtypeidsupdateinstance"></a>
# **PassTypeIdsUpdateInstance**
> PassTypeIdResponse PassTypeIdsUpdateInstance (string id, PassTypeIdUpdateRequest passTypeIdUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **passTypeIdUpdateRequest** | [**PassTypeIdUpdateRequest**](PassTypeIdUpdateRequest.md) | PassTypeId representation |  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **200** | Single PassTypeId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

