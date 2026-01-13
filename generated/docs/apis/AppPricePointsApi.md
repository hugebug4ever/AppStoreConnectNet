# AppStoreConnect.Net.Api.AppPricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppPricePointsV3EqualizationsGetToManyRelated**](AppPricePointsApi.md#apppricepointsv3equalizationsgettomanyrelated) | **GET** /v3/appPricePoints/{id}/equalizations |  |
| [**AppPricePointsV3EqualizationsGetToManyRelationship**](AppPricePointsApi.md#apppricepointsv3equalizationsgettomanyrelationship) | **GET** /v3/appPricePoints/{id}/relationships/equalizations |  |
| [**AppPricePointsV3GetInstance**](AppPricePointsApi.md#apppricepointsv3getinstance) | **GET** /v3/appPricePoints/{id} |  |

<a id="apppricepointsv3equalizationsgettomanyrelated"></a>
# **AppPricePointsV3EqualizationsGetToManyRelated**
> AppPricePointsV3Response AppPricePointsV3EqualizationsGetToManyRelated (string id, List<string> filterTerritory = null, List<string> fieldsAppPricePoints = null, List<string> fieldsApps = null, List<string> fieldsTerritories = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricePointsV3Response**](AppPricePointsV3Response.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of AppPricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="apppricepointsv3equalizationsgettomanyrelationship"></a>
# **AppPricePointsV3EqualizationsGetToManyRelationship**
> AppPricePointV3EqualizationsLinkagesResponse AppPricePointsV3EqualizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppPricePointV3EqualizationsLinkagesResponse**](AppPricePointV3EqualizationsLinkagesResponse.md)

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

<a id="apppricepointsv3getinstance"></a>
# **AppPricePointsV3GetInstance**
> AppPricePointV3Response AppPricePointsV3GetInstance (string id, List<string> fieldsAppPricePoints = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricePointV3Response**](AppPricePointV3Response.md)

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
| **200** | Single AppPricePoint |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

