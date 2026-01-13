# AppStoreConnect.Net.Api.GameCenterMatchmakingRuleSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterMatchmakingRuleSetsCreateInstance**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetscreateinstance) | **POST** /v1/gameCenterMatchmakingRuleSets |  |
| [**GameCenterMatchmakingRuleSetsDeleteInstance**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsdeleteinstance) | **DELETE** /v1/gameCenterMatchmakingRuleSets/{id} |  |
| [**GameCenterMatchmakingRuleSetsGetCollection**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsgetcollection) | **GET** /v1/gameCenterMatchmakingRuleSets |  |
| [**GameCenterMatchmakingRuleSetsGetInstance**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsgetinstance) | **GET** /v1/gameCenterMatchmakingRuleSets/{id} |  |
| [**GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelated) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/matchmakingQueues |  |
| [**GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/matchmakingQueues |  |
| [**GameCenterMatchmakingRuleSetsRulesGetToManyRelated**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsrulesgettomanyrelated) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/rules |  |
| [**GameCenterMatchmakingRuleSetsRulesGetToManyRelationship**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsrulesgettomanyrelationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/rules |  |
| [**GameCenterMatchmakingRuleSetsTeamsGetToManyRelated**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsteamsgettomanyrelated) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/teams |  |
| [**GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsteamsgettomanyrelationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/teams |  |
| [**GameCenterMatchmakingRuleSetsUpdateInstance**](GameCenterMatchmakingRuleSetsApi.md#gamecentermatchmakingrulesetsupdateinstance) | **PATCH** /v1/gameCenterMatchmakingRuleSets/{id} |  |

<a id="gamecentermatchmakingrulesetscreateinstance"></a>
# **GameCenterMatchmakingRuleSetsCreateInstance**
> GameCenterMatchmakingRuleSetResponse GameCenterMatchmakingRuleSetsCreateInstance (GameCenterMatchmakingRuleSetCreateRequest gameCenterMatchmakingRuleSetCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterMatchmakingRuleSetCreateRequest** | [**GameCenterMatchmakingRuleSetCreateRequest**](GameCenterMatchmakingRuleSetCreateRequest.md) | GameCenterMatchmakingRuleSet representation |  |

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
| **201** | Single GameCenterMatchmakingRuleSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsdeleteinstance"></a>
# **GameCenterMatchmakingRuleSetsDeleteInstance**
> void GameCenterMatchmakingRuleSetsDeleteInstance (string id)




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

<a id="gamecentermatchmakingrulesetsgetcollection"></a>
# **GameCenterMatchmakingRuleSetsGetCollection**
> GameCenterMatchmakingRuleSetsResponse GameCenterMatchmakingRuleSetsGetCollection (List<string> fieldsGameCenterMatchmakingRuleSets = null, List<string> fieldsGameCenterMatchmakingTeams = null, List<string> fieldsGameCenterMatchmakingRules = null, List<string> fieldsGameCenterMatchmakingQueues = null, int limit = null, List<string> include = null, int limitMatchmakingQueues = null, int limitRules = null, int limitTeams = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMatchmakingQueues** | **int** | maximum number of related matchmakingQueues returned (when they are included) | [optional]  |
| **limitRules** | **int** | maximum number of related rules returned (when they are included) | [optional]  |
| **limitTeams** | **int** | maximum number of related teams returned (when they are included) | [optional]  |

### Return type

[**GameCenterMatchmakingRuleSetsResponse**](GameCenterMatchmakingRuleSetsResponse.md)

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
| **200** | List of GameCenterMatchmakingRuleSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsgetinstance"></a>
# **GameCenterMatchmakingRuleSetsGetInstance**
> GameCenterMatchmakingRuleSetResponse GameCenterMatchmakingRuleSetsGetInstance (string id, List<string> fieldsGameCenterMatchmakingRuleSets = null, List<string> fieldsGameCenterMatchmakingTeams = null, List<string> fieldsGameCenterMatchmakingRules = null, List<string> fieldsGameCenterMatchmakingQueues = null, List<string> include = null, int limitMatchmakingQueues = null, int limitRules = null, int limitTeams = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMatchmakingQueues** | **int** | maximum number of related matchmakingQueues returned (when they are included) | [optional]  |
| **limitRules** | **int** | maximum number of related rules returned (when they are included) | [optional]  |
| **limitTeams** | **int** | maximum number of related teams returned (when they are included) | [optional]  |

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
| **200** | Single GameCenterMatchmakingRuleSet |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated**
> GameCenterMatchmakingQueuesResponse GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated (string id, List<string> fieldsGameCenterMatchmakingQueues = null, List<string> fieldsGameCenterMatchmakingRuleSets = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterMatchmakingQueuesResponse**](GameCenterMatchmakingQueuesResponse.md)

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
| **200** | List of GameCenterMatchmakingQueues |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship**
> GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse**](GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse.md)

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

<a id="gamecentermatchmakingrulesetsrulesgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsRulesGetToManyRelated**
> GameCenterMatchmakingRulesResponse GameCenterMatchmakingRuleSetsRulesGetToManyRelated (string id, List<string> fieldsGameCenterMatchmakingRules = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterMatchmakingRulesResponse**](GameCenterMatchmakingRulesResponse.md)

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
| **200** | List of GameCenterMatchmakingRules |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsrulesgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsRulesGetToManyRelationship**
> GameCenterMatchmakingRuleSetRulesLinkagesResponse GameCenterMatchmakingRuleSetsRulesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterMatchmakingRuleSetRulesLinkagesResponse**](GameCenterMatchmakingRuleSetRulesLinkagesResponse.md)

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

<a id="gamecentermatchmakingrulesetsteamsgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsTeamsGetToManyRelated**
> GameCenterMatchmakingTeamsResponse GameCenterMatchmakingRuleSetsTeamsGetToManyRelated (string id, List<string> fieldsGameCenterMatchmakingTeams = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterMatchmakingTeamsResponse**](GameCenterMatchmakingTeamsResponse.md)

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
| **200** | List of GameCenterMatchmakingTeams |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecentermatchmakingrulesetsteamsgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship**
> GameCenterMatchmakingRuleSetTeamsLinkagesResponse GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterMatchmakingRuleSetTeamsLinkagesResponse**](GameCenterMatchmakingRuleSetTeamsLinkagesResponse.md)

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

<a id="gamecentermatchmakingrulesetsupdateinstance"></a>
# **GameCenterMatchmakingRuleSetsUpdateInstance**
> GameCenterMatchmakingRuleSetResponse GameCenterMatchmakingRuleSetsUpdateInstance (string id, GameCenterMatchmakingRuleSetUpdateRequest gameCenterMatchmakingRuleSetUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterMatchmakingRuleSetUpdateRequest** | [**GameCenterMatchmakingRuleSetUpdateRequest**](GameCenterMatchmakingRuleSetUpdateRequest.md) | GameCenterMatchmakingRuleSet representation |  |

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
| **200** | Single GameCenterMatchmakingRuleSet |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

