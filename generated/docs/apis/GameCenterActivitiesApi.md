# AppStoreConnect.Net.Api.GameCenterActivitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterActivitiesAchievementsCreateToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesachievementscreatetomanyrelationship) | **POST** /v1/gameCenterActivities/{id}/relationships/achievements |  |
| [**GameCenterActivitiesAchievementsDeleteToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesachievementsdeletetomanyrelationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/achievements |  |
| [**GameCenterActivitiesAchievementsV2CreateToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesachievementsv2createtomanyrelationship) | **POST** /v1/gameCenterActivities/{id}/relationships/achievementsV2 |  |
| [**GameCenterActivitiesAchievementsV2DeleteToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesachievementsv2deletetomanyrelationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/achievementsV2 |  |
| [**GameCenterActivitiesCreateInstance**](GameCenterActivitiesApi.md#gamecenteractivitiescreateinstance) | **POST** /v1/gameCenterActivities |  |
| [**GameCenterActivitiesDeleteInstance**](GameCenterActivitiesApi.md#gamecenteractivitiesdeleteinstance) | **DELETE** /v1/gameCenterActivities/{id} |  |
| [**GameCenterActivitiesGetInstance**](GameCenterActivitiesApi.md#gamecenteractivitiesgetinstance) | **GET** /v1/gameCenterActivities/{id} |  |
| [**GameCenterActivitiesLeaderboardsCreateToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesleaderboardscreatetomanyrelationship) | **POST** /v1/gameCenterActivities/{id}/relationships/leaderboards |  |
| [**GameCenterActivitiesLeaderboardsDeleteToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesleaderboardsdeletetomanyrelationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/leaderboards |  |
| [**GameCenterActivitiesLeaderboardsV2CreateToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesleaderboardsv2createtomanyrelationship) | **POST** /v1/gameCenterActivities/{id}/relationships/leaderboardsV2 |  |
| [**GameCenterActivitiesLeaderboardsV2DeleteToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesleaderboardsv2deletetomanyrelationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/leaderboardsV2 |  |
| [**GameCenterActivitiesUpdateInstance**](GameCenterActivitiesApi.md#gamecenteractivitiesupdateinstance) | **PATCH** /v1/gameCenterActivities/{id} |  |
| [**GameCenterActivitiesVersionsGetToManyRelated**](GameCenterActivitiesApi.md#gamecenteractivitiesversionsgettomanyrelated) | **GET** /v1/gameCenterActivities/{id}/versions |  |
| [**GameCenterActivitiesVersionsGetToManyRelationship**](GameCenterActivitiesApi.md#gamecenteractivitiesversionsgettomanyrelationship) | **GET** /v1/gameCenterActivities/{id}/relationships/versions |  |

<a id="gamecenteractivitiesachievementscreatetomanyrelationship"></a>
# **GameCenterActivitiesAchievementsCreateToManyRelationship**
> void GameCenterActivitiesAchievementsCreateToManyRelationship (string id, GameCenterActivityAchievementsLinkagesRequest gameCenterActivityAchievementsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityAchievementsLinkagesRequest** | [**GameCenterActivityAchievementsLinkagesRequest**](GameCenterActivityAchievementsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesachievementsdeletetomanyrelationship"></a>
# **GameCenterActivitiesAchievementsDeleteToManyRelationship**
> void GameCenterActivitiesAchievementsDeleteToManyRelationship (string id, GameCenterActivityAchievementsLinkagesRequest gameCenterActivityAchievementsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityAchievementsLinkagesRequest** | [**GameCenterActivityAchievementsLinkagesRequest**](GameCenterActivityAchievementsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesachievementsv2createtomanyrelationship"></a>
# **GameCenterActivitiesAchievementsV2CreateToManyRelationship**
> void GameCenterActivitiesAchievementsV2CreateToManyRelationship (string id, GameCenterActivityAchievementsV2LinkagesRequest gameCenterActivityAchievementsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityAchievementsV2LinkagesRequest** | [**GameCenterActivityAchievementsV2LinkagesRequest**](GameCenterActivityAchievementsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesachievementsv2deletetomanyrelationship"></a>
# **GameCenterActivitiesAchievementsV2DeleteToManyRelationship**
> void GameCenterActivitiesAchievementsV2DeleteToManyRelationship (string id, GameCenterActivityAchievementsV2LinkagesRequest gameCenterActivityAchievementsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityAchievementsV2LinkagesRequest** | [**GameCenterActivityAchievementsV2LinkagesRequest**](GameCenterActivityAchievementsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiescreateinstance"></a>
# **GameCenterActivitiesCreateInstance**
> GameCenterActivityResponse GameCenterActivitiesCreateInstance (GameCenterActivityCreateRequest gameCenterActivityCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterActivityCreateRequest** | [**GameCenterActivityCreateRequest**](GameCenterActivityCreateRequest.md) | GameCenterActivity representation |  |

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
| **201** | Single GameCenterActivity |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitiesdeleteinstance"></a>
# **GameCenterActivitiesDeleteInstance**
> void GameCenterActivitiesDeleteInstance (string id)




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

<a id="gamecenteractivitiesgetinstance"></a>
# **GameCenterActivitiesGetInstance**
> GameCenterActivityResponse GameCenterActivitiesGetInstance (string id, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterActivityVersions = null, List<string> include = null, int limitAchievements = null, int limitAchievementsV2 = null, int limitLeaderboards = null, int limitLeaderboardsV2 = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAchievements** | **int** | maximum number of related achievements returned (when they are included) | [optional]  |
| **limitAchievementsV2** | **int** | maximum number of related achievementsV2 returned (when they are included) | [optional]  |
| **limitLeaderboards** | **int** | maximum number of related leaderboards returned (when they are included) | [optional]  |
| **limitLeaderboardsV2** | **int** | maximum number of related leaderboardsV2 returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
| **200** | Single GameCenterActivity |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitiesleaderboardscreatetomanyrelationship"></a>
# **GameCenterActivitiesLeaderboardsCreateToManyRelationship**
> void GameCenterActivitiesLeaderboardsCreateToManyRelationship (string id, GameCenterActivityLeaderboardsLinkagesRequest gameCenterActivityLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLeaderboardsLinkagesRequest** | [**GameCenterActivityLeaderboardsLinkagesRequest**](GameCenterActivityLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesleaderboardsdeletetomanyrelationship"></a>
# **GameCenterActivitiesLeaderboardsDeleteToManyRelationship**
> void GameCenterActivitiesLeaderboardsDeleteToManyRelationship (string id, GameCenterActivityLeaderboardsLinkagesRequest gameCenterActivityLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLeaderboardsLinkagesRequest** | [**GameCenterActivityLeaderboardsLinkagesRequest**](GameCenterActivityLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesleaderboardsv2createtomanyrelationship"></a>
# **GameCenterActivitiesLeaderboardsV2CreateToManyRelationship**
> void GameCenterActivitiesLeaderboardsV2CreateToManyRelationship (string id, GameCenterActivityLeaderboardsV2LinkagesRequest gameCenterActivityLeaderboardsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLeaderboardsV2LinkagesRequest** | [**GameCenterActivityLeaderboardsV2LinkagesRequest**](GameCenterActivityLeaderboardsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesleaderboardsv2deletetomanyrelationship"></a>
# **GameCenterActivitiesLeaderboardsV2DeleteToManyRelationship**
> void GameCenterActivitiesLeaderboardsV2DeleteToManyRelationship (string id, GameCenterActivityLeaderboardsV2LinkagesRequest gameCenterActivityLeaderboardsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityLeaderboardsV2LinkagesRequest** | [**GameCenterActivityLeaderboardsV2LinkagesRequest**](GameCenterActivityLeaderboardsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenteractivitiesupdateinstance"></a>
# **GameCenterActivitiesUpdateInstance**
> GameCenterActivityResponse GameCenterActivitiesUpdateInstance (string id, GameCenterActivityUpdateRequest gameCenterActivityUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterActivityUpdateRequest** | [**GameCenterActivityUpdateRequest**](GameCenterActivityUpdateRequest.md) | GameCenterActivity representation |  |

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
| **200** | Single GameCenterActivity |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitiesversionsgettomanyrelated"></a>
# **GameCenterActivitiesVersionsGetToManyRelated**
> GameCenterActivityVersionsResponse GameCenterActivitiesVersionsGetToManyRelated (string id, List<string> fieldsGameCenterActivityVersions = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterActivityLocalizations = null, List<string> fieldsGameCenterActivityImages = null, List<string> fieldsGameCenterActivityVersionReleases = null, int limit = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterActivityLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityLocalizations | [optional]  |
| **fieldsGameCenterActivityImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityImages | [optional]  |
| **fieldsGameCenterActivityVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterActivityVersionsResponse**](GameCenterActivityVersionsResponse.md)

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
| **200** | List of GameCenterActivityVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenteractivitiesversionsgettomanyrelationship"></a>
# **GameCenterActivitiesVersionsGetToManyRelationship**
> GameCenterActivityVersionsLinkagesResponse GameCenterActivitiesVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterActivityVersionsLinkagesResponse**](GameCenterActivityVersionsLinkagesResponse.md)

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

