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



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsCreateInstanceExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var gameCenterGroupCreateRequest = new GameCenterGroupCreateRequest(); // GameCenterGroupCreateRequest | GameCenterGroup representation

            try
            {
                GameCenterGroupResponse result = apiInstance.GameCenterGroupsCreateInstance(gameCenterGroupCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupResponse> response = apiInstance.GameCenterGroupsCreateInstanceWithHttpInfo(gameCenterGroupCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsdeleteinstance"></a>
# **GameCenterGroupsDeleteInstance**
> void GameCenterGroupsDeleteInstance (string id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsDeleteInstanceExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterGroupsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsDeleteInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterAchievementsGetToManyRelated**
> GameCenterAchievementsResponse GameCenterGroupsGameCenterAchievementsGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterAchievementLocalizations = null, List<string>? fieldsGameCenterAchievementReleases = null, List<string>? fieldsGameCenterActivities = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null, int? limitReleases = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterArchived = new List<string>?(); // List<string>? | filter by attribute 'archived' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterAchievementLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional) 
            var fieldsGameCenterAchievementReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementReleases (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterAchievementsResponse result = apiInstance.GameCenterGroupsGameCenterAchievementsGetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementReleases, fieldsGameCenterActivities, limit, include, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementsResponse> response = apiInstance.GameCenterGroupsGameCenterAchievementsGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievementLocalizations, fieldsGameCenterAchievementReleases, fieldsGameCenterActivities, limit, include, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievementLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsGetToManyRelationship**
> GameCenterGroupGameCenterAchievementsLinkagesResponse GameCenterGroupsGameCenterAchievementsGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterAchievementsLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterAchievementsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterAchievementsLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterAchievementsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship (string id, GameCenterGroupGameCenterAchievementsLinkagesRequest gameCenterGroupGameCenterAchievementsLinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterAchievementsLinkagesRequest = new GameCenterGroupGameCenterAchievementsLinkagesRequest(); // GameCenterGroupGameCenterAchievementsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship(id, gameCenterGroupGameCenterAchievementsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterAchievementsReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterAchievementsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterAchievementsV2GetToManyRelated**
> GameCenterAchievementsV2Response GameCenterGroupsGameCenterAchievementsV2GetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterAchievementVersions = null, int? limit = null, List<string>? include = null, int? limitVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsV2GetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterArchived = new List<string>?(); // List<string>? | filter by attribute 'archived' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterAchievementVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterAchievementsV2Response result = apiInstance.GameCenterGroupsGameCenterAchievementsV2GetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterActivities, fieldsGameCenterAchievementVersions, limit, include, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2GetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsV2GetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAchievementsV2Response> response = apiInstance.GameCenterGroupsGameCenterAchievementsV2GetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterAchievements, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterActivities, fieldsGameCenterAchievementVersions, limit, include, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2GetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship**
> GameCenterGroupGameCenterAchievementsV2LinkagesResponse GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsV2GetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterAchievementsV2LinkagesResponse result = apiInstance.GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2GetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsV2GetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterAchievementsV2LinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterAchievementsV2GetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2GetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterachievementsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterAchievementsV2LinkagesRequest gameCenterGroupGameCenterAchievementsV2LinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterAchievementsV2LinkagesRequest = new GameCenterGroupGameCenterAchievementsV2LinkagesRequest(); // GameCenterGroupGameCenterAchievementsV2LinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship(id, gameCenterGroupGameCenterAchievementsV2LinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterAchievementsV2LinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterAchievementsV2ReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenteractivitiesgettomanyrelated"></a>
# **GameCenterGroupsGameCenterActivitiesGetToManyRelated**
> GameCenterActivitiesResponse GameCenterGroupsGameCenterActivitiesGetToManyRelated (string id, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterActivityVersions = null, int? limit = null, List<string>? include = null, int? limitAchievements = null, int? limitAchievementsV2 = null, int? limitLeaderboards = null, int? limitLeaderboardsV2 = null, int? limitVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterActivitiesGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterActivityVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAchievements = 56;  // int? | maximum number of related achievements returned (when they are included) (optional) 
            var limitAchievementsV2 = 56;  // int? | maximum number of related achievementsV2 returned (when they are included) (optional) 
            var limitLeaderboards = 56;  // int? | maximum number of related leaderboards returned (when they are included) (optional) 
            var limitLeaderboardsV2 = 56;  // int? | maximum number of related leaderboardsV2 returned (when they are included) (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterActivitiesResponse result = apiInstance.GameCenterGroupsGameCenterActivitiesGetToManyRelated(id, fieldsGameCenterActivities, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievements, fieldsGameCenterLeaderboards, fieldsGameCenterActivityVersions, limit, include, limitAchievements, limitAchievementsV2, limitLeaderboards, limitLeaderboardsV2, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterActivitiesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterActivitiesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterActivitiesResponse> response = apiInstance.GameCenterGroupsGameCenterActivitiesGetToManyRelatedWithHttpInfo(id, fieldsGameCenterActivities, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterAchievements, fieldsGameCenterLeaderboards, fieldsGameCenterActivityVersions, limit, include, limitAchievements, limitAchievementsV2, limitLeaderboards, limitLeaderboardsV2, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterActivitiesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAchievements** | **int?** | maximum number of related achievements returned (when they are included) | [optional]  |
| **limitAchievementsV2** | **int?** | maximum number of related achievementsV2 returned (when they are included) | [optional]  |
| **limitLeaderboards** | **int?** | maximum number of related leaderboards returned (when they are included) | [optional]  |
| **limitLeaderboardsV2** | **int?** | maximum number of related leaderboardsV2 returned (when they are included) | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenteractivitiesgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterActivitiesGetToManyRelationship**
> GameCenterGroupGameCenterActivitiesLinkagesResponse GameCenterGroupsGameCenterActivitiesGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterActivitiesGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterActivitiesLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterActivitiesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterActivitiesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterActivitiesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterActivitiesLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterActivitiesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterActivitiesGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterchallengesgettomanyrelated"></a>
# **GameCenterGroupsGameCenterChallengesGetToManyRelated**
> GameCenterChallengesResponse GameCenterGroupsGameCenterChallengesGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterChallengeVersions = null, List<string>? fieldsGameCenterLeaderboards = null, int? limit = null, List<string>? include = null, int? limitVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterChallengesGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterArchived = new List<string>?(); // List<string>? | filter by attribute 'archived' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterChallengeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersions (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterChallengesResponse result = apiInstance.GameCenterGroupsGameCenterChallengesGetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterChallenges, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterChallengeVersions, fieldsGameCenterLeaderboards, limit, include, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterChallengesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterChallengesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengesResponse> response = apiInstance.GameCenterGroupsGameCenterChallengesGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterChallenges, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterChallengeVersions, fieldsGameCenterLeaderboards, limit, include, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterChallengesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterchallengesgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterChallengesGetToManyRelationship**
> GameCenterGroupGameCenterChallengesLinkagesResponse GameCenterGroupsGameCenterChallengesGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterChallengesGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterChallengesLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterChallengesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterChallengesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterChallengesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterChallengesLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterChallengesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterChallengesGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterdetailsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterDetailsGetToManyRelated**
> GameCenterDetailsResponse GameCenterGroupsGameCenterDetailsGetToManyRelated (string id, List<string>? filterGameCenterAppVersionsEnabled = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsApps = null, List<string>? fieldsGameCenterAppVersions = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterAchievementReleases = null, List<string>? fieldsGameCenterActivityVersionReleases = null, List<string>? fieldsGameCenterChallengeVersionReleases = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? fieldsAppStoreVersions = null, int? limit = null, List<string>? include = null, int? limitGameCenterAppVersions = null, int? limitGameCenterLeaderboards = null, int? limitGameCenterLeaderboardsV2 = null, int? limitGameCenterLeaderboardSets = null, int? limitGameCenterLeaderboardSetsV2 = null, int? limitGameCenterAchievements = null, int? limitGameCenterAchievementsV2 = null, int? limitGameCenterActivities = null, int? limitGameCenterChallenges = null, int? limitAchievementReleases = null, int? limitActivityReleases = null, int? limitChallengeReleases = null, int? limitLeaderboardReleases = null, int? limitLeaderboardSetReleases = null, int? limitChallengesMinimumPlatformVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterDetailsGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterGameCenterAppVersionsEnabled = new List<string>?(); // List<string>? | filter by attribute 'gameCenterAppVersions.enabled' (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsGameCenterAppVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAppVersions (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var fieldsGameCenterAchievementReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievementReleases (optional) 
            var fieldsGameCenterActivityVersionReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivityVersionReleases (optional) 
            var fieldsGameCenterChallengeVersionReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional) 
            var fieldsGameCenterLeaderboardReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional) 
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterAppVersions = 56;  // int? | maximum number of related gameCenterAppVersions returned (when they are included) (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitGameCenterLeaderboardsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSetsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) (optional) 
            var limitGameCenterAchievements = 56;  // int? | maximum number of related gameCenterAchievements returned (when they are included) (optional) 
            var limitGameCenterAchievementsV2 = 56;  // int? | maximum number of related gameCenterAchievementsV2 returned (when they are included) (optional) 
            var limitGameCenterActivities = 56;  // int? | maximum number of related gameCenterActivities returned (when they are included) (optional) 
            var limitGameCenterChallenges = 56;  // int? | maximum number of related gameCenterChallenges returned (when they are included) (optional) 
            var limitAchievementReleases = 56;  // int? | maximum number of related achievementReleases returned (when they are included) (optional) 
            var limitActivityReleases = 56;  // int? | maximum number of related activityReleases returned (when they are included) (optional) 
            var limitChallengeReleases = 56;  // int? | maximum number of related challengeReleases returned (when they are included) (optional) 
            var limitLeaderboardReleases = 56;  // int? | maximum number of related leaderboardReleases returned (when they are included) (optional) 
            var limitLeaderboardSetReleases = 56;  // int? | maximum number of related leaderboardSetReleases returned (when they are included) (optional) 
            var limitChallengesMinimumPlatformVersions = 56;  // int? | maximum number of related challengesMinimumPlatformVersions returned (when they are included) (optional) 

            try
            {
                GameCenterDetailsResponse result = apiInstance.GameCenterGroupsGameCenterDetailsGetToManyRelated(id, filterGameCenterAppVersionsEnabled, fieldsGameCenterDetails, fieldsApps, fieldsGameCenterAppVersions, fieldsGameCenterGroups, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterAchievementReleases, fieldsGameCenterActivityVersionReleases, fieldsGameCenterChallengeVersionReleases, fieldsGameCenterLeaderboardReleases, fieldsGameCenterLeaderboardSetReleases, fieldsAppStoreVersions, limit, include, limitGameCenterAppVersions, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitAchievementReleases, limitActivityReleases, limitChallengeReleases, limitLeaderboardReleases, limitLeaderboardSetReleases, limitChallengesMinimumPlatformVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterDetailsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterDetailsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterDetailsResponse> response = apiInstance.GameCenterGroupsGameCenterDetailsGetToManyRelatedWithHttpInfo(id, filterGameCenterAppVersionsEnabled, fieldsGameCenterDetails, fieldsApps, fieldsGameCenterAppVersions, fieldsGameCenterGroups, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterAchievementReleases, fieldsGameCenterActivityVersionReleases, fieldsGameCenterChallengeVersionReleases, fieldsGameCenterLeaderboardReleases, fieldsGameCenterLeaderboardSetReleases, fieldsAppStoreVersions, limit, include, limitGameCenterAppVersions, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitAchievementReleases, limitActivityReleases, limitChallengeReleases, limitLeaderboardReleases, limitLeaderboardSetReleases, limitChallengesMinimumPlatformVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterDetailsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterGameCenterAppVersionsEnabled** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;gameCenterAppVersions.enabled&#39; | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterAchievementReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievementReleases | [optional]  |
| **fieldsGameCenterActivityVersionReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional]  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAppVersions** | **int?** | maximum number of related gameCenterAppVersions returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int?** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int?** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterAchievements** | **int?** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int?** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int?** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int?** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitAchievementReleases** | **int?** | maximum number of related achievementReleases returned (when they are included) | [optional]  |
| **limitActivityReleases** | **int?** | maximum number of related activityReleases returned (when they are included) | [optional]  |
| **limitChallengeReleases** | **int?** | maximum number of related challengeReleases returned (when they are included) | [optional]  |
| **limitLeaderboardReleases** | **int?** | maximum number of related leaderboardReleases returned (when they are included) | [optional]  |
| **limitLeaderboardSetReleases** | **int?** | maximum number of related leaderboardSetReleases returned (when they are included) | [optional]  |
| **limitChallengesMinimumPlatformVersions** | **int?** | maximum number of related challengesMinimumPlatformVersions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterdetailsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterDetailsGetToManyRelationship**
> GameCenterGroupGameCenterDetailsLinkagesResponse GameCenterGroupsGameCenterDetailsGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterDetailsGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterDetailsLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterDetailsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterDetailsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterDetailsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterDetailsLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterDetailsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterDetailsGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated**
> GameCenterLeaderboardSetsResponse GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null, int? limitGameCenterLeaderboards = null, int? limitReleases = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetsResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated(id, filterReferenceName, filterId, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, limit, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetsResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterId, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, limit, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest = new GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest(); // GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship(id, gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterLeaderboardSetsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated**
> GameCenterLeaderboardSetsV2Response GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetVersions = null, int? limit = null, List<string>? include = null, int? limitGameCenterLeaderboards = null, int? limitVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetsV2Response result = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated(id, filterReferenceName, filterId, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetVersions, limit, include, limitGameCenterLeaderboards, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetsV2Response> response = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelatedWithHttpInfo(id, filterReferenceName, filterId, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetVersions, limit, include, limitGameCenterLeaderboards, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterLeaderboardSetsV2LinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2GetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsetsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest = new GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest(); // GameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship(id, gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterLeaderboardSetsV2LinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardSetsV2ReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsResponse GameCenterGroupsGameCenterLeaderboardsGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, int? limit = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitLocalizations = null, int? limitReleases = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsGetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterArchived = new List<string>?(); // List<string>? | filter by attribute 'archived' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardsResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardsGetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardsResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardsLinkagesResponse GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsGetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterLeaderboardsLinkagesResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterLeaderboardsLinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardsLinkagesRequest gameCenterGroupGameCenterLeaderboardsLinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterLeaderboardsLinkagesRequest = new GameCenterGroupGameCenterLeaderboardsLinkagesRequest(); // GameCenterGroupGameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship(id, gameCenterGroupGameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsv2gettomanyrelated"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated**
> GameCenterLeaderboardsV2Response GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterLeaderboardVersions = null, int? limit = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitVersions = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelatedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterReferenceName = new List<string>?(); // List<string>? | filter by attribute 'referenceName' (optional) 
            var filterArchived = new List<string>?(); // List<string>? | filter by attribute 'archived' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var fieldsGameCenterLeaderboardVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardsV2Response result = apiInstance.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterLeaderboardVersions, limit, include, limitGameCenterLeaderboardSets, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardsV2Response> response = apiInstance.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterLeaderboardVersions, limit, include, limitGameCenterLeaderboardSets, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterReferenceName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;referenceName&#39; | [optional]  |
| **filterArchived** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;archived&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsv2gettomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship**
> GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship (string id, int? limit = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse result = apiInstance.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupGameCenterLeaderboardsV2LinkagesResponse> response = apiInstance.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2GetToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgamecenterleaderboardsv2replacetomanyrelationship"></a>
# **GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship**
> void GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship (string id, GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationshipExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest = new GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest(); // GameCenterGroupGameCenterLeaderboardsV2LinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship(id, gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationshipWithHttpInfo(id, gameCenterGroupGameCenterLeaderboardsV2LinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGameCenterLeaderboardsV2ReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgetcollection"></a>
# **GameCenterGroupsGetCollection**
> GameCenterGroupsResponse GameCenterGroupsGetCollection (List<string>? filterGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, int? limit = null, List<string>? include = null, int? limitGameCenterAchievements = null, int? limitGameCenterAchievementsV2 = null, int? limitGameCenterActivities = null, int? limitGameCenterChallenges = null, int? limitGameCenterDetails = null, int? limitGameCenterLeaderboardSets = null, int? limitGameCenterLeaderboardSetsV2 = null, int? limitGameCenterLeaderboards = null, int? limitGameCenterLeaderboardsV2 = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGetCollectionExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var filterGameCenterDetails = new List<string>?(); // List<string>? | filter by id(s) of related 'gameCenterDetails' (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterAchievements = 56;  // int? | maximum number of related gameCenterAchievements returned (when they are included) (optional) 
            var limitGameCenterAchievementsV2 = 56;  // int? | maximum number of related gameCenterAchievementsV2 returned (when they are included) (optional) 
            var limitGameCenterActivities = 56;  // int? | maximum number of related gameCenterActivities returned (when they are included) (optional) 
            var limitGameCenterChallenges = 56;  // int? | maximum number of related gameCenterChallenges returned (when they are included) (optional) 
            var limitGameCenterDetails = 56;  // int? | maximum number of related gameCenterDetails returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSetsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitGameCenterLeaderboardsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) (optional) 

            try
            {
                GameCenterGroupsResponse result = apiInstance.GameCenterGroupsGetCollection(filterGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitGameCenterDetails, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupsResponse> response = apiInstance.GameCenterGroupsGetCollectionWithHttpInfo(filterGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitGameCenterDetails, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;gameCenterDetails&#39; | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAchievements** | **int?** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int?** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int?** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int?** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitGameCenterDetails** | **int?** | maximum number of related gameCenterDetails returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int?** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int?** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsgetinstance"></a>
# **GameCenterGroupsGetInstance**
> GameCenterGroupResponse GameCenterGroupsGetInstance (string id, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterAchievements = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? include = null, int? limitGameCenterAchievements = null, int? limitGameCenterAchievementsV2 = null, int? limitGameCenterActivities = null, int? limitGameCenterChallenges = null, int? limitGameCenterDetails = null, int? limitGameCenterLeaderboardSets = null, int? limitGameCenterLeaderboardSetsV2 = null, int? limitGameCenterLeaderboards = null, int? limitGameCenterLeaderboardsV2 = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsGetInstanceExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterAchievements = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAchievements (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterAchievements = 56;  // int? | maximum number of related gameCenterAchievements returned (when they are included) (optional) 
            var limitGameCenterAchievementsV2 = 56;  // int? | maximum number of related gameCenterAchievementsV2 returned (when they are included) (optional) 
            var limitGameCenterActivities = 56;  // int? | maximum number of related gameCenterActivities returned (when they are included) (optional) 
            var limitGameCenterChallenges = 56;  // int? | maximum number of related gameCenterChallenges returned (when they are included) (optional) 
            var limitGameCenterDetails = 56;  // int? | maximum number of related gameCenterDetails returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitGameCenterLeaderboardSetsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitGameCenterLeaderboardsV2 = 56;  // int? | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) (optional) 

            try
            {
                GameCenterGroupResponse result = apiInstance.GameCenterGroupsGetInstance(id, fieldsGameCenterGroups, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitGameCenterDetails, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupResponse> response = apiInstance.GameCenterGroupsGetInstanceWithHttpInfo(id, fieldsGameCenterGroups, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSets, fieldsGameCenterAchievements, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterAchievements, limitGameCenterAchievementsV2, limitGameCenterActivities, limitGameCenterChallenges, limitGameCenterDetails, limitGameCenterLeaderboardSets, limitGameCenterLeaderboardSetsV2, limitGameCenterLeaderboards, limitGameCenterLeaderboardsV2);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterAchievements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAchievements | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterAchievements** | **int?** | maximum number of related gameCenterAchievements returned (when they are included) | [optional]  |
| **limitGameCenterAchievementsV2** | **int?** | maximum number of related gameCenterAchievementsV2 returned (when they are included) | [optional]  |
| **limitGameCenterActivities** | **int?** | maximum number of related gameCenterActivities returned (when they are included) | [optional]  |
| **limitGameCenterChallenges** | **int?** | maximum number of related gameCenterChallenges returned (when they are included) | [optional]  |
| **limitGameCenterDetails** | **int?** | maximum number of related gameCenterDetails returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardSetsV2** | **int?** | maximum number of related gameCenterLeaderboardSetsV2 returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboardsV2** | **int?** | maximum number of related gameCenterLeaderboardsV2 returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentergroupsupdateinstance"></a>
# **GameCenterGroupsUpdateInstance**
> GameCenterGroupResponse GameCenterGroupsUpdateInstance (string id, GameCenterGroupUpdateRequest gameCenterGroupUpdateRequest)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using AppStoreConnect.Net.Api;
using AppStoreConnect.Net.Client;
using AppStoreConnect.Net.Model;

namespace Example
{
    public class GameCenterGroupsUpdateInstanceExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.appstoreconnect.apple.com";
            // Configure Bearer token for authorization: itc-bearer-token
            config.AccessToken = "YOUR_BEARER_TOKEN";

            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new GameCenterGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterGroupUpdateRequest = new GameCenterGroupUpdateRequest(); // GameCenterGroupUpdateRequest | GameCenterGroup representation

            try
            {
                GameCenterGroupResponse result = apiInstance.GameCenterGroupsUpdateInstance(id, gameCenterGroupUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterGroupsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterGroupResponse> response = apiInstance.GameCenterGroupsUpdateInstanceWithHttpInfo(id, gameCenterGroupUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterGroupsApi.GameCenterGroupsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

