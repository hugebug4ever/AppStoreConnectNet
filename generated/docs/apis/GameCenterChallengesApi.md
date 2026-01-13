# AppStoreConnect.Net.Api.GameCenterChallengesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterChallengesCreateInstance**](GameCenterChallengesApi.md#gamecenterchallengescreateinstance) | **POST** /v1/gameCenterChallenges |  |
| [**GameCenterChallengesDeleteInstance**](GameCenterChallengesApi.md#gamecenterchallengesdeleteinstance) | **DELETE** /v1/gameCenterChallenges/{id} |  |
| [**GameCenterChallengesGetInstance**](GameCenterChallengesApi.md#gamecenterchallengesgetinstance) | **GET** /v1/gameCenterChallenges/{id} |  |
| [**GameCenterChallengesLeaderboardUpdateToOneRelationship**](GameCenterChallengesApi.md#gamecenterchallengesleaderboardupdatetoonerelationship) | **PATCH** /v1/gameCenterChallenges/{id}/relationships/leaderboard |  |
| [**GameCenterChallengesLeaderboardV2UpdateToOneRelationship**](GameCenterChallengesApi.md#gamecenterchallengesleaderboardv2updatetoonerelationship) | **PATCH** /v1/gameCenterChallenges/{id}/relationships/leaderboardV2 |  |
| [**GameCenterChallengesUpdateInstance**](GameCenterChallengesApi.md#gamecenterchallengesupdateinstance) | **PATCH** /v1/gameCenterChallenges/{id} |  |
| [**GameCenterChallengesVersionsGetToManyRelated**](GameCenterChallengesApi.md#gamecenterchallengesversionsgettomanyrelated) | **GET** /v1/gameCenterChallenges/{id}/versions |  |
| [**GameCenterChallengesVersionsGetToManyRelationship**](GameCenterChallengesApi.md#gamecenterchallengesversionsgettomanyrelationship) | **GET** /v1/gameCenterChallenges/{id}/relationships/versions |  |

<a id="gamecenterchallengescreateinstance"></a>
# **GameCenterChallengesCreateInstance**
> GameCenterChallengeResponse GameCenterChallengesCreateInstance (GameCenterChallengeCreateRequest gameCenterChallengeCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterChallengeCreateRequest** | [**GameCenterChallengeCreateRequest**](GameCenterChallengeCreateRequest.md) | GameCenterChallenge representation |  |

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
| **201** | Single GameCenterChallenge |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengesdeleteinstance"></a>
# **GameCenterChallengesDeleteInstance**
> void GameCenterChallengesDeleteInstance (string id)




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

<a id="gamecenterchallengesgetinstance"></a>
# **GameCenterChallengesGetInstance**
> GameCenterChallengeResponse GameCenterChallengesGetInstance (string id, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterChallengeVersions = null, List<string> include = null, int limitVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int** | maximum number of related versions returned (when they are included) | [optional]  |

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
| **200** | Single GameCenterChallenge |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengesleaderboardupdatetoonerelationship"></a>
# **GameCenterChallengesLeaderboardUpdateToOneRelationship**
> void GameCenterChallengesLeaderboardUpdateToOneRelationship (string id, GameCenterChallengeLeaderboardLinkageRequest gameCenterChallengeLeaderboardLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeLeaderboardLinkageRequest** | [**GameCenterChallengeLeaderboardLinkageRequest**](GameCenterChallengeLeaderboardLinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterchallengesleaderboardv2updatetoonerelationship"></a>
# **GameCenterChallengesLeaderboardV2UpdateToOneRelationship**
> void GameCenterChallengesLeaderboardV2UpdateToOneRelationship (string id, GameCenterChallengeLeaderboardV2LinkageRequest gameCenterChallengeLeaderboardV2LinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeLeaderboardV2LinkageRequest** | [**GameCenterChallengeLeaderboardV2LinkageRequest**](GameCenterChallengeLeaderboardV2LinkageRequest.md) | Related linkage |  |

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

<a id="gamecenterchallengesupdateinstance"></a>
# **GameCenterChallengesUpdateInstance**
> GameCenterChallengeResponse GameCenterChallengesUpdateInstance (string id, GameCenterChallengeUpdateRequest gameCenterChallengeUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterChallengeUpdateRequest** | [**GameCenterChallengeUpdateRequest**](GameCenterChallengeUpdateRequest.md) | GameCenterChallenge representation |  |

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
| **200** | Single GameCenterChallenge |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengesversionsgettomanyrelated"></a>
# **GameCenterChallengesVersionsGetToManyRelated**
> GameCenterChallengeVersionsResponse GameCenterChallengesVersionsGetToManyRelated (string id, List<string> fieldsGameCenterChallengeVersions = null, List<string> fieldsGameCenterChallenges = null, List<string> fieldsGameCenterChallengeLocalizations = null, List<string> fieldsGameCenterChallengeVersionReleases = null, List<string> fieldsGameCenterChallengeImages = null, int limit = null, List<string> include = null, int limitLocalizations = null, int limitReleases = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int** | maximum number of related releases returned (when they are included) | [optional]  |

### Return type

[**GameCenterChallengeVersionsResponse**](GameCenterChallengeVersionsResponse.md)

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
| **200** | List of GameCenterChallengeVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterchallengesversionsgettomanyrelationship"></a>
# **GameCenterChallengesVersionsGetToManyRelationship**
> GameCenterChallengeVersionsLinkagesResponse GameCenterChallengesVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterChallengeVersionsLinkagesResponse**](GameCenterChallengeVersionsLinkagesResponse.md)

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

