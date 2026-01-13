# AppStoreConnect.Net.Api.AppCustomProductPageLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/appPreviewSets |  |
| [**AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/appScreenshotSets |  |
| [**AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppCustomProductPageLocalizationsCreateInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationscreateinstance) | **POST** /v1/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageLocalizationsDeleteInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsdeleteinstance) | **DELETE** /v1/appCustomProductPageLocalizations/{id} |  |
| [**AppCustomProductPageLocalizationsGetInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsgetinstance) | **GET** /v1/appCustomProductPageLocalizations/{id} |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordscreatetomanyrelationship) | **POST** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsdeletetomanyrelationship) | **DELETE** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsUpdateInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsupdateinstance) | **PATCH** /v1/appCustomProductPageLocalizations/{id} |  |

<a id="appcustomproductpagelocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string> filterPreviewType = null, List<string> filterAppStoreVersionLocalization = null, List<string> filterAppStoreVersionExperimentTreatmentLocalization = null, List<string> fieldsAppPreviewSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppPreviews = null, int limit = null, List<string> include = null, int limitAppPreviews = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPreviewType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;previewType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
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

<a id="appcustomproductpagelocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship**
> AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse**](AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string> filterScreenshotDisplayType = null, List<string> filterAppStoreVersionLocalization = null, List<string> filterAppStoreVersionExperimentTreatmentLocalization = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string> fieldsAppScreenshots = null, int limit = null, List<string> include = null, int limitAppScreenshots = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterScreenshotDisplayType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;screenshotDisplayType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
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

<a id="appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse**](AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationscreateinstance"></a>
# **AppCustomProductPageLocalizationsCreateInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsCreateInstance (AppCustomProductPageLocalizationCreateRequest appCustomProductPageLocalizationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageLocalizationCreateRequest** | [**AppCustomProductPageLocalizationCreateRequest**](AppCustomProductPageLocalizationCreateRequest.md) | AppCustomProductPageLocalization representation |  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **201** | Single AppCustomProductPageLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpagelocalizationsdeleteinstance"></a>
# **AppCustomProductPageLocalizationsDeleteInstance**
> void AppCustomProductPageLocalizationsDeleteInstance (string id)




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

<a id="appcustomproductpagelocalizationsgetinstance"></a>
# **AppCustomProductPageLocalizationsGetInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsGetInstance (string id, List<string> fieldsAppCustomProductPageLocalizations = null, List<string> fieldsAppScreenshotSets = null, List<string> fieldsAppPreviewSets = null, List<string> include = null, int limitAppPreviewSets = null, int limitAppScreenshotSets = null, int limitSearchKeywords = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **200** | Single AppCustomProductPageLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appcustomproductpagelocalizationssearchkeywordscreatetomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship**
> void AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship (string id, AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest appCustomProductPageLocalizationSearchKeywordsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationSearchKeywordsLinkagesRequest** | [**AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest**](AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appcustomproductpagelocalizationssearchkeywordsdeletetomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship**
> void AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship (string id, AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest appCustomProductPageLocalizationSearchKeywordsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationSearchKeywordsLinkagesRequest** | [**AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest**](AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appcustomproductpagelocalizationssearchkeywordsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated**
> AppKeywordsResponse AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated (string id, List<string> filterPlatform = null, List<string> filterLocale = null, List<string> fieldsAppKeywords = null, int limit = null)




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

<a id="appcustomproductpagelocalizationssearchkeywordsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship**
> AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse**](AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationsupdateinstance"></a>
# **AppCustomProductPageLocalizationsUpdateInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsUpdateInstance (string id, AppCustomProductPageLocalizationUpdateRequest appCustomProductPageLocalizationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationUpdateRequest** | [**AppCustomProductPageLocalizationUpdateRequest**](AppCustomProductPageLocalizationUpdateRequest.md) | AppCustomProductPageLocalization representation |  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **200** | Single AppCustomProductPageLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

