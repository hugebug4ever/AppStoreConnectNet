# AppStoreConnect.Net.Api.AppClipDefaultExperiencesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelated**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesappclipappstorereviewdetailgettoonerelated) | **GET** /v1/appClipDefaultExperiences/{id}/appClipAppStoreReviewDetail |  |
| [**AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelationship**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesappclipappstorereviewdetailgettoonerelationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/appClipAppStoreReviewDetail |  |
| [**AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelated**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesappclipdefaultexperiencelocalizationsgettomanyrelated) | **GET** /v1/appClipDefaultExperiences/{id}/appClipDefaultExperienceLocalizations |  |
| [**AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelationship**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesappclipdefaultexperiencelocalizationsgettomanyrelationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/appClipDefaultExperienceLocalizations |  |
| [**AppClipDefaultExperiencesCreateInstance**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencescreateinstance) | **POST** /v1/appClipDefaultExperiences |  |
| [**AppClipDefaultExperiencesDeleteInstance**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesdeleteinstance) | **DELETE** /v1/appClipDefaultExperiences/{id} |  |
| [**AppClipDefaultExperiencesGetInstance**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesgetinstance) | **GET** /v1/appClipDefaultExperiences/{id} |  |
| [**AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelated**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesreleasewithappstoreversiongettoonerelated) | **GET** /v1/appClipDefaultExperiences/{id}/releaseWithAppStoreVersion |  |
| [**AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelationship**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesreleasewithappstoreversiongettoonerelationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion |  |
| [**AppClipDefaultExperiencesReleaseWithAppStoreVersionUpdateToOneRelationship**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesreleasewithappstoreversionupdatetoonerelationship) | **PATCH** /v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion |  |
| [**AppClipDefaultExperiencesUpdateInstance**](AppClipDefaultExperiencesApi.md#appclipdefaultexperiencesupdateinstance) | **PATCH** /v1/appClipDefaultExperiences/{id} |  |

<a id="appclipdefaultexperiencesappclipappstorereviewdetailgettoonerelated"></a>
# **AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelated**
> AppClipAppStoreReviewDetailResponse AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelated (string id, List<string> fieldsAppClipAppStoreReviewDetails = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppClipAppStoreReviewDetailResponse**](AppClipAppStoreReviewDetailResponse.md)

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
| **200** | Single AppClipAppStoreReviewDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipdefaultexperiencesappclipappstorereviewdetailgettoonerelationship"></a>
# **AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelationship**
> AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse AppClipDefaultExperiencesAppClipAppStoreReviewDetailGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse**](AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse.md)

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

<a id="appclipdefaultexperiencesappclipdefaultexperiencelocalizationsgettomanyrelated"></a>
# **AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelated**
> AppClipDefaultExperienceLocalizationsResponse AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelated (string id, List<string> filterLocale = null, List<string> fieldsAppClipDefaultExperienceLocalizations = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppClipHeaderImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLocale** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **fieldsAppClipDefaultExperienceLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppClipHeaderImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipHeaderImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppClipDefaultExperienceLocalizationsResponse**](AppClipDefaultExperienceLocalizationsResponse.md)

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
| **200** | List of AppClipDefaultExperienceLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipdefaultexperiencesappclipdefaultexperiencelocalizationsgettomanyrelationship"></a>
# **AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelationship**
> AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse AppClipDefaultExperiencesAppClipDefaultExperienceLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse**](AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse.md)

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

<a id="appclipdefaultexperiencescreateinstance"></a>
# **AppClipDefaultExperiencesCreateInstance**
> AppClipDefaultExperienceResponse AppClipDefaultExperiencesCreateInstance (AppClipDefaultExperienceCreateRequest appClipDefaultExperienceCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appClipDefaultExperienceCreateRequest** | [**AppClipDefaultExperienceCreateRequest**](AppClipDefaultExperienceCreateRequest.md) | AppClipDefaultExperience representation |  |

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
| **201** | Single AppClipDefaultExperience |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipdefaultexperiencesdeleteinstance"></a>
# **AppClipDefaultExperiencesDeleteInstance**
> void AppClipDefaultExperiencesDeleteInstance (string id)




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

<a id="appclipdefaultexperiencesgetinstance"></a>
# **AppClipDefaultExperiencesGetInstance**
> AppClipDefaultExperienceResponse AppClipDefaultExperiencesGetInstance (string id, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsAppClipDefaultExperienceLocalizations = null, List<string> fieldsAppClipAppStoreReviewDetails = null, List<string> include = null, int limitAppClipDefaultExperienceLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsAppClipDefaultExperienceLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional]  |
| **fieldsAppClipAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppClipDefaultExperienceLocalizations** | **int** | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
| **200** | Single AppClipDefaultExperience |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipdefaultexperiencesreleasewithappstoreversiongettoonerelated"></a>
# **AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelated**
> AppStoreVersionResponse AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelated (string id, List<string> fieldsAppStoreVersions = null, List<string> fieldsApps = null, List<string> fieldsAgeRatingDeclarations = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsBuilds = null, List<string> fieldsAppStoreVersionPhasedReleases = null, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsRoutingAppCoverages = null, List<string> fieldsAppStoreReviewDetails = null, List<string> fieldsAppStoreVersionSubmissions = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAlternativeDistributionPackages = null, List<string> include = null, int limitAppStoreVersionLocalizations = null, int limitAppStoreVersionExperiments = null, int limitAppStoreVersionExperimentsV2 = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsAppStoreVersionPhasedReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsRoutingAppCoverages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type routingAppCoverages | [optional]  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **fieldsAppStoreVersionSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionSubmissions | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionLocalizations** | **int** | maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperiments** | **int** | maximum number of related appStoreVersionExperiments returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
| **200** | Single AppStoreVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipdefaultexperiencesreleasewithappstoreversiongettoonerelationship"></a>
# **AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelationship**
> AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse AppClipDefaultExperiencesReleaseWithAppStoreVersionGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse**](AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse.md)

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

<a id="appclipdefaultexperiencesreleasewithappstoreversionupdatetoonerelationship"></a>
# **AppClipDefaultExperiencesReleaseWithAppStoreVersionUpdateToOneRelationship**
> void AppClipDefaultExperiencesReleaseWithAppStoreVersionUpdateToOneRelationship (string id, AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest appClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest** | [**AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest**](AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest.md) | Related linkage |  |

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

<a id="appclipdefaultexperiencesupdateinstance"></a>
# **AppClipDefaultExperiencesUpdateInstance**
> AppClipDefaultExperienceResponse AppClipDefaultExperiencesUpdateInstance (string id, AppClipDefaultExperienceUpdateRequest appClipDefaultExperienceUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appClipDefaultExperienceUpdateRequest** | [**AppClipDefaultExperienceUpdateRequest**](AppClipDefaultExperienceUpdateRequest.md) | AppClipDefaultExperience representation |  |

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
| **200** | Single AppClipDefaultExperience |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

