# AppStoreConnect.Net.Api.GameCenterLeaderboardSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetsCreateInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetscreateinstance) | **POST** /v1/gameCenterLeaderboardSets |  |
| [**GameCenterLeaderboardSetsDeleteInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgamecenterleaderboardscreatetomanyrelationship) | **POST** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgamecenterleaderboardsdeletetomanyrelationship) | **DELETE** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelated) | **GET** /v1/gameCenterLeaderboardSets/{id}/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgamecenterleaderboardsreplacetomanyrelationship) | **PATCH** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsGetInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgetinstance) | **GET** /v1/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgroupleaderboardsetgettoonerelated) | **GET** /v1/gameCenterLeaderboardSets/{id}/groupLeaderboardSet |  |
| [**GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgroupleaderboardsetgettoonerelationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/groupLeaderboardSet |  |
| [**GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsgroupleaderboardsetupdatetoonerelationship) | **PATCH** /v1/gameCenterLeaderboardSets/{id}/relationships/groupLeaderboardSet |  |
| [**GameCenterLeaderboardSetsLocalizationsGetToManyRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetslocalizationsgettomanyrelated) | **GET** /v1/gameCenterLeaderboardSets/{id}/localizations |  |
| [**GameCenterLeaderboardSetsLocalizationsGetToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/localizations |  |
| [**GameCenterLeaderboardSetsReleasesGetToManyRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsreleasesgettomanyrelated) | **GET** /v1/gameCenterLeaderboardSets/{id}/releases |  |
| [**GameCenterLeaderboardSetsReleasesGetToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsreleasesgettomanyrelationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/releases |  |
| [**GameCenterLeaderboardSetsUpdateInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsV2CreateInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2createinstance) | **POST** /v2/gameCenterLeaderboardSets |  |
| [**GameCenterLeaderboardSetsV2DeleteInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2gamecenterleaderboardscreatetomanyrelationship) | **POST** /v2/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2gamecenterleaderboardsdeletetomanyrelationship) | **DELETE** /v2/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardSets/{id}/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2gamecenterleaderboardsreplacetomanyrelationship) | **PATCH** /v2/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardSetsV2GetInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2getinstance) | **GET** /v2/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsV2UpdateInstance**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboardSets/{id} |  |
| [**GameCenterLeaderboardSetsV2VersionsGetToManyRelated**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2versionsgettomanyrelated) | **GET** /v2/gameCenterLeaderboardSets/{id}/versions |  |
| [**GameCenterLeaderboardSetsV2VersionsGetToManyRelationship**](GameCenterLeaderboardSetsApi.md#gamecenterleaderboardsetsv2versionsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboardSets/{id}/relationships/versions |  |

<a id="gamecenterleaderboardsetscreateinstance"></a>
# **GameCenterLeaderboardSetsCreateInstance**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsCreateInstance (GameCenterLeaderboardSetCreateRequest gameCenterLeaderboardSetCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetCreateRequest** | [**GameCenterLeaderboardSetCreateRequest**](GameCenterLeaderboardSetCreateRequest.md) | GameCenterLeaderboardSet representation |  |

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
| **201** | Single GameCenterLeaderboardSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsdeleteinstance"></a>
# **GameCenterLeaderboardSetsDeleteInstance**
> void GameCenterLeaderboardSetsDeleteInstance (string id)




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

<a id="gamecenterleaderboardsetsgamecenterleaderboardscreatetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsgamecenterleaderboardsdeletetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsResponse GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, int limit = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitLocalizations = null, int limitReleases = null)




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

<a id="gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship**
> GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse.md)

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

<a id="gamecenterleaderboardsetsgamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsgetinstance"></a>
# **GameCenterLeaderboardSetsGetInstance**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsGetInstance (string id, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSetReleases = null, List<string> include = null, int limitGameCenterLeaderboards = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
| **200** | Single GameCenterLeaderboardSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsgroupleaderboardsetgettoonerelated"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSetReleases = null, List<string> include = null, int limitLocalizations = null, int limitGameCenterLeaderboards = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
| **200** | Single GameCenterLeaderboardSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsgroupleaderboardsetgettoonerelationship"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship**
> GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse**](GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse.md)

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

<a id="gamecenterleaderboardsetsgroupleaderboardsetupdatetoonerelationship"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship**
> void GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship (string id, GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest** | [**GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest**](GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardsetslocalizationsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsLocalizationsGetToManyRelated**
> GameCenterLeaderboardSetLocalizationsResponse GameCenterLeaderboardSetsLocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardSetImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationsResponse**](GameCenterLeaderboardSetLocalizationsResponse.md)

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
| **200** | List of GameCenterLeaderboardSetLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetslocalizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsLocalizationsGetToManyRelationship**
> GameCenterLeaderboardSetLocalizationsLinkagesResponse GameCenterLeaderboardSetsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetLocalizationsLinkagesResponse**](GameCenterLeaderboardSetLocalizationsLinkagesResponse.md)

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

<a id="gamecenterleaderboardsetsreleasesgettomanyrelated"></a>
# **GameCenterLeaderboardSetsReleasesGetToManyRelated**
> GameCenterLeaderboardSetReleasesResponse GameCenterLeaderboardSetsReleasesGetToManyRelated (string id, List<string> filterLive = null, List<string> filterGameCenterDetail = null, List<string> fieldsGameCenterLeaderboardSetReleases = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterLeaderboardSets = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLive** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;live&#39; | [optional]  |
| **filterGameCenterDetail** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterDetail&#39; | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetReleasesResponse**](GameCenterLeaderboardSetReleasesResponse.md)

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
| **200** | List of GameCenterLeaderboardSetReleases |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsreleasesgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsReleasesGetToManyRelationship**
> GameCenterLeaderboardSetReleasesLinkagesResponse GameCenterLeaderboardSetsReleasesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetReleasesLinkagesResponse**](GameCenterLeaderboardSetReleasesLinkagesResponse.md)

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

<a id="gamecenterleaderboardsetsupdateinstance"></a>
# **GameCenterLeaderboardSetsUpdateInstance**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsUpdateInstance (string id, GameCenterLeaderboardSetUpdateRequest gameCenterLeaderboardSetUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetUpdateRequest** | [**GameCenterLeaderboardSetUpdateRequest**](GameCenterLeaderboardSetUpdateRequest.md) | GameCenterLeaderboardSet representation |  |

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
| **200** | Single GameCenterLeaderboardSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsv2createinstance"></a>
# **GameCenterLeaderboardSetsV2CreateInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2CreateInstance (GameCenterLeaderboardSetV2CreateRequest gameCenterLeaderboardSetV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetV2CreateRequest** | [**GameCenterLeaderboardSetV2CreateRequest**](GameCenterLeaderboardSetV2CreateRequest.md) | GameCenterLeaderboardSet representation |  |

### Return type

[**GameCenterLeaderboardSetV2Response**](GameCenterLeaderboardSetV2Response.md)

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
| **201** | Single GameCenterLeaderboardSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsv2deleteinstance"></a>
# **GameCenterLeaderboardSetsV2DeleteInstance**
> void GameCenterLeaderboardSetsV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardscreatetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsdeletetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsV2Response GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated (string id, List<string> filterReferenceName = null, List<string> filterArchived = null, List<string> filterId = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterLeaderboardVersions = null, int limit = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitVersions = null)




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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship**
> GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse**](GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse.md)

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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest** | [**GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterleaderboardsetsv2getinstance"></a>
# **GameCenterLeaderboardSetsV2GetInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardSetVersions = null, List<string> include = null, int limitGameCenterLeaderboards = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetV2Response**](GameCenterLeaderboardSetV2Response.md)

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
| **200** | Single GameCenterLeaderboardSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsv2updateinstance"></a>
# **GameCenterLeaderboardSetsV2UpdateInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2UpdateInstance (string id, GameCenterLeaderboardSetV2UpdateRequest gameCenterLeaderboardSetV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetV2UpdateRequest** | [**GameCenterLeaderboardSetV2UpdateRequest**](GameCenterLeaderboardSetV2UpdateRequest.md) | GameCenterLeaderboardSet representation |  |

### Return type

[**GameCenterLeaderboardSetV2Response**](GameCenterLeaderboardSetV2Response.md)

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
| **200** | Single GameCenterLeaderboardSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsv2versionsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsV2VersionsGetToManyRelated**
> GameCenterLeaderboardSetVersionsV2Response GameCenterLeaderboardSetsV2VersionsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardSetVersions = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardSetLocalizations = null, int limit = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardSetVersionsV2Response**](GameCenterLeaderboardSetVersionsV2Response.md)

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
| **200** | List of GameCenterLeaderboardSetVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsetsv2versionsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2VersionsGetToManyRelationship**
> GameCenterLeaderboardSetV2VersionsLinkagesResponse GameCenterLeaderboardSetsV2VersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardSetV2VersionsLinkagesResponse**](GameCenterLeaderboardSetV2VersionsLinkagesResponse.md)

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

