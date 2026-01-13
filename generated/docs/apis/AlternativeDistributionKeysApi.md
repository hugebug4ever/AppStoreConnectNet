# AppStoreConnect.Net.Api.AlternativeDistributionKeysApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionKeysCreateInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeyscreateinstance) | **POST** /v1/alternativeDistributionKeys |  |
| [**AlternativeDistributionKeysDeleteInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeysdeleteinstance) | **DELETE** /v1/alternativeDistributionKeys/{id} |  |
| [**AlternativeDistributionKeysGetCollection**](AlternativeDistributionKeysApi.md#alternativedistributionkeysgetcollection) | **GET** /v1/alternativeDistributionKeys |  |
| [**AlternativeDistributionKeysGetInstance**](AlternativeDistributionKeysApi.md#alternativedistributionkeysgetinstance) | **GET** /v1/alternativeDistributionKeys/{id} |  |

<a id="alternativedistributionkeyscreateinstance"></a>
# **AlternativeDistributionKeysCreateInstance**
> AlternativeDistributionKeyResponse AlternativeDistributionKeysCreateInstance (AlternativeDistributionKeyCreateRequest alternativeDistributionKeyCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionKeyCreateRequest** | [**AlternativeDistributionKeyCreateRequest**](AlternativeDistributionKeyCreateRequest.md) | AlternativeDistributionKey representation |  |

### Return type

[**AlternativeDistributionKeyResponse**](AlternativeDistributionKeyResponse.md)

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
| **201** | Single AlternativeDistributionKey |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionkeysdeleteinstance"></a>
# **AlternativeDistributionKeysDeleteInstance**
> void AlternativeDistributionKeysDeleteInstance (string id)




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

<a id="alternativedistributionkeysgetcollection"></a>
# **AlternativeDistributionKeysGetCollection**
> AlternativeDistributionKeysResponse AlternativeDistributionKeysGetCollection (bool existsApp = null, List<string> fieldsAlternativeDistributionKeys = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **existsApp** | **bool** | filter by existence or non-existence of related &#39;app&#39; | [optional]  |
| **fieldsAlternativeDistributionKeys** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionKeys | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionKeysResponse**](AlternativeDistributionKeysResponse.md)

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
| **200** | List of AlternativeDistributionKeys |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionkeysgetinstance"></a>
# **AlternativeDistributionKeysGetInstance**
> AlternativeDistributionKeyResponse AlternativeDistributionKeysGetInstance (string id, List<string> fieldsAlternativeDistributionKeys = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionKeys** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionKeys | [optional]  |

### Return type

[**AlternativeDistributionKeyResponse**](AlternativeDistributionKeyResponse.md)

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
| **200** | Single AlternativeDistributionKey |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

