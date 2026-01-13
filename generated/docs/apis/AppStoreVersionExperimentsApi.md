# AppStoreConnect.Net.Api.AppStoreVersionExperimentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelated) | **GET** /v1/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelationship) | **GET** /v1/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsCreateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentscreateinstance) | **POST** /v1/appStoreVersionExperiments |  |
| [**AppStoreVersionExperimentsDeleteInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsdeleteinstance) | **DELETE** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsGetInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsgetinstance) | **GET** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsUpdateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsupdateinstance) | **PATCH** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelated) | **GET** /v2/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelationship) | **GET** /v2/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsV2CreateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2createinstance) | **POST** /v2/appStoreVersionExperiments |  |
| [**AppStoreVersionExperimentsV2DeleteInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2deleteinstance) | **DELETE** /v2/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2GetInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2getinstance) | **GET** /v2/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2UpdateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2updateinstance) | **PATCH** /v2/appStoreVersionExperiments/{id} |  |

<a id="appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelated"></a>
# **AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated**
> AppStoreVersionExperimentTreatmentsResponse AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated (string id, List<string> fieldsAppStoreVersionExperimentTreatments = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, int limit = null, List<string> include = null, int limitAppStoreVersionExperimentTreatmentLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatmentLocalizations** | **int** | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
| **200** | List of AppStoreVersionExperimentTreatments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelationship"></a>
# **AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship**
> AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

<a id="appstoreversionexperimentscreateinstance"></a>
# **AppStoreVersionExperimentsCreateInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsCreateInstance (AppStoreVersionExperimentCreateRequest appStoreVersionExperimentCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentCreateRequest** | [**AppStoreVersionExperimentCreateRequest**](AppStoreVersionExperimentCreateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **201** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsdeleteinstance"></a>
# **AppStoreVersionExperimentsDeleteInstance**
> void AppStoreVersionExperimentsDeleteInstance (string id)




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

<a id="appstoreversionexperimentsgetinstance"></a>
# **AppStoreVersionExperimentsGetInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsGetInstance (string id, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAppStoreVersionExperimentTreatments = null, List<string> include = null, int limitAppStoreVersionExperimentTreatments = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatments** | **int** | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsupdateinstance"></a>
# **AppStoreVersionExperimentsUpdateInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsUpdateInstance (string id, AppStoreVersionExperimentUpdateRequest appStoreVersionExperimentUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionExperimentUpdateRequest** | [**AppStoreVersionExperimentUpdateRequest**](AppStoreVersionExperimentUpdateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelated"></a>
# **AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated**
> AppStoreVersionExperimentTreatmentsResponse AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated (string id, List<string> fieldsAppStoreVersionExperimentTreatments = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, int limit = null, List<string> include = null, int limitAppStoreVersionExperimentTreatmentLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatmentLocalizations** | **int** | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
| **200** | List of AppStoreVersionExperimentTreatments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelationship"></a>
# **AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship**
> AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

<a id="appstoreversionexperimentsv2createinstance"></a>
# **AppStoreVersionExperimentsV2CreateInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2CreateInstance (AppStoreVersionExperimentV2CreateRequest appStoreVersionExperimentV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentV2CreateRequest** | [**AppStoreVersionExperimentV2CreateRequest**](AppStoreVersionExperimentV2CreateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **201** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsv2deleteinstance"></a>
# **AppStoreVersionExperimentsV2DeleteInstance**
> void AppStoreVersionExperimentsV2DeleteInstance (string id)




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

<a id="appstoreversionexperimentsv2getinstance"></a>
# **AppStoreVersionExperimentsV2GetInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2GetInstance (string id, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAppStoreVersionExperimentTreatments = null, List<string> include = null, int limitAppStoreVersionExperimentTreatments = null, int limitControlVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatments** | **int** | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional]  |
| **limitControlVersions** | **int** | maximum number of related controlVersions returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimentsv2updateinstance"></a>
# **AppStoreVersionExperimentsV2UpdateInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2UpdateInstance (string id, AppStoreVersionExperimentV2UpdateRequest appStoreVersionExperimentV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionExperimentV2UpdateRequest** | [**AppStoreVersionExperimentV2UpdateRequest**](AppStoreVersionExperimentV2UpdateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

