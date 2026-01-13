# AppStoreConnect.Net.Api.ProfilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ProfilesBundleIdGetToOneRelated**](ProfilesApi.md#profilesbundleidgettoonerelated) | **GET** /v1/profiles/{id}/bundleId |  |
| [**ProfilesBundleIdGetToOneRelationship**](ProfilesApi.md#profilesbundleidgettoonerelationship) | **GET** /v1/profiles/{id}/relationships/bundleId |  |
| [**ProfilesCertificatesGetToManyRelated**](ProfilesApi.md#profilescertificatesgettomanyrelated) | **GET** /v1/profiles/{id}/certificates |  |
| [**ProfilesCertificatesGetToManyRelationship**](ProfilesApi.md#profilescertificatesgettomanyrelationship) | **GET** /v1/profiles/{id}/relationships/certificates |  |
| [**ProfilesCreateInstance**](ProfilesApi.md#profilescreateinstance) | **POST** /v1/profiles |  |
| [**ProfilesDeleteInstance**](ProfilesApi.md#profilesdeleteinstance) | **DELETE** /v1/profiles/{id} |  |
| [**ProfilesDevicesGetToManyRelated**](ProfilesApi.md#profilesdevicesgettomanyrelated) | **GET** /v1/profiles/{id}/devices |  |
| [**ProfilesDevicesGetToManyRelationship**](ProfilesApi.md#profilesdevicesgettomanyrelationship) | **GET** /v1/profiles/{id}/relationships/devices |  |
| [**ProfilesGetCollection**](ProfilesApi.md#profilesgetcollection) | **GET** /v1/profiles |  |
| [**ProfilesGetInstance**](ProfilesApi.md#profilesgetinstance) | **GET** /v1/profiles/{id} |  |

<a id="profilesbundleidgettoonerelated"></a>
# **ProfilesBundleIdGetToOneRelated**
> BundleIdWithoutIncludesResponse ProfilesBundleIdGetToOneRelated (string id, List<string> fieldsBundleIds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBundleIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIds | [optional]  |

### Return type

[**BundleIdWithoutIncludesResponse**](BundleIdWithoutIncludesResponse.md)

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
| **200** | Single BundleId with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="profilesbundleidgettoonerelationship"></a>
# **ProfilesBundleIdGetToOneRelationship**
> ProfileBundleIdLinkageResponse ProfilesBundleIdGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**ProfileBundleIdLinkageResponse**](ProfileBundleIdLinkageResponse.md)

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

<a id="profilescertificatesgettomanyrelated"></a>
# **ProfilesCertificatesGetToManyRelated**
> CertificatesWithoutIncludesResponse ProfilesCertificatesGetToManyRelated (string id, List<string> fieldsCertificates = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**CertificatesWithoutIncludesResponse**](CertificatesWithoutIncludesResponse.md)

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
| **200** | List of Certificates with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="profilescertificatesgettomanyrelationship"></a>
# **ProfilesCertificatesGetToManyRelationship**
> ProfileCertificatesLinkagesResponse ProfilesCertificatesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ProfileCertificatesLinkagesResponse**](ProfileCertificatesLinkagesResponse.md)

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

<a id="profilescreateinstance"></a>
# **ProfilesCreateInstance**
> ProfileResponse ProfilesCreateInstance (ProfileCreateRequest profileCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **profileCreateRequest** | [**ProfileCreateRequest**](ProfileCreateRequest.md) | Profile representation |  |

### Return type

[**ProfileResponse**](ProfileResponse.md)

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
| **201** | Single Profile |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="profilesdeleteinstance"></a>
# **ProfilesDeleteInstance**
> void ProfilesDeleteInstance (string id)




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

<a id="profilesdevicesgettomanyrelated"></a>
# **ProfilesDevicesGetToManyRelated**
> DevicesWithoutIncludesResponse ProfilesDevicesGetToManyRelated (string id, List<string> fieldsDevices = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsDevices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type devices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**DevicesWithoutIncludesResponse**](DevicesWithoutIncludesResponse.md)

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
| **200** | List of Devices with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="profilesdevicesgettomanyrelationship"></a>
# **ProfilesDevicesGetToManyRelationship**
> ProfileDevicesLinkagesResponse ProfilesDevicesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ProfileDevicesLinkagesResponse**](ProfileDevicesLinkagesResponse.md)

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

<a id="profilesgetcollection"></a>
# **ProfilesGetCollection**
> ProfilesResponse ProfilesGetCollection (List<string> filterName = null, List<string> filterProfileType = null, List<string> filterProfileState = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsProfiles = null, List<string> fieldsBundleIds = null, List<string> fieldsDevices = null, List<string> fieldsCertificates = null, int limit = null, List<string> include = null, int limitCertificates = null, int limitDevices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterProfileType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;profileType&#39; | [optional]  |
| **filterProfileState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;profileState&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsProfiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type profiles | [optional]  |
| **fieldsBundleIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIds | [optional]  |
| **fieldsDevices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type devices | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |
| **limitDevices** | **int** | maximum number of related devices returned (when they are included) | [optional]  |

### Return type

[**ProfilesResponse**](ProfilesResponse.md)

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
| **200** | List of Profiles |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="profilesgetinstance"></a>
# **ProfilesGetInstance**
> ProfileResponse ProfilesGetInstance (string id, List<string> fieldsProfiles = null, List<string> fieldsBundleIds = null, List<string> fieldsDevices = null, List<string> fieldsCertificates = null, List<string> include = null, int limitCertificates = null, int limitDevices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsProfiles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type profiles | [optional]  |
| **fieldsBundleIds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type bundleIds | [optional]  |
| **fieldsDevices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type devices | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int** | maximum number of related certificates returned (when they are included) | [optional]  |
| **limitDevices** | **int** | maximum number of related devices returned (when they are included) | [optional]  |

### Return type

[**ProfileResponse**](ProfileResponse.md)

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
| **200** | Single Profile |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

