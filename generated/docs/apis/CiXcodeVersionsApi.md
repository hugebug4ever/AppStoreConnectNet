# AppStoreConnect.Net.Api.CiXcodeVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiXcodeVersionsGetCollection**](CiXcodeVersionsApi.md#cixcodeversionsgetcollection) | **GET** /v1/ciXcodeVersions |  |
| [**CiXcodeVersionsGetInstance**](CiXcodeVersionsApi.md#cixcodeversionsgetinstance) | **GET** /v1/ciXcodeVersions/{id} |  |
| [**CiXcodeVersionsMacOsVersionsGetToManyRelated**](CiXcodeVersionsApi.md#cixcodeversionsmacosversionsgettomanyrelated) | **GET** /v1/ciXcodeVersions/{id}/macOsVersions |  |
| [**CiXcodeVersionsMacOsVersionsGetToManyRelationship**](CiXcodeVersionsApi.md#cixcodeversionsmacosversionsgettomanyrelationship) | **GET** /v1/ciXcodeVersions/{id}/relationships/macOsVersions |  |

<a id="cixcodeversionsgetcollection"></a>
# **CiXcodeVersionsGetCollection**
> CiXcodeVersionsResponse CiXcodeVersionsGetCollection (List<string> fieldsCiXcodeVersions = null, List<string> fieldsCiMacOsVersions = null, int limit = null, List<string> include = null, int limitMacOsVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMacOsVersions** | **int** | maximum number of related macOsVersions returned (when they are included) | [optional]  |

### Return type

[**CiXcodeVersionsResponse**](CiXcodeVersionsResponse.md)

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
| **200** | List of CiXcodeVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cixcodeversionsgetinstance"></a>
# **CiXcodeVersionsGetInstance**
> CiXcodeVersionResponse CiXcodeVersionsGetInstance (string id, List<string> fieldsCiXcodeVersions = null, List<string> fieldsCiMacOsVersions = null, List<string> include = null, int limitMacOsVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMacOsVersions** | **int** | maximum number of related macOsVersions returned (when they are included) | [optional]  |

### Return type

[**CiXcodeVersionResponse**](CiXcodeVersionResponse.md)

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
| **200** | Single CiXcodeVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cixcodeversionsmacosversionsgettomanyrelated"></a>
# **CiXcodeVersionsMacOsVersionsGetToManyRelated**
> CiMacOsVersionsResponse CiXcodeVersionsMacOsVersionsGetToManyRelated (string id, List<string> fieldsCiMacOsVersions = null, List<string> fieldsCiXcodeVersions = null, int limit = null, List<string> include = null, int limitXcodeVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitXcodeVersions** | **int** | maximum number of related xcodeVersions returned (when they are included) | [optional]  |

### Return type

[**CiMacOsVersionsResponse**](CiMacOsVersionsResponse.md)

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
| **200** | List of CiMacOsVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cixcodeversionsmacosversionsgettomanyrelationship"></a>
# **CiXcodeVersionsMacOsVersionsGetToManyRelationship**
> CiXcodeVersionMacOsVersionsLinkagesResponse CiXcodeVersionsMacOsVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiXcodeVersionMacOsVersionsLinkagesResponse**](CiXcodeVersionMacOsVersionsLinkagesResponse.md)

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

