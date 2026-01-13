# AppStoreConnect.Net.Api.NominationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**NominationsCreateInstance**](NominationsApi.md#nominationscreateinstance) | **POST** /v1/nominations |  |
| [**NominationsDeleteInstance**](NominationsApi.md#nominationsdeleteinstance) | **DELETE** /v1/nominations/{id} |  |
| [**NominationsGetCollection**](NominationsApi.md#nominationsgetcollection) | **GET** /v1/nominations |  |
| [**NominationsGetInstance**](NominationsApi.md#nominationsgetinstance) | **GET** /v1/nominations/{id} |  |
| [**NominationsUpdateInstance**](NominationsApi.md#nominationsupdateinstance) | **PATCH** /v1/nominations/{id} |  |

<a id="nominationscreateinstance"></a>
# **NominationsCreateInstance**
> NominationResponse NominationsCreateInstance (NominationCreateRequest nominationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **nominationCreateRequest** | [**NominationCreateRequest**](NominationCreateRequest.md) | Nomination representation |  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **201** | Single Nomination |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="nominationsdeleteinstance"></a>
# **NominationsDeleteInstance**
> void NominationsDeleteInstance (string id)




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

<a id="nominationsgetcollection"></a>
# **NominationsGetCollection**
> NominationsResponse NominationsGetCollection (List<string> filterState, List<string> filterType = null, List<string> filterRelatedApps = null, List<string> sort = null, List<string> fieldsNominations = null, int limit = null, List<string> include = null, int limitInAppEvents = null, int limitRelatedApps = null, int limitSupportedTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; |  |
| **filterType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;type&#39; | [optional]  |
| **filterRelatedApps** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;relatedApps&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsNominations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type nominations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitInAppEvents** | **int** | maximum number of related inAppEvents returned (when they are included) | [optional]  |
| **limitRelatedApps** | **int** | maximum number of related relatedApps returned (when they are included) | [optional]  |
| **limitSupportedTerritories** | **int** | maximum number of related supportedTerritories returned (when they are included) | [optional]  |

### Return type

[**NominationsResponse**](NominationsResponse.md)

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
| **200** | List of Nominations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="nominationsgetinstance"></a>
# **NominationsGetInstance**
> NominationResponse NominationsGetInstance (string id, List<string> fieldsNominations = null, List<string> include = null, int limitInAppEvents = null, int limitRelatedApps = null, int limitSupportedTerritories = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsNominations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type nominations | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitInAppEvents** | **int** | maximum number of related inAppEvents returned (when they are included) | [optional]  |
| **limitRelatedApps** | **int** | maximum number of related relatedApps returned (when they are included) | [optional]  |
| **limitSupportedTerritories** | **int** | maximum number of related supportedTerritories returned (when they are included) | [optional]  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **200** | Single Nomination |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="nominationsupdateinstance"></a>
# **NominationsUpdateInstance**
> NominationResponse NominationsUpdateInstance (string id, NominationUpdateRequest nominationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **nominationUpdateRequest** | [**NominationUpdateRequest**](NominationUpdateRequest.md) | Nomination representation |  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **200** | Single Nomination |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

