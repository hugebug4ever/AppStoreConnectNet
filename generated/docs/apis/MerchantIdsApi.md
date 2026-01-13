# AppStoreConnect.Net.Api.MerchantIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MerchantIdsCertificatesGetToManyRelated**](MerchantIdsApi.md#merchantidscertificatesgettomanyrelated) | **GET** /v1/merchantIds/{id}/certificates |  |
| [**MerchantIdsCertificatesGetToManyRelationship**](MerchantIdsApi.md#merchantidscertificatesgettomanyrelationship) | **GET** /v1/merchantIds/{id}/relationships/certificates |  |
| [**MerchantIdsCreateInstance**](MerchantIdsApi.md#merchantidscreateinstance) | **POST** /v1/merchantIds |  |
| [**MerchantIdsDeleteInstance**](MerchantIdsApi.md#merchantidsdeleteinstance) | **DELETE** /v1/merchantIds/{id} |  |
| [**MerchantIdsGetCollection**](MerchantIdsApi.md#merchantidsgetcollection) | **GET** /v1/merchantIds |  |
| [**MerchantIdsGetInstance**](MerchantIdsApi.md#merchantidsgetinstance) | **GET** /v1/merchantIds/{id} |  |
| [**MerchantIdsUpdateInstance**](MerchantIdsApi.md#merchantidsupdateinstance) | **PATCH** /v1/merchantIds/{id} |  |

<a id="merchantidscertificatesgettomanyrelated"></a>
# **MerchantIdsCertificatesGetToManyRelated**
> CertificatesResponse MerchantIdsCertificatesGetToManyRelated (string id, List<string> filterDisplayName = null, List<string> filterCertificateType = null, List<string> filterSerialNumber = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsCertificates = null, List<string> fieldsPassTypeIds = null, int limit = null, List<string> include = null)




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

<a id="merchantidscertificatesgettomanyrelationship"></a>
# **MerchantIdsCertificatesGetToManyRelationship**
> MerchantIdCertificatesLinkagesResponse MerchantIdsCertificatesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**MerchantIdCertificatesLinkagesResponse**](MerchantIdCertificatesLinkagesResponse.md)

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

<a id="merchantidscreateinstance"></a>
# **MerchantIdsCreateInstance**
> MerchantIdResponse MerchantIdsCreateInstance (MerchantIdCreateRequest merchantIdCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **merchantIdCreateRequest** | [**MerchantIdCreateRequest**](MerchantIdCreateRequest.md) | MerchantId representation |  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **201** | Single MerchantId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="merchantidsdeleteinstance"></a>
# **MerchantIdsDeleteInstance**
> void MerchantIdsDeleteInstance (string id)




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

<a id="merchantidsgetcollection"></a>
# **MerchantIdsGetCollection**
> MerchantIdsResponse MerchantIdsGetCollection (List<string> filterName = null, List<string> filterIdentifier = null, List<string> sort = null, List<string> fieldsMerchantIds = null, List<string> fieldsCertificates = null, int limit = null, List<string> include = null, int limitCertificates = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIdentifier** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;identifier&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsMerchantIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type merchantIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**MerchantIdsResponse**](MerchantIdsResponse.md)

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
| **200** | List of MerchantIds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="merchantidsgetinstance"></a>
# **MerchantIdsGetInstance**
> MerchantIdResponse MerchantIdsGetInstance (string id, List<string> fieldsMerchantIds = null, List<string> fieldsCertificates = null, List<string> include = null, int limitCertificates = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsMerchantIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type merchantIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **200** | Single MerchantId |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="merchantidsupdateinstance"></a>
# **MerchantIdsUpdateInstance**
> MerchantIdResponse MerchantIdsUpdateInstance (string id, MerchantIdUpdateRequest merchantIdUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **merchantIdUpdateRequest** | [**MerchantIdUpdateRequest**](MerchantIdUpdateRequest.md) | MerchantId representation |  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **200** | Single MerchantId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

