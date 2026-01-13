# AppStoreConnect.Net.Api.GameCenterGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterGroupsCreateInstance**](GameCenterGroupsApi.md#gamecentergroupscreateinstance) | **POST** /v1/gameCenterGroups |  |
| [**GameCenterGroupsDeleteInstance**](GameCenterGroupsApi.md#gamecentergroupsdeleteinstance) | **DELETE** /v1/gameCenterGroups/{id} |  |
| [**GameCenterGroupsGameCenterAchievementsGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterAchievements |  |
| [**GameCenterGroupsGameCenterAchievementsGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievements |  |
| [**GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsreplacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievements |  |
| [**GameCenterGroupsGameCenterAchievementsV2GetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsv2gettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterAchievementsV2 |  |
| [**GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsv2gettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievementsV2 |  |
| [**GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterachievementsv2replacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievementsV2 |  |
| [**GameCenterGroupsGameCenterActivitiesGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenteractivitiesgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterActivities |  |
| [**GameCenterGroupsGameCenterActivitiesGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenteractivitiesgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterActivities |  |
| [**GameCenterGroupsGameCenterChallengesGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterchallengesgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterChallenges |  |
| [**GameCenterGroupsGameCenterChallengesGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterchallengesgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterChallenges |  |
| [**GameCenterGroupsGameCenterDetailsGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterdetailsgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterDetails |  |
| [**GameCenterGroupsGameCenterDetailsGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterdetailsgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterDetails |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboardSets |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSets |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsreplacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSets |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboardSetsV2 |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSetsV2 |  |
| [**GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsetsv2replacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSetsV2 |  |
| [**GameCenterGroupsGameCenterLeaderboardsGetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsgettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboards |  |
| [**GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsgettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsreplacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsv2gettomanyrelated) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboardsV2 |  |
| [**GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsv2gettomanyrelationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardsV2 |  |
| [**GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship**](GameCenterGroupsApi.md#gamecentergroupsgamecenterleaderboardsv2replacetomanyrelationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardsV2 |  |
| [**GameCenterGroupsGetCollection**](GameCenterGroupsApi.md#gamecentergroupsgetcollection) | **GET** /v1/gameCenterGroups |  |
| [**GameCenterGroupsGetInstance**](GameCenterGroupsApi.md#gamecentergroupsgetinstance) | **GET** /v1/gameCenterGroups/{id} |  |
| [**GameCenterGroupsUpdateInstance**](GameCenterGroupsApi.md#gamecentergroupsupdateinstance) | **PATCH** /v1/gameCenterGroups/{id} |  |

<a id="gamecentergroupscreateinstance"></a>
# **GameCenterGroupsCreateInstance**
> GameCenterGroupResponse GameCenterGroupsCreateInstance (GameCenterGroupCreateRequest gameCenterGroupCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterGroupCreateRequest** | [**GameCenterGroupCreateRequest**](GameCenterGroupCreateRequest.md) | GameCenterGroup representation |  |

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
| **201** | Single GameCenterGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsdeleteinstance"></a>
# **GameCenterGroupsDeleteInstance**
> void GameCenterGroupsDeleteInstance (string id)




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

<a id="gamecentergroupsgamecenterachievementsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterAchievementsGetToManyRelated**
> GameCenterAchievementsResponse GameCenterGroupsGameCenterAchievementsGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterAchievementLocalizations = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> fieldsGameCenterActivities = null, int limit = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementsResponse**](GameCenterAchievementsResponse.md)

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
| **200** | List of GameCenterAchievements |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterachievementsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsGetToManyRelationship**
> GameCenterGroupGameCenterAchievementsLinkagesResponse GameCenterGroupsGameCenterAchievementsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterAchievementsLinkagesResponse**](GameCenterGroupGameCenterAchievementsLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterachievementsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship (string id, GameCenterGroupGameCenterAchievementsLinkagesRequest gameCenterGroupGameCenterAchievementsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterAchievementsLinkagesRequest** | [**GameCenterGroupGameCenterAchievementsLinkagesRequest**](GameCenterGroupGameCenterAchievementsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgamecenterachievementsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterAchievementsV2GetToManyRelated**
> GameCenterAchievementsV2Response GameCenterGroupsGameCenterAchievementsV2GetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterAchievementVersions = null, int limit = null, List<string> include = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAchievementsV2Response**](GameCenterAchievementsV2Response.md)

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
| **200** | List of GameCenterAchievements |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterachievementsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship**
> GameCenterGroupGameCenterAchievementsV2LinkagesResponse GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterAchievementsV2LinkagesResponse**](GameCenterGroupGameCenterAchievementsV2LinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterachievementsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterAchievementsV2LinkagesRequest gameCenterGroupGameCenterAchievementsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterAchievementsV2LinkagesRequest** | [**GameCenterGroupGameCenterAchievementsV2LinkagesRequest**](GameCenterGroupGameCenterAchievementsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgamecenteractivitiesgettomanyrelated"></a>
# **GameCenterGroupsGameCenterActivitiesGetToManyRelated**
> GameCenterActivitiesResponse GameCenterGroupsGameCenterActivitiesGetToManyRelated (string id, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterActivityVersions = null, int limit = null, List<string> include = null, int limitAchievements = null, int limitAchievementsV2 = null, int limitLeaderboards = null, int limitLeaderboardsV2 = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAchievements** | **int** | maximum number of related achievements returned (when they are included) | [optional]  |
| **limitAchievementsV2** | **int** | maximum number of related achievementsV2 returned (when they are included) | [optional]  |
| **limitLeaderboards** | **int** | maximum number of related leaderboards returned (when they are included) | [optional]  |
| **limitLeaderboardsV2** | **int** | maximum number of related leaderboardsV2 returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterActivitiesResponse**](GameCenterActivitiesResponse.md)

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
| **200** | List of GameCenterActivities |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenteractivitiesgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterActivitiesGetToManyRelationship**
> GameCenterGroupGameCenterActivitiesLinkagesResponse GameCenterGroupsGameCenterActivitiesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterActivitiesLinkagesResponse**](GameCenterGroupGameCenterActivitiesLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterchallengesgettomanyrelated"></a>
# **GameCenterGroupsGameCenterChallengesGetToManyRelated**
> GameCenterChallengesResponse GameCenterGroupsGameCenterChallengesGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterChallengeVersions = null, List<string> fieldsGameCenterLeaderboards = null, int limit = null, List<string> include = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterChallengesResponse**](GameCenterChallengesResponse.md)

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
| **200** | List of GameCenterChallenges |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterchallengesgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterChallengesGetToManyRelationship**
> GameCenterGroupGameCenterChallengesLinkagesResponse GameCenterGroupsGameCenterChallengesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterChallengesLinkagesResponse**](GameCenterGroupGameCenterChallengesLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterdetailsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterDetailsGetToManyRelated**
> GameCenterDetailsResponse GameCenterGroupsGameCenterDetailsGetToManyRelated (string id, List<string> filterGameCenterAppVersionsEnabled = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsApps = null, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterAchievementReleases = null, List<string> fieldsGameCenterActivityVersionReleases = null, List<string> fieldsGameCenterChallengeVersionReleases = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> fieldsGameCenterLeaderboardSetReleases = null, List<string> fieldsAppStoreVersions = null, int limit = null, List<string> include = null, int limitGameCenterAppVersions = null, int limitGameCenterLeaderboards = null, int limitGameCenterLeaderboardsV2 = null, int limitGameCenterLeaderboardSets = null, int limitGameCenterLeaderboardSetsV2 = null, int limitGameCenterAchievements = null, int limitGameCenterAchievementsV2 = null, int limitGameCenterActivities = null, int limitGameCenterChallenges = null, int limitAchievementReleases = null, int limitActivityReleases = null, int limitChallengeReleases = null, int limitLeaderboardReleases = null, int limitLeaderboardSetReleases = null, int limitChallengesMinimumPlatformVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterGameCenterAppVersionsEnabled** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;gameCenterAppVersions.enabled&#39; | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivityVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional]  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAppVersions** | **int** | maximum number of related gameCenterAppVersions returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterAchievements** | **int** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitAchievementReleases** | **int** | maximum number of related achievementReleases returned (when they are included) | [optional]  |
| **limitActivityReleases** | **int** | maximum number of related activityReleases returned (when they are included) | [optional]  |
| **limitChallengeReleases** | **int** | maximum number of related challengeReleases returned (when they are included) | [optional]  |
| **limitLeaderboardReleases** | **int** | maximum number of related leaderboardReleases returned (when they are included) | [optional]  |
| **limitLeaderboardSetReleases** | **int** | maximum number of related leaderboardSetReleases returned (when they are included) | [optional]  |
| **limitChallengesMinimumPlatformVersions** | **int** | maximum number of related challengesMinimumPlatformVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterDetailsResponse**](GameCenterDetailsResponse.md)

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
| **200** | List of GameCenterDetails |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterdetailsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterDetailsGetToManyRelationship**
> GameCenterGroupGameCenterDetailsLinkagesResponse GameCenterGroupsGameCenterDetailsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterDetailsLinkagesResponse**](GameCenterGroupGameCenterDetailsLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterleaderboardsetsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated**
> GameCenterLeaderboardSetsResponse GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSetReleases = null, int limit = null, List<string> include = null, int limitLocalizations = null, int limitGameCenterLeaderboards = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetsResponse**](GameCenterLeaderboardSetsResponse.md)

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
| **200** | List of GameCenterLeaderboardSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse**](GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterleaderboardsetsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest** | [**GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest**](GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated**
> GameCenterLeaderboardSetsV2Response GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSetVersions = null, int limit = null, List<string> include = null, int limitGameCenterLeaderboards = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetsV2Response**](GameCenterLeaderboardSetsV2Response.md)

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
| **200** | List of GameCenterLeaderboardSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse**](GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterleaderboardsetsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest** | [**GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest**](GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsResponse GameCenterGroupsGameCenterLeaderboardsGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, int limit = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardsResponse**](GameCenterLeaderboardsResponse.md)

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
| **200** | List of GameCenterLeaderboards |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardsLinkagesResponse GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterLeaderboardsLinkagesResponse**](GameCenterGroupGameCenterLeaderboardsLinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardsLinkagesRequest gameCenterGroupGameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterLeaderboardsLinkagesRequest** | [**GameCenterGroupGameCenterLeaderboardsLinkagesRequest**](GameCenterGroupGameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgamecenterleaderboardsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated**
> GameCenterLeaderboardsV2Response GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterLeaderboardVersions = null, int limit = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardsV2Response**](GameCenterLeaderboardsV2Response.md)

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
| **200** | List of GameCenterLeaderboards |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgamecenterleaderboardsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse**](GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse.md)

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

<a id="gamecentergroupsgamecenterleaderboardsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest** | [**GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest**](GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecentergroupsgetcollection"></a>
# **GameCenterGroupsGetCollection**
> GameCenterGroupsResponse GameCenterGroupsGetCollection (List<string> filterGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, int limit = null, List<string> include = null, int limitGameCenterAchievements = null, int limitGameCenterAchievementsV2 = null, int limitGameCenterActivities = null, int limitGameCenterChallenges = null, int limitGameCenterDetails = null, int limitGameCenterLeaderboardSets = null, int limitGameCenterLeaderboardSetsV2 = null, int limitGameCenterLeaderboards = null, int limitGameCenterLeaderboardsV2 = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterGameCenterDetails** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterDetails&#39; | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAchievements** | **int** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitGameCenterDetails** | **int** | maximum number of related gameCenterDetails returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |

### Return type

[**GameCenterGroupsResponse**](GameCenterGroupsResponse.md)

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
| **200** | List of GameCenterGroups |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsgetinstance"></a>
# **GameCenterGroupsGetInstance**
> GameCenterGroupResponse GameCenterGroupsGetInstance (string id, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterAchievements = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, List<string> include = null, int limitGameCenterAchievements = null, int limitGameCenterAchievementsV2 = null, int limitGameCenterActivities = null, int limitGameCenterChallenges = null, int limitGameCenterDetails = null, int limitGameCenterLeaderboardSets = null, int limitGameCenterLeaderboardSetsV2 = null, int limitGameCenterLeaderboards = null, int limitGameCenterLeaderboardsV2 = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAchievements** | **int** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitGameCenterDetails** | **int** | maximum number of related gameCenterDetails returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
| **200** | Single GameCenterGroup |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentergroupsupdateinstance"></a>
# **GameCenterGroupsUpdateInstance**
> GameCenterGroupResponse GameCenterGroupsUpdateInstance (string id, GameCenterGroupUpdateRequest gameCenterGroupUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterGroupUpdateRequest** | [**GameCenterGroupUpdateRequest**](GameCenterGroupUpdateRequest.md) | GameCenterGroup representation |  |

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
| **200** | Single GameCenterGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

