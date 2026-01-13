# AppStoreConnect.Net.Api.AppEventLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppEventLocalizationsAppEventScreenshotsGetToManyRelated**](AppEventLocalizationsApi.md#appeventlocalizationsappeventscreenshotsgettomanyrelated) | **GET** /v1/appEventLocalizations/{id}/appEventScreenshots |  |
| [**AppEventLocalizationsAppEventScreenshotsGetToManyRelationship**](AppEventLocalizationsApi.md#appeventlocalizationsappeventscreenshotsgettomanyrelationship) | **GET** /v1/appEventLocalizations/{id}/relationships/appEventScreenshots |  |
| [**AppEventLocalizationsAppEventVideoClipsGetToManyRelated**](AppEventLocalizationsApi.md#appeventlocalizationsappeventvideoclipsgettomanyrelated) | **GET** /v1/appEventLocalizations/{id}/appEventVideoClips |  |
| [**AppEventLocalizationsAppEventVideoClipsGetToManyRelationship**](AppEventLocalizationsApi.md#appeventlocalizationsappeventvideoclipsgettomanyrelationship) | **GET** /v1/appEventLocalizations/{id}/relationships/appEventVideoClips |  |
| [**AppEventLocalizationsCreateInstance**](AppEventLocalizationsApi.md#appeventlocalizationscreateinstance) | **POST** /v1/appEventLocalizations |  |
| [**AppEventLocalizationsDeleteInstance**](AppEventLocalizationsApi.md#appeventlocalizationsdeleteinstance) | **DELETE** /v1/appEventLocalizations/{id} |  |
| [**AppEventLocalizationsGetInstance**](AppEventLocalizationsApi.md#appeventlocalizationsgetinstance) | **GET** /v1/appEventLocalizations/{id} |  |
| [**AppEventLocalizationsUpdateInstance**](AppEventLocalizationsApi.md#appeventlocalizationsupdateinstance) | **PATCH** /v1/appEventLocalizations/{id} |  |

<a id="appeventlocalizationsappeventscreenshotsgettomanyrelated"></a>
# **AppEventLocalizationsAppEventScreenshotsGetToManyRelated**
> AppEventScreenshotsResponse AppEventLocalizationsAppEventScreenshotsGetToManyRelated (string id, List<string> fieldsAppEventScreenshots = null, List<string> fieldsAppEventLocalizations = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEventScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventScreenshots | [optional]  |
| **fieldsAppEventLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppEventScreenshotsResponse**](AppEventScreenshotsResponse.md)

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
| **200** | List of AppEventScreenshots |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventlocalizationsappeventscreenshotsgettomanyrelationship"></a>
# **AppEventLocalizationsAppEventScreenshotsGetToManyRelationship**
> AppEventLocalizationAppEventScreenshotsLinkagesResponse AppEventLocalizationsAppEventScreenshotsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppEventLocalizationAppEventScreenshotsLinkagesResponse**](AppEventLocalizationAppEventScreenshotsLinkagesResponse.md)

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

<a id="appeventlocalizationsappeventvideoclipsgettomanyrelated"></a>
# **AppEventLocalizationsAppEventVideoClipsGetToManyRelated**
> AppEventVideoClipsResponse AppEventLocalizationsAppEventVideoClipsGetToManyRelated (string id, List<string> fieldsAppEventVideoClips = null, List<string> fieldsAppEventLocalizations = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEventVideoClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventVideoClips | [optional]  |
| **fieldsAppEventLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppEventVideoClipsResponse**](AppEventVideoClipsResponse.md)

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
| **200** | List of AppEventVideoClips |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventlocalizationsappeventvideoclipsgettomanyrelationship"></a>
# **AppEventLocalizationsAppEventVideoClipsGetToManyRelationship**
> AppEventLocalizationAppEventVideoClipsLinkagesResponse AppEventLocalizationsAppEventVideoClipsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppEventLocalizationAppEventVideoClipsLinkagesResponse**](AppEventLocalizationAppEventVideoClipsLinkagesResponse.md)

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

<a id="appeventlocalizationscreateinstance"></a>
# **AppEventLocalizationsCreateInstance**
> AppEventLocalizationResponse AppEventLocalizationsCreateInstance (AppEventLocalizationCreateRequest appEventLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appEventLocalizationCreateRequest** | [**AppEventLocalizationCreateRequest**](AppEventLocalizationCreateRequest.md) | AppEventLocalization representation |  |

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
| **201** | Single AppEventLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventlocalizationsdeleteinstance"></a>
# **AppEventLocalizationsDeleteInstance**
> void AppEventLocalizationsDeleteInstance (string id)




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

<a id="appeventlocalizationsgetinstance"></a>
# **AppEventLocalizationsGetInstance**
> AppEventLocalizationResponse AppEventLocalizationsGetInstance (string id, List<string> fieldsAppEventLocalizations = null, List<string> fieldsAppEventScreenshots = null, List<string> fieldsAppEventVideoClips = null, List<string> include = null, int limitAppEventScreenshots = null, int limitAppEventVideoClips = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEventLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventLocalizations | [optional]  |
| **fieldsAppEventScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventScreenshots | [optional]  |
| **fieldsAppEventVideoClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEventVideoClips | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppEventScreenshots** | **int** | maximum number of related appEventScreenshots returned (when they are included) | [optional]  |
| **limitAppEventVideoClips** | **int** | maximum number of related appEventVideoClips returned (when they are included) | [optional]  |

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
| **200** | Single AppEventLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appeventlocalizationsupdateinstance"></a>
# **AppEventLocalizationsUpdateInstance**
> AppEventLocalizationResponse AppEventLocalizationsUpdateInstance (string id, AppEventLocalizationUpdateRequest appEventLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appEventLocalizationUpdateRequest** | [**AppEventLocalizationUpdateRequest**](AppEventLocalizationUpdateRequest.md) | AppEventLocalization representation |  |

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
| **200** | Single AppEventLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

