# AppStoreConnect.Net.Api.GameCenterAchievementsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAchievementsActivityUpdateToOneRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsactivityupdatetoonerelationship) | **PATCH** /v1/gameCenterAchievements/{id}/relationships/activity |  |
| [**GameCenterAchievementsCreateInstance**](GameCenterAchievementsApi.md#gamecenterachievementscreateinstance) | **POST** /v1/gameCenterAchievements |  |
| [**GameCenterAchievementsDeleteInstance**](GameCenterAchievementsApi.md#gamecenterachievementsdeleteinstance) | **DELETE** /v1/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsGetInstance**](GameCenterAchievementsApi.md#gamecenterachievementsgetinstance) | **GET** /v1/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsGroupAchievementGetToOneRelated**](GameCenterAchievementsApi.md#gamecenterachievementsgroupachievementgettoonerelated) | **GET** /v1/gameCenterAchievements/{id}/groupAchievement |  |
| [**GameCenterAchievementsGroupAchievementGetToOneRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsgroupachievementgettoonerelationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/groupAchievement |  |
| [**GameCenterAchievementsGroupAchievementUpdateToOneRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsgroupachievementupdatetoonerelationship) | **PATCH** /v1/gameCenterAchievements/{id}/relationships/groupAchievement |  |
| [**GameCenterAchievementsLocalizationsGetToManyRelated**](GameCenterAchievementsApi.md#gamecenterachievementslocalizationsgettomanyrelated) | **GET** /v1/gameCenterAchievements/{id}/localizations |  |
| [**GameCenterAchievementsLocalizationsGetToManyRelationship**](GameCenterAchievementsApi.md#gamecenterachievementslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/localizations |  |
| [**GameCenterAchievementsReleasesGetToManyRelated**](GameCenterAchievementsApi.md#gamecenterachievementsreleasesgettomanyrelated) | **GET** /v1/gameCenterAchievements/{id}/releases |  |
| [**GameCenterAchievementsReleasesGetToManyRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsreleasesgettomanyrelationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/releases |  |
| [**GameCenterAchievementsUpdateInstance**](GameCenterAchievementsApi.md#gamecenterachievementsupdateinstance) | **PATCH** /v1/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsV2ActivityUpdateToOneRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsv2activityupdatetoonerelationship) | **PATCH** /v2/gameCenterAchievements/{id}/relationships/activity |  |
| [**GameCenterAchievementsV2CreateInstance**](GameCenterAchievementsApi.md#gamecenterachievementsv2createinstance) | **POST** /v2/gameCenterAchievements |  |
| [**GameCenterAchievementsV2DeleteInstance**](GameCenterAchievementsApi.md#gamecenterachievementsv2deleteinstance) | **DELETE** /v2/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsV2GetInstance**](GameCenterAchievementsApi.md#gamecenterachievementsv2getinstance) | **GET** /v2/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsV2UpdateInstance**](GameCenterAchievementsApi.md#gamecenterachievementsv2updateinstance) | **PATCH** /v2/gameCenterAchievements/{id} |  |
| [**GameCenterAchievementsV2VersionsGetToManyRelated**](GameCenterAchievementsApi.md#gamecenterachievementsv2versionsgettomanyrelated) | **GET** /v2/gameCenterAchievements/{id}/versions |  |
| [**GameCenterAchievementsV2VersionsGetToManyRelationship**](GameCenterAchievementsApi.md#gamecenterachievementsv2versionsgettomanyrelationship) | **GET** /v2/gameCenterAchievements/{id}/relationships/versions |  |

<a id="gamecenterachievementsactivityupdatetoonerelationship"></a>
# **GameCenterAchievementsActivityUpdateToOneRelationship**
> void GameCenterAchievementsActivityUpdateToOneRelationship (string id, GameCenterAchievementActivityLinkageRequest gameCenterAchievementActivityLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementActivityLinkageRequest** | [**GameCenterAchievementActivityLinkageRequest**](GameCenterAchievementActivityLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterachievementscreateinstance"></a>
# **GameCenterAchievementsCreateInstance**
> GameCenterAchievementResponse GameCenterAchievementsCreateInstance (GameCenterAchievementCreateRequest gameCenterAchievementCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementCreateRequest** | [**GameCenterAchievementCreateRequest**](GameCenterAchievementCreateRequest.md) | GameCenterAchievement representation |  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **201** | Single GameCenterAchievement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsdeleteinstance"></a>
# **GameCenterAchievementsDeleteInstance**
> void GameCenterAchievementsDeleteInstance (string id)




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

<a id="gamecenterachievementsgetinstance"></a>
# **GameCenterAchievementsGetInstance**
> GameCenterAchievementResponse GameCenterAchievementsGetInstance (string id, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsgroupachievementgettoonerelated"></a>
# **GameCenterAchievementsGroupAchievementGetToOneRelated**
> GameCenterAchievementResponse GameCenterAchievementsGroupAchievementGetToOneRelated (string id, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> fieldsGameCenterActivities = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsgroupachievementgettoonerelationship"></a>
# **GameCenterAchievementsGroupAchievementGetToOneRelationship**
> GameCenterAchievementGroupAchievementLinkageResponse GameCenterAchievementsGroupAchievementGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAchievementGroupAchievementLinkageResponse**](GameCenterAchievementGroupAchievementLinkageResponse.md)

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

<a id="gamecenterachievementsgroupachievementupdatetoonerelationship"></a>
# **GameCenterAchievementsGroupAchievementUpdateToOneRelationship**
> void GameCenterAchievementsGroupAchievementUpdateToOneRelationship (string id, GameCenterAchievementGroupAchievementLinkageRequest gameCenterAchievementGroupAchievementLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementGroupAchievementLinkageRequest** | [**GameCenterAchievementGroupAchievementLinkageRequest**](GameCenterAchievementGroupAchievementLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterachievementslocalizationsgettomanyrelated"></a>
# **GameCenterAchievementsLocalizationsGetToManyRelated**
> GameCenterAchievementLocalizationsResponse GameCenterAchievementsLocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterAchievementImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementLocalizationsResponse**](GameCenterAchievementLocalizationsResponse.md)

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
| **200** | List of GameCenterAchievementLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementslocalizationsgettomanyrelationship"></a>
# **GameCenterAchievementsLocalizationsGetToManyRelationship**
> GameCenterAchievementLocalizationsLinkagesResponse GameCenterAchievementsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterAchievementLocalizationsLinkagesResponse**](GameCenterAchievementLocalizationsLinkagesResponse.md)

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

<a id="gamecenterachievementsreleasesgettomanyrelated"></a>
# **GameCenterAchievementsReleasesGetToManyRelated**
> GameCenterAchievementReleasesResponse GameCenterAchievementsReleasesGetToManyRelated (string id, List<string> filterLive = null, List<string> filterGameCenterDetail = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterAchievements = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLive** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;live&#39; | [optional]  |
| **filterGameCenterDetail** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterDetail&#39; | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterAchievementReleasesResponse**](GameCenterAchievementReleasesResponse.md)

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
| **200** | List of GameCenterAchievementReleases |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsreleasesgettomanyrelationship"></a>
# **GameCenterAchievementsReleasesGetToManyRelationship**
> GameCenterAchievementReleasesLinkagesResponse GameCenterAchievementsReleasesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterAchievementReleasesLinkagesResponse**](GameCenterAchievementReleasesLinkagesResponse.md)

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

<a id="gamecenterachievementsupdateinstance"></a>
# **GameCenterAchievementsUpdateInstance**
> GameCenterAchievementResponse GameCenterAchievementsUpdateInstance (string id, GameCenterAchievementUpdateRequest gameCenterAchievementUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementUpdateRequest** | [**GameCenterAchievementUpdateRequest**](GameCenterAchievementUpdateRequest.md) | GameCenterAchievement representation |  |

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsv2activityupdatetoonerelationship"></a>
# **GameCenterAchievementsV2ActivityUpdateToOneRelationship**
> void GameCenterAchievementsV2ActivityUpdateToOneRelationship (string id, GameCenterAchievementV2ActivityLinkageRequest gameCenterAchievementV2ActivityLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementV2ActivityLinkageRequest** | [**GameCenterAchievementV2ActivityLinkageRequest**](GameCenterAchievementV2ActivityLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterachievementsv2createinstance"></a>
# **GameCenterAchievementsV2CreateInstance**
> GameCenterAchievementV2Response GameCenterAchievementsV2CreateInstance (GameCenterAchievementV2CreateRequest gameCenterAchievementV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAchievementV2CreateRequest** | [**GameCenterAchievementV2CreateRequest**](GameCenterAchievementV2CreateRequest.md) | GameCenterAchievement representation |  |

### Return type

[**GameCenterAchievementV2Response**](GameCenterAchievementV2Response.md)

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
| **201** | Single GameCenterAchievement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsv2deleteinstance"></a>
# **GameCenterAchievementsV2DeleteInstance**
> void GameCenterAchievementsV2DeleteInstance (string id)




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

<a id="gamecenterachievementsv2getinstance"></a>
# **GameCenterAchievementsV2GetInstance**
> GameCenterAchievementV2Response GameCenterAchievementsV2GetInstance (string id, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterAchievementVersions = null, List<string> include = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementV2Response**](GameCenterAchievementV2Response.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsv2updateinstance"></a>
# **GameCenterAchievementsV2UpdateInstance**
> GameCenterAchievementV2Response GameCenterAchievementsV2UpdateInstance (string id, GameCenterAchievementV2UpdateRequest gameCenterAchievementV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAchievementV2UpdateRequest** | [**GameCenterAchievementV2UpdateRequest**](GameCenterAchievementV2UpdateRequest.md) | GameCenterAchievement representation |  |

### Return type

[**GameCenterAchievementV2Response**](GameCenterAchievementV2Response.md)

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
| **200** | Single GameCenterAchievement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsv2versionsgettomanyrelated"></a>
# **GameCenterAchievementsV2VersionsGetToManyRelated**
> GameCenterAchievementVersionsV2Response GameCenterAchievementsV2VersionsGetToManyRelated (string id, List<string> fieldsGameCenterAchievementVersions = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterAchievementLocalizations = null, int limit = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementVersionsV2Response**](GameCenterAchievementVersionsV2Response.md)

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
| **200** | List of GameCenterAchievementVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterachievementsv2versionsgettomanyrelationship"></a>
# **GameCenterAchievementsV2VersionsGetToManyRelationship**
> GameCenterAchievementV2VersionsLinkagesResponse GameCenterAchievementsV2VersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterAchievementV2VersionsLinkagesResponse**](GameCenterAchievementV2VersionsLinkagesResponse.md)

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

