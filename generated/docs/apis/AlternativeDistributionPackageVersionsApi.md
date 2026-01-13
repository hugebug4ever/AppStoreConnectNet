# AppStoreConnect.Net.Api.AlternativeDistributionPackageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackageVersionsDeltasGetToManyRelated**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsdeltasgettomanyrelated) | **GET** /v1/alternativeDistributionPackageVersions/{id}/deltas |  |
| [**AlternativeDistributionPackageVersionsDeltasGetToManyRelationship**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsdeltasgettomanyrelationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/deltas |  |
| [**AlternativeDistributionPackageVersionsGetInstance**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsgetinstance) | **GET** /v1/alternativeDistributionPackageVersions/{id} |  |
| [**AlternativeDistributionPackageVersionsVariantsGetToManyRelated**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsvariantsgettomanyrelated) | **GET** /v1/alternativeDistributionPackageVersions/{id}/variants |  |
| [**AlternativeDistributionPackageVersionsVariantsGetToManyRelationship**](AlternativeDistributionPackageVersionsApi.md#alternativedistributionpackageversionsvariantsgettomanyrelationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/variants |  |

<a id="alternativedistributionpackageversionsdeltasgettomanyrelated"></a>
# **AlternativeDistributionPackageVersionsDeltasGetToManyRelated**
> AlternativeDistributionPackageDeltasResponse AlternativeDistributionPackageVersionsDeltasGetToManyRelated (string id, List<string> fieldsAlternativeDistributionPackageDeltas = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageDeltasResponse**](AlternativeDistributionPackageDeltasResponse.md)

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
| **200** | List of AlternativeDistributionPackageDeltas |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackageversionsdeltasgettomanyrelationship"></a>
# **AlternativeDistributionPackageVersionsDeltasGetToManyRelationship**
> AlternativeDistributionPackageVersionDeltasLinkagesResponse AlternativeDistributionPackageVersionsDeltasGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionDeltasLinkagesResponse**](AlternativeDistributionPackageVersionDeltasLinkagesResponse.md)

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

<a id="alternativedistributionpackageversionsgetinstance"></a>
# **AlternativeDistributionPackageVersionsGetInstance**
> AlternativeDistributionPackageVersionResponse AlternativeDistributionPackageVersionsGetInstance (string id, List<string> fieldsAlternativeDistributionPackageVersions = null, List<string> fieldsAlternativeDistributionPackageVariants = null, List<string> fieldsAlternativeDistributionPackageDeltas = null, List<string> include = null, int limitDeltas = null, int limitVariants = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional]  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitDeltas** | **int** | maximum number of related deltas returned (when they are included) | [optional]  |
| **limitVariants** | **int** | maximum number of related variants returned (when they are included) | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionResponse**](AlternativeDistributionPackageVersionResponse.md)

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
| **200** | Single AlternativeDistributionPackageVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackageversionsvariantsgettomanyrelated"></a>
# **AlternativeDistributionPackageVersionsVariantsGetToManyRelated**
> AlternativeDistributionPackageVariantsResponse AlternativeDistributionPackageVersionsVariantsGetToManyRelated (string id, List<string> fieldsAlternativeDistributionPackageVariants = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageVariantsResponse**](AlternativeDistributionPackageVariantsResponse.md)

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
| **200** | List of AlternativeDistributionPackageVariants |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributionpackageversionsvariantsgettomanyrelationship"></a>
# **AlternativeDistributionPackageVersionsVariantsGetToManyRelationship**
> AlternativeDistributionPackageVersionVariantsLinkagesResponse AlternativeDistributionPackageVersionsVariantsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionPackageVersionVariantsLinkagesResponse**](AlternativeDistributionPackageVersionVariantsLinkagesResponse.md)

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

