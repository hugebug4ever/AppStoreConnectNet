# AppStoreConnect.Net.Api.AppStoreVersionLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/appPreviewSets |  |
| [**AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/appScreenshotSets |  |
| [**AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppStoreVersionLocalizationsCreateInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationscreateinstance) | **POST** /v1/appStoreVersionLocalizations |  |
| [**AppStoreVersionLocalizationsDeleteInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsdeleteinstance) | **DELETE** /v1/appStoreVersionLocalizations/{id} |  |
| [**AppStoreVersionLocalizationsGetInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsgetinstance) | **GET** /v1/appStoreVersionLocalizations/{id} |  |
| [**AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordscreatetomanyrelationship) | **POST** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsdeletetomanyrelationship) | **DELETE** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsUpdateInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsupdateinstance) | **PATCH** /v1/appStoreVersionLocalizations/{id} |  |

<a id="appstoreversionlocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string> filterPreviewType = null, List<string> filterAppCustomProductPageLocalization = null, List<string> filterAppStoreVersionExperimentTreatmentLocalization = null, List<string> fieldsAppPreviewSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppPreviews = null, int limit = null, List<string> include = null, int limitAppPreviews = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPreviewType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;previewType&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **filterAppStoreVersionExperimentTreatmentLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional]  |
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

<a id="appstoreversionlocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship**
> AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse**](AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string> filterScreenshotDisplayType = null, List<string> filterAppCustomProductPageLocalization = null, List<string> filterAppStoreVersionExperimentTreatmentLocalization = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppScreenshots = null, int limit = null, List<string> include = null, int limitAppScreenshots = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterScreenshotDisplayType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;screenshotDisplayType&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **filterAppStoreVersionExperimentTreatmentLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional]  |
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

<a id="appstoreversionlocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse**](AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationscreateinstance"></a>
# **AppStoreVersionLocalizationsCreateInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsCreateInstance (AppStoreVersionLocalizationCreateRequest appStoreVersionLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionLocalizationCreateRequest** | [**AppStoreVersionLocalizationCreateRequest**](AppStoreVersionLocalizationCreateRequest.md) | AppStoreVersionLocalization representation |  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **201** | Single AppStoreVersionLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionlocalizationsdeleteinstance"></a>
# **AppStoreVersionLocalizationsDeleteInstance**
> void AppStoreVersionLocalizationsDeleteInstance (string id)




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

<a id="appstoreversionlocalizationsgetinstance"></a>
# **AppStoreVersionLocalizationsGetInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsGetInstance (string id, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppPreviewSets = null, List<string> include = null, int limitAppPreviewSets = null, int limitAppScreenshotSets = null, int limitSearchKeywords = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **200** | Single AppStoreVersionLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionlocalizationssearchkeywordscreatetomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship**
> void AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship (string id, AppStoreVersionLocalizationSearchKeywordsLinkagesRequest appStoreVersionLocalizationSearchKeywordsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationSearchKeywordsLinkagesRequest** | [**AppStoreVersionLocalizationSearchKeywordsLinkagesRequest**](AppStoreVersionLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionlocalizationssearchkeywordsdeletetomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship**
> void AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship (string id, AppStoreVersionLocalizationSearchKeywordsLinkagesRequest appStoreVersionLocalizationSearchKeywordsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationSearchKeywordsLinkagesRequest** | [**AppStoreVersionLocalizationSearchKeywordsLinkagesRequest**](AppStoreVersionLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **422** | Unprocessable request entity error(s) |  -  |
| **409** | Request entity error(s) |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionlocalizationssearchkeywordsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated**
> AppKeywordsResponse AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated (string id, List<string> filterPlatform = null, List<string> filterLocale = null, List<string> fieldsAppKeywords = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by platform | [optional]  |
| **filterLocale** | [**List&lt;string&gt;**](string.md) | filter by locale | [optional]  |
| **fieldsAppKeywords** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appKeywords | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppKeywordsResponse**](AppKeywordsResponse.md)

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
| **200** | List of AppKeywords |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appstoreversionlocalizationssearchkeywordsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship**
> AppStoreVersionLocalizationSearchKeywordsLinkagesResponse AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppStoreVersionLocalizationSearchKeywordsLinkagesResponse**](AppStoreVersionLocalizationSearchKeywordsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationsupdateinstance"></a>
# **AppStoreVersionLocalizationsUpdateInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsUpdateInstance (string id, AppStoreVersionLocalizationUpdateRequest appStoreVersionLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationUpdateRequest** | [**AppStoreVersionLocalizationUpdateRequest**](AppStoreVersionLocalizationUpdateRequest.md) | AppStoreVersionLocalization representation |  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **200** | Single AppStoreVersionLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

