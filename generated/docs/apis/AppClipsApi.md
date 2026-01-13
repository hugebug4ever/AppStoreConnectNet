# AppStoreConnect.Net.Api.AppClipsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipsAppClipAdvancedExperiencesGetToManyRelated**](AppClipsApi.md#appclipsappclipadvancedexperiencesgettomanyrelated) | **GET** /v1/appClips/{id}/appClipAdvancedExperiences |  |
| [**AppClipsAppClipAdvancedExperiencesGetToManyRelationship**](AppClipsApi.md#appclipsappclipadvancedexperiencesgettomanyrelationship) | **GET** /v1/appClips/{id}/relationships/appClipAdvancedExperiences |  |
| [**AppClipsAppClipDefaultExperiencesGetToManyRelated**](AppClipsApi.md#appclipsappclipdefaultexperiencesgettomanyrelated) | **GET** /v1/appClips/{id}/appClipDefaultExperiences |  |
| [**AppClipsAppClipDefaultExperiencesGetToManyRelationship**](AppClipsApi.md#appclipsappclipdefaultexperiencesgettomanyrelationship) | **GET** /v1/appClips/{id}/relationships/appClipDefaultExperiences |  |
| [**AppClipsGetInstance**](AppClipsApi.md#appclipsgetinstance) | **GET** /v1/appClips/{id} |  |

<a id="appclipsappclipadvancedexperiencesgettomanyrelated"></a>
# **AppClipsAppClipAdvancedExperiencesGetToManyRelated**
> AppClipAdvancedExperiencesResponse AppClipsAppClipAdvancedExperiencesGetToManyRelated (string id, List<string> filterStatus = null, List<string> filterPlaceStatus = null, List<string> filterAction = null, List<string> fieldsAppClipAdvancedExperiences = null, List<string> fieldsAppClips = null, List<string> fieldsAppClipAdvancedExperienceImages = null, List<string> fieldsAppClipAdvancedExperienceLocalizations = null, int limit = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterStatus** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;status&#39; | [optional]  |
| **filterPlaceStatus** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;placeStatus&#39; | [optional]  |
| **filterAction** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;action&#39; | [optional]  |
| **fieldsAppClipAdvancedExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAdvancedExperiences | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppClipAdvancedExperienceImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAdvancedExperienceImages | [optional]  |
| **fieldsAppClipAdvancedExperienceLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAdvancedExperienceLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**AppClipAdvancedExperiencesResponse**](AppClipAdvancedExperiencesResponse.md)

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
| **200** | List of AppClipAdvancedExperiences |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipsappclipadvancedexperiencesgettomanyrelationship"></a>
# **AppClipsAppClipAdvancedExperiencesGetToManyRelationship**
> AppClipAppClipAdvancedExperiencesLinkagesResponse AppClipsAppClipAdvancedExperiencesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppClipAppClipAdvancedExperiencesLinkagesResponse**](AppClipAppClipAdvancedExperiencesLinkagesResponse.md)

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

<a id="appclipsappclipdefaultexperiencesgettomanyrelated"></a>
# **AppClipsAppClipDefaultExperiencesGetToManyRelated**
> AppClipDefaultExperiencesResponse AppClipsAppClipDefaultExperiencesGetToManyRelated (string id, bool existsReleaseWithAppStoreVersion = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppClips = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsAppClipDefaultExperienceLocalizations = null, List<string> fieldsAppClipAppStoreReviewDetails = null, int limit = null, List<string> include = null, int limitAppClipDefaultExperienceLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **existsReleaseWithAppStoreVersion** | **bool** | filter by existence or non-existence of related &#39;releaseWithAppStoreVersion&#39; | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsAppClipDefaultExperienceLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional]  |
| **fieldsAppClipAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppClipDefaultExperienceLocalizations** | **int** | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppClipDefaultExperiencesResponse**](AppClipDefaultExperiencesResponse.md)

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
| **200** | List of AppClipDefaultExperiences |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="appclipsappclipdefaultexperiencesgettomanyrelationship"></a>
# **AppClipsAppClipDefaultExperiencesGetToManyRelationship**
> AppClipAppClipDefaultExperiencesLinkagesResponse AppClipsAppClipDefaultExperiencesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppClipAppClipDefaultExperiencesLinkagesResponse**](AppClipAppClipDefaultExperiencesLinkagesResponse.md)

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

<a id="appclipsgetinstance"></a>
# **AppClipsGetInstance**
> AppClipResponse AppClipsGetInstance (string id, List<string> fieldsAppClips = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> include = null, int limitAppClipDefaultExperiences = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClips** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppClipDefaultExperiences** | **int** | maximum number of related appClipDefaultExperiences returned (when they are included) | [optional]  |

### Return type

[**AppClipResponse**](AppClipResponse.md)

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
| **200** | Single AppClip |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

