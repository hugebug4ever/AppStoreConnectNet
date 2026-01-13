# AppStoreConnect.Net.Api.AppStoreVersionExperimentTreatmentLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsCreateInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationscreateinstance) | **POST** /v1/appStoreVersionExperimentTreatmentLocalizations |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsdeleteinstance) | **DELETE** /v1/appStoreVersionExperimentTreatmentLocalizations/{id} |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsGetInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsgetinstance) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id} |  |

<a id="appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string> filterPreviewType = null, List<string> filterAppStoreVersionLocalization = null, List<string> filterAppCustomProductPageLocalization = null, List<string> fieldsAppPreviewSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppPreviews = null, int limit = null, List<string> include = null, int limitAppPreviews = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPreviewType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;previewType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppPreviews** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviews | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviews** | **int** | maximum number of related appPreviews returned (when they are included) | [optional]  |

### Return type

[**AppPreviewSetsResponse**](AppPreviewSetsResponse.md)

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
| **200** | List of AppPreviewSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship**
> AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse**](AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string> filterScreenshotDisplayType = null, List<string> filterAppStoreVersionLocalization = null, List<string> filterAppCustomProductPageLocalization = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppScreenshots = null, int limit = null, List<string> include = null, int limitAppScreenshots = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterScreenshotDisplayType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;screenshotDisplayType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppScreenshots** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshots | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppScreenshots** | **int** | maximum number of related appScreenshots returned (when they are included) | [optional]  |

### Return type

[**AppScreenshotSetsResponse**](AppScreenshotSetsResponse.md)

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
| **200** | List of AppScreenshotSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse**](AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appstoreversionexperimenttreatmentlocalizationscreateinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsCreateInstance**
> AppStoreVersionExperimentTreatmentLocalizationResponse AppStoreVersionExperimentTreatmentLocalizationsCreateInstance (AppStoreVersionExperimentTreatmentLocalizationCreateRequest appStoreVersionExperimentTreatmentLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentTreatmentLocalizationCreateRequest** | [**AppStoreVersionExperimentTreatmentLocalizationCreateRequest**](AppStoreVersionExperimentTreatmentLocalizationCreateRequest.md) | AppStoreVersionExperimentTreatmentLocalization representation |  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationResponse**](AppStoreVersionExperimentTreatmentLocalizationResponse.md)

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
| **201** | Single AppStoreVersionExperimentTreatmentLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsdeleteinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance**
> void AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance (string id)




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

<a id="appstoreversionexperimenttreatmentlocalizationsgetinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsGetInstance**
> AppStoreVersionExperimentTreatmentLocalizationResponse AppStoreVersionExperimentTreatmentLocalizationsGetInstance (string id, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppPreviewSets = null, List<string> include = null, int limitAppPreviewSets = null, int limitAppScreenshotSets = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationResponse**](AppStoreVersionExperimentTreatmentLocalizationResponse.md)

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
| **200** | Single AppStoreVersionExperimentTreatmentLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

