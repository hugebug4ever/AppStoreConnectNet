# AppStoreConnect.Net.Api.CiMacOsVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiMacOsVersionsGetCollection**](CiMacOsVersionsApi.md#cimacosversionsgetcollection) | **GET** /v1/ciMacOsVersions |  |
| [**CiMacOsVersionsGetInstance**](CiMacOsVersionsApi.md#cimacosversionsgetinstance) | **GET** /v1/ciMacOsVersions/{id} |  |
| [**CiMacOsVersionsXcodeVersionsGetToManyRelated**](CiMacOsVersionsApi.md#cimacosversionsxcodeversionsgettomanyrelated) | **GET** /v1/ciMacOsVersions/{id}/xcodeVersions |  |
| [**CiMacOsVersionsXcodeVersionsGetToManyRelationship**](CiMacOsVersionsApi.md#cimacosversionsxcodeversionsgettomanyrelationship) | **GET** /v1/ciMacOsVersions/{id}/relationships/xcodeVersions |  |

<a id="cimacosversionsgetcollection"></a>
# **CiMacOsVersionsGetCollection**
> CiMacOsVersionsResponse CiMacOsVersionsGetCollection (List<string> fieldsCiMacOsVersions = null, List<string> fieldsCiXcodeVersions = null, int limit = null, List<string> include = null, int limitXcodeVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
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
| **200** | List of CiMacOsVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cimacosversionsgetinstance"></a>
# **CiMacOsVersionsGetInstance**
> CiMacOsVersionResponse CiMacOsVersionsGetInstance (string id, List<string> fieldsCiMacOsVersions = null, List<string> fieldsCiXcodeVersions = null, List<string> include = null, int limitXcodeVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiMacOsVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciMacOsVersions | [optional]  |
| **fieldsCiXcodeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciXcodeVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitXcodeVersions** | **int** | maximum number of related xcodeVersions returned (when they are included) | [optional]  |

### Return type

[**CiMacOsVersionResponse**](CiMacOsVersionResponse.md)

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
| **200** | Single CiMacOsVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cimacosversionsxcodeversionsgettomanyrelated"></a>
# **CiMacOsVersionsXcodeVersionsGetToManyRelated**
> CiXcodeVersionsResponse CiMacOsVersionsXcodeVersionsGetToManyRelated (string id, List<string> fieldsCiXcodeVersions = null, List<string> fieldsCiMacOsVersions = null, int limit = null, List<string> include = null, int limitMacOsVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
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
| **404** | Not found error |  -  |
| **200** | List of CiXcodeVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="cimacosversionsxcodeversionsgettomanyrelationship"></a>
# **CiMacOsVersionsXcodeVersionsGetToManyRelationship**
> CiMacOsVersionXcodeVersionsLinkagesResponse CiMacOsVersionsXcodeVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CiMacOsVersionXcodeVersionsLinkagesResponse**](CiMacOsVersionXcodeVersionsLinkagesResponse.md)

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

