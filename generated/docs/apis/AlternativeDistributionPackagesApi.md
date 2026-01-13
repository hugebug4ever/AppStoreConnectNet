# AppStoreConnect.Net.Api.AlternativeDistributionPackagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackagesCreateInstance**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagescreateinstance) | **POST** /v1/alternativeDistributionPackages |  |
| [**AlternativeDistributionPackagesGetInstance**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesgetinstance) | **GET** /v1/alternativeDistributionPackages/{id} |  |
| [**AlternativeDistributionPackagesVersionsGetToManyRelated**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesversionsgettomanyrelated) | **GET** /v1/alternativeDistributionPackages/{id}/versions |  |
| [**AlternativeDistributionPackagesVersionsGetToManyRelationship**](AlternativeDistributionPackagesApi.md#alternativedistributionpackagesversionsgettomanyrelationship) | **GET** /v1/alternativeDistributionPackages/{id}/relationships/versions |  |

<a id="alternativedistributionpackagescreateinstance"></a>
# **AlternativeDistributionPackagesCreateInstance**
> AlternativeDistributionPackageResponse AlternativeDistributionPackagesCreateInstance (AlternativeDistributionPackageCreateRequest alternativeDistributionPackageCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionPackageCreateRequest** | [**AlternativeDistributionPackageCreateRequest**](AlternativeDistributionPackageCreateRequest.md) | AlternativeDistributionPackage representation |  |

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

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
| **201** | Single AlternativeDistributionPackage |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackagesgetinstance"></a>
# **AlternativeDistributionPackagesGetInstance**
> AlternativeDistributionPackageResponse AlternativeDistributionPackagesGetInstance (string id, List<string> fieldsAlternativeDistributionPackages = null, List<string> fieldsAlternativeDistributionPackageVersions = null, List<string> include = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

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
| **200** | Single AlternativeDistributionPackage |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackagesversionsgettomanyrelated"></a>
# **AlternativeDistributionPackagesVersionsGetToManyRelated**
> AlternativeDistributionPackageVersionsResponse AlternativeDistributionPackagesVersionsGetToManyRelated (string id, List<string> filterState = null, List<string> fieldsAlternativeDistributionPackageVersions = null, List<string> fieldsAlternativeDistributionPackageVariants = null, List<string> fieldsAlternativeDistributionPackageDeltas = null, List<string> fieldsAlternativeDistributionPackages = null, int limit = null, List<string> include = null, int limitVariants = null, int limitDeltas = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVariants** | **int** | maximum number of related variants returned (when they are included) | [optional]  |
| **limitDeltas** | **int** | maximum number of related deltas returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionsResponse**](AlternativeDistributionPackageVersionsResponse.md)

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
| **200** | List of AlternativeDistributionPackageVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackagesversionsgettomanyrelationship"></a>
# **AlternativeDistributionPackagesVersionsGetToManyRelationship**
> AlternativeDistributionPackageVersionsLinkagesResponse AlternativeDistributionPackagesVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionsLinkagesResponse**](AlternativeDistributionPackageVersionsLinkagesResponse.md)

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

