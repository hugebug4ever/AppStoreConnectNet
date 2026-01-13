# AppStoreConnect.Net.Api.AlternativeDistributionDomainsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionDomainsCreateInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainscreateinstance) | **POST** /v1/alternativeDistributionDomains |  |
| [**AlternativeDistributionDomainsDeleteInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsdeleteinstance) | **DELETE** /v1/alternativeDistributionDomains/{id} |  |
| [**AlternativeDistributionDomainsGetCollection**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsgetcollection) | **GET** /v1/alternativeDistributionDomains |  |
| [**AlternativeDistributionDomainsGetInstance**](AlternativeDistributionDomainsApi.md#alternativedistributiondomainsgetinstance) | **GET** /v1/alternativeDistributionDomains/{id} |  |

<a id="alternativedistributiondomainscreateinstance"></a>
# **AlternativeDistributionDomainsCreateInstance**
> AlternativeDistributionDomainResponse AlternativeDistributionDomainsCreateInstance (AlternativeDistributionDomainCreateRequest alternativeDistributionDomainCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **alternativeDistributionDomainCreateRequest** | [**AlternativeDistributionDomainCreateRequest**](AlternativeDistributionDomainCreateRequest.md) | AlternativeDistributionDomain representation |  |

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
| **201** | Single AlternativeDistributionDomain |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributiondomainsdeleteinstance"></a>
# **AlternativeDistributionDomainsDeleteInstance**
> void AlternativeDistributionDomainsDeleteInstance (string id)




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

<a id="alternativedistributiondomainsgetcollection"></a>
# **AlternativeDistributionDomainsGetCollection**
> AlternativeDistributionDomainsResponse AlternativeDistributionDomainsGetCollection (List<string> fieldsAlternativeDistributionDomains = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsAlternativeDistributionDomains** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionDomains | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AlternativeDistributionDomainsResponse**](AlternativeDistributionDomainsResponse.md)

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
| **200** | List of AlternativeDistributionDomains |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="alternativedistributiondomainsgetinstance"></a>
# **AlternativeDistributionDomainsGetInstance**
> AlternativeDistributionDomainResponse AlternativeDistributionDomainsGetInstance (string id, List<string> fieldsAlternativeDistributionDomains = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionDomains** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionDomains | [optional]  |

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
| **200** | Single AlternativeDistributionDomain |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

