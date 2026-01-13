# AppStoreConnect.Net.Api.GameCenterLeaderboardsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardsActivityUpdateToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsactivityupdatetoonerelationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/activity |  |
| [**GameCenterLeaderboardsChallengeUpdateToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardschallengeupdatetoonerelationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/challenge |  |
| [**GameCenterLeaderboardsCreateInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardscreateinstance) | **POST** /v1/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardsDeleteInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsGetInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsgetinstance) | **GET** /v1/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsGroupLeaderboardGetToOneRelated**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsgroupleaderboardgettoonerelated) | **GET** /v1/gameCenterLeaderboards/{id}/groupLeaderboard |  |
| [**GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsgroupleaderboardgettoonerelationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard |  |
| [**GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsgroupleaderboardupdatetoonerelationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard |  |
| [**GameCenterLeaderboardsLocalizationsGetToManyRelated**](GameCenterLeaderboardsApi.md#gamecenterleaderboardslocalizationsgettomanyrelated) | **GET** /v1/gameCenterLeaderboards/{id}/localizations |  |
| [**GameCenterLeaderboardsLocalizationsGetToManyRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardslocalizationsgettomanyrelationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/localizations |  |
| [**GameCenterLeaderboardsReleasesGetToManyRelated**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsreleasesgettomanyrelated) | **GET** /v1/gameCenterLeaderboards/{id}/releases |  |
| [**GameCenterLeaderboardsReleasesGetToManyRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsreleasesgettomanyrelationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/releases |  |
| [**GameCenterLeaderboardsUpdateInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsupdateinstance) | **PATCH** /v1/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsV2ActivityUpdateToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2activityupdatetoonerelationship) | **PATCH** /v2/gameCenterLeaderboards/{id}/relationships/activity |  |
| [**GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2challengeupdatetoonerelationship) | **PATCH** /v2/gameCenterLeaderboards/{id}/relationships/challenge |  |
| [**GameCenterLeaderboardsV2CreateInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2createinstance) | **POST** /v2/gameCenterLeaderboards |  |
| [**GameCenterLeaderboardsV2DeleteInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2deleteinstance) | **DELETE** /v2/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsV2GetInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2getinstance) | **GET** /v2/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsV2UpdateInstance**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2updateinstance) | **PATCH** /v2/gameCenterLeaderboards/{id} |  |
| [**GameCenterLeaderboardsV2VersionsGetToManyRelated**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2versionsgettomanyrelated) | **GET** /v2/gameCenterLeaderboards/{id}/versions |  |
| [**GameCenterLeaderboardsV2VersionsGetToManyRelationship**](GameCenterLeaderboardsApi.md#gamecenterleaderboardsv2versionsgettomanyrelationship) | **GET** /v2/gameCenterLeaderboards/{id}/relationships/versions |  |

<a id="gamecenterleaderboardsactivityupdatetoonerelationship"></a>
# **GameCenterLeaderboardsActivityUpdateToOneRelationship**
> void GameCenterLeaderboardsActivityUpdateToOneRelationship (string id, GameCenterLeaderboardActivityLinkageRequest gameCenterLeaderboardActivityLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardActivityLinkageRequest** | [**GameCenterLeaderboardActivityLinkageRequest**](GameCenterLeaderboardActivityLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardschallengeupdatetoonerelationship"></a>
# **GameCenterLeaderboardsChallengeUpdateToOneRelationship**
> void GameCenterLeaderboardsChallengeUpdateToOneRelationship (string id, GameCenterLeaderboardChallengeLinkageRequest gameCenterLeaderboardChallengeLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardChallengeLinkageRequest** | [**GameCenterLeaderboardChallengeLinkageRequest**](GameCenterLeaderboardChallengeLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardscreateinstance"></a>
# **GameCenterLeaderboardsCreateInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsCreateInstance (GameCenterLeaderboardCreateRequest gameCenterLeaderboardCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardCreateRequest** | [**GameCenterLeaderboardCreateRequest**](GameCenterLeaderboardCreateRequest.md) | GameCenterLeaderboard representation |  |

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
| **201** | Single GameCenterLeaderboard |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsdeleteinstance"></a>
# **GameCenterLeaderboardsDeleteInstance**
> void GameCenterLeaderboardsDeleteInstance (string id)




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

<a id="gamecenterleaderboardsgetinstance"></a>
# **GameCenterLeaderboardsGetInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsGetInstance (string id, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
| **200** | Single GameCenterLeaderboard |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsgroupleaderboardgettoonerelated"></a>
# **GameCenterLeaderboardsGroupLeaderboardGetToOneRelated**
> GameCenterLeaderboardResponse GameCenterLeaderboardsGroupLeaderboardGetToOneRelated (string id, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterGroups = null, List<string> fieldsGameCenterLeaderboardSets = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> fieldsGameCenterActivities = null, List<string> fieldsGameCenterChallenges = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
| **200** | Single GameCenterLeaderboard |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsgroupleaderboardgettoonerelationship"></a>
# **GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship**
> GameCenterLeaderboardGroupLeaderboardLinkageResponse GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardGroupLeaderboardLinkageResponse**](GameCenterLeaderboardGroupLeaderboardLinkageResponse.md)

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

<a id="gamecenterleaderboardsgroupleaderboardupdatetoonerelationship"></a>
# **GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship**
> void GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship (string id, GameCenterLeaderboardGroupLeaderboardLinkageRequest gameCenterLeaderboardGroupLeaderboardLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardGroupLeaderboardLinkageRequest** | [**GameCenterLeaderboardGroupLeaderboardLinkageRequest**](GameCenterLeaderboardGroupLeaderboardLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardslocalizationsgettomanyrelated"></a>
# **GameCenterLeaderboardsLocalizationsGetToManyRelated**
> GameCenterLeaderboardLocalizationsResponse GameCenterLeaderboardsLocalizationsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardLocalizations = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardImages = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationsResponse**](GameCenterLeaderboardLocalizationsResponse.md)

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
| **200** | List of GameCenterLeaderboardLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardslocalizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardsLocalizationsGetToManyRelationship**
> GameCenterLeaderboardLocalizationsLinkagesResponse GameCenterLeaderboardsLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardLocalizationsLinkagesResponse**](GameCenterLeaderboardLocalizationsLinkagesResponse.md)

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

<a id="gamecenterleaderboardsreleasesgettomanyrelated"></a>
# **GameCenterLeaderboardsReleasesGetToManyRelated**
> GameCenterLeaderboardReleasesResponse GameCenterLeaderboardsReleasesGetToManyRelated (string id, List<string> filterLive = null, List<string> filterGameCenterDetail = null, List<string> fieldsGameCenterLeaderboardReleases = null, List<string> fieldsGameCenterDetails = null, List<string> fieldsGameCenterLeaderboards = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLive** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;live&#39; | [optional]  |
| **filterGameCenterDetail** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterDetail&#39; | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardReleasesResponse**](GameCenterLeaderboardReleasesResponse.md)

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
| **200** | List of GameCenterLeaderboardReleases |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsreleasesgettomanyrelationship"></a>
# **GameCenterLeaderboardsReleasesGetToManyRelationship**
> GameCenterLeaderboardReleasesLinkagesResponse GameCenterLeaderboardsReleasesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardReleasesLinkagesResponse**](GameCenterLeaderboardReleasesLinkagesResponse.md)

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

<a id="gamecenterleaderboardsupdateinstance"></a>
# **GameCenterLeaderboardsUpdateInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsUpdateInstance (string id, GameCenterLeaderboardUpdateRequest gameCenterLeaderboardUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardUpdateRequest** | [**GameCenterLeaderboardUpdateRequest**](GameCenterLeaderboardUpdateRequest.md) | GameCenterLeaderboard representation |  |

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
| **200** | Single GameCenterLeaderboard |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsv2activityupdatetoonerelationship"></a>
# **GameCenterLeaderboardsV2ActivityUpdateToOneRelationship**
> void GameCenterLeaderboardsV2ActivityUpdateToOneRelationship (string id, GameCenterLeaderboardV2ActivityLinkageRequest gameCenterLeaderboardV2ActivityLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardV2ActivityLinkageRequest** | [**GameCenterLeaderboardV2ActivityLinkageRequest**](GameCenterLeaderboardV2ActivityLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardsv2challengeupdatetoonerelationship"></a>
# **GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship**
> void GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship (string id, GameCenterLeaderboardV2ChallengeLinkageRequest gameCenterLeaderboardV2ChallengeLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardV2ChallengeLinkageRequest** | [**GameCenterLeaderboardV2ChallengeLinkageRequest**](GameCenterLeaderboardV2ChallengeLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterleaderboardsv2createinstance"></a>
# **GameCenterLeaderboardsV2CreateInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2CreateInstance (GameCenterLeaderboardV2CreateRequest gameCenterLeaderboardV2CreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardV2CreateRequest** | [**GameCenterLeaderboardV2CreateRequest**](GameCenterLeaderboardV2CreateRequest.md) | GameCenterLeaderboard representation |  |

### Return type

[**GameCenterLeaderboardV2Response**](GameCenterLeaderboardV2Response.md)

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
| **201** | Single GameCenterLeaderboard |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsv2deleteinstance"></a>
# **GameCenterLeaderboardsV2DeleteInstance**
> void GameCenterLeaderboardsV2DeleteInstance (string id)




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

<a id="gamecenterleaderboardsv2getinstance"></a>
# **GameCenterLeaderboardsV2GetInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2GetInstance (string id, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardVersions = null, List<string> include = null, int limitGameCenterLeaderboardSets = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardV2Response**](GameCenterLeaderboardV2Response.md)

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
| **200** | Single GameCenterLeaderboard |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsv2updateinstance"></a>
# **GameCenterLeaderboardsV2UpdateInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2UpdateInstance (string id, GameCenterLeaderboardV2UpdateRequest gameCenterLeaderboardV2UpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardV2UpdateRequest** | [**GameCenterLeaderboardV2UpdateRequest**](GameCenterLeaderboardV2UpdateRequest.md) | GameCenterLeaderboard representation |  |

### Return type

[**GameCenterLeaderboardV2Response**](GameCenterLeaderboardV2Response.md)

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
| **200** | Single GameCenterLeaderboard |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsv2versionsgettomanyrelated"></a>
# **GameCenterLeaderboardsV2VersionsGetToManyRelated**
> GameCenterLeaderboardVersionsV2Response GameCenterLeaderboardsV2VersionsGetToManyRelated (string id, List<string> fieldsGameCenterLeaderboardVersions = null, List<string> fieldsGameCenterLeaderboards = null, List<string> fieldsGameCenterLeaderboardLocalizations = null, int limit = null, List<string> include = null, int limitLocalizations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**GameCenterLeaderboardVersionsV2Response**](GameCenterLeaderboardVersionsV2Response.md)

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
| **200** | List of GameCenterLeaderboardVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterleaderboardsv2versionsgettomanyrelationship"></a>
# **GameCenterLeaderboardsV2VersionsGetToManyRelationship**
> GameCenterLeaderboardV2VersionsLinkagesResponse GameCenterLeaderboardsV2VersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterLeaderboardV2VersionsLinkagesResponse**](GameCenterLeaderboardV2VersionsLinkagesResponse.md)

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

