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
    public class GameCenterLeaderboardSetsCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetCreateRequest = new GameCenterLeaderboardSetCreateRequest(); // GameCenterLeaderboardSetCreateRequest | GameCenterLeaderboardSet representation

            try
            {
                GameCenterLeaderboardSetResponse result = apiInstance.GameCenterLeaderboardSetsCreateInstance(gameCenterLeaderboardSetCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetResponse> response = apiInstance.GameCenterLeaderboardSetsCreateInstanceWithHttpInfo(gameCenterLeaderboardSetCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsdeleteinstance"></a>
# **GameCenterLeaderboardSetsDeleteInstance**
> void GameCenterLeaderboardSetsDeleteInstance (string id)



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
    public class GameCenterLeaderboardSetsDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetsgamecenterleaderboardscreatetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgamecenterleaderboardsdeletetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsResponse GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, int? limit = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
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
                GameCenterLeaderboardsResponse result = apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardsResponse> response = apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, limit, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetsgamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship**
> GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse result = apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgetinstance"></a>
# **GameCenterLeaderboardSetsGetInstance**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsGetInstance (string id, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? include = null, int? limitGameCenterLeaderboards = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardSetsGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetResponse result = apiInstance.GameCenterLeaderboardSetsGetInstance(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitGameCenterLeaderboards, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetResponse> response = apiInstance.GameCenterLeaderboardSetsGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitGameCenterLeaderboards, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgroupleaderboardsetgettoonerelated"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? include = null, int? limitLocalizations = null, int? limitGameCenterLeaderboards = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetResponse result = apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetResponse> response = apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgroupleaderboardsetgettoonerelationship"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship**
> GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse result = apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse> response = apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsgroupleaderboardsetupdatetoonerelationship"></a>
# **GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship**
> void GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship (string id, GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest)



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
    public class GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest = new GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest(); // GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship(id, gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsGroupLeaderboardSetUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetslocalizationsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsLocalizationsGetToManyRelated**
> GameCenterLeaderboardSetLocalizationsResponse GameCenterLeaderboardSetsLocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardSetImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetsLocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboardSetImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetLocalizationsResponse result = apiInstance.GameCenterLeaderboardSetsLocalizationsGetToManyRelated(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationsResponse> response = apiInstance.GameCenterLeaderboardSetsLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetslocalizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsLocalizationsGetToManyRelationship**
> GameCenterLeaderboardSetLocalizationsLinkagesResponse GameCenterLeaderboardSetsLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetsLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetLocalizationsLinkagesResponse result = apiInstance.GameCenterLeaderboardSetsLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetLocalizationsLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetsLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsreleasesgettomanyrelated"></a>
# **GameCenterLeaderboardSetsReleasesGetToManyRelated**
> GameCenterLeaderboardSetReleasesResponse GameCenterLeaderboardSetsReleasesGetToManyRelated (string id, List<string>? filterLive = null, List<string>? filterGameCenterDetail = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterLeaderboardSets = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetsReleasesGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterLive = new List<string>?(); // List<string>? | filter by attribute 'live' (optional) 
            var filterGameCenterDetail = new List<string>?(); // List<string>? | filter by id(s) of related 'gameCenterDetail' (optional) 
            var fieldsGameCenterLeaderboardSetReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetReleasesResponse result = apiInstance.GameCenterLeaderboardSetsReleasesGetToManyRelated(id, filterLive, filterGameCenterDetail, fieldsGameCenterLeaderboardSetReleases, fieldsGameCenterDetails, fieldsGameCenterLeaderboardSets, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsReleasesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsReleasesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetReleasesResponse> response = apiInstance.GameCenterLeaderboardSetsReleasesGetToManyRelatedWithHttpInfo(id, filterLive, filterGameCenterDetail, fieldsGameCenterLeaderboardSetReleases, fieldsGameCenterDetails, fieldsGameCenterLeaderboardSets, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsReleasesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLive** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;live&#39; | [optional]  |
| **filterGameCenterDetail** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;gameCenterDetail&#39; | [optional]  |
| **fieldsGameCenterLeaderboardSetReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsreleasesgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsReleasesGetToManyRelationship**
> GameCenterLeaderboardSetReleasesLinkagesResponse GameCenterLeaderboardSetsReleasesGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetsReleasesGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetReleasesLinkagesResponse result = apiInstance.GameCenterLeaderboardSetsReleasesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsReleasesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsReleasesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetReleasesLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetsReleasesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsReleasesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsupdateinstance"></a>
# **GameCenterLeaderboardSetsUpdateInstance**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetsUpdateInstance (string id, GameCenterLeaderboardSetUpdateRequest gameCenterLeaderboardSetUpdateRequest)



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
    public class GameCenterLeaderboardSetsUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetUpdateRequest = new GameCenterLeaderboardSetUpdateRequest(); // GameCenterLeaderboardSetUpdateRequest | GameCenterLeaderboardSet representation

            try
            {
                GameCenterLeaderboardSetResponse result = apiInstance.GameCenterLeaderboardSetsUpdateInstance(id, gameCenterLeaderboardSetUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetResponse> response = apiInstance.GameCenterLeaderboardSetsUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2createinstance"></a>
# **GameCenterLeaderboardSetsV2CreateInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2CreateInstance (GameCenterLeaderboardSetV2CreateRequest gameCenterLeaderboardSetV2CreateRequest)



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
    public class GameCenterLeaderboardSetsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetV2CreateRequest = new GameCenterLeaderboardSetV2CreateRequest(); // GameCenterLeaderboardSetV2CreateRequest | GameCenterLeaderboardSet representation

            try
            {
                GameCenterLeaderboardSetV2Response result = apiInstance.GameCenterLeaderboardSetsV2CreateInstance(gameCenterLeaderboardSetV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetV2Response> response = apiInstance.GameCenterLeaderboardSetsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardSetV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2deleteinstance"></a>
# **GameCenterLeaderboardSetsV2DeleteInstance**
> void GameCenterLeaderboardSetsV2DeleteInstance (string id)



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
    public class GameCenterLeaderboardSetsV2DeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardscreatetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsdeletetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated**
> GameCenterLeaderboardsV2Response GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated (string id, List<string>? filterReferenceName = null, List<string>? filterArchived = null, List<string>? filterId = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterLeaderboardVersions = null, int? limit = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitVersions = null)



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
    public class GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
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
                GameCenterLeaderboardsV2Response result = apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterLeaderboardVersions, limit, include, limitGameCenterLeaderboardSets, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardsV2Response> response = apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelatedWithHttpInfo(id, filterReferenceName, filterArchived, filterId, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterActivities, fieldsGameCenterChallenges, fieldsGameCenterLeaderboardVersions, limit, include, limitGameCenterLeaderboardSets, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship**
> GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse result = apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2gamecenterleaderboardsreplacetomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship**
> void GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship (string id, GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest)



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
    public class GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest = new GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest(); // GameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo(id, gameCenterLeaderboardSetV2GameCenterLeaderboardsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GameCenterLeaderboardsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2getinstance"></a>
# **GameCenterLeaderboardSetsV2GetInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetVersions = null, List<string>? include = null, int? limitGameCenterLeaderboards = null, int? limitVersions = null)



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
    public class GameCenterLeaderboardSetsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardSetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboards = 56;  // int? | maximum number of related gameCenterLeaderboards returned (when they are included) (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetV2Response result = apiInstance.GameCenterLeaderboardSetsV2GetInstance(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetVersions, include, limitGameCenterLeaderboards, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetV2Response> response = apiInstance.GameCenterLeaderboardSetsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetVersions, include, limitGameCenterLeaderboards, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboards** | **int?** | maximum number of related gameCenterLeaderboards returned (when they are included) | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2updateinstance"></a>
# **GameCenterLeaderboardSetsV2UpdateInstance**
> GameCenterLeaderboardSetV2Response GameCenterLeaderboardSetsV2UpdateInstance (string id, GameCenterLeaderboardSetV2UpdateRequest gameCenterLeaderboardSetV2UpdateRequest)



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
    public class GameCenterLeaderboardSetsV2UpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetV2UpdateRequest = new GameCenterLeaderboardSetV2UpdateRequest(); // GameCenterLeaderboardSetV2UpdateRequest | GameCenterLeaderboardSet representation

            try
            {
                GameCenterLeaderboardSetV2Response result = apiInstance.GameCenterLeaderboardSetsV2UpdateInstance(id, gameCenterLeaderboardSetV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetV2Response> response = apiInstance.GameCenterLeaderboardSetsV2UpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2versionsgettomanyrelated"></a>
# **GameCenterLeaderboardSetsV2VersionsGetToManyRelated**
> GameCenterLeaderboardSetVersionsV2Response GameCenterLeaderboardSetsV2VersionsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardSetVersions = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class GameCenterLeaderboardSetsV2VersionsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardSetVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetVersions (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboardSetLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardSetVersionsV2Response result = apiInstance.GameCenterLeaderboardSetsV2VersionsGetToManyRelated(id, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetLocalizations, limit, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2VersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2VersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetVersionsV2Response> response = apiInstance.GameCenterLeaderboardSetsV2VersionsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSetVersions, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardSetLocalizations, limit, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2VersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardSetLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetsv2versionsgettomanyrelationship"></a>
# **GameCenterLeaderboardSetsV2VersionsGetToManyRelationship**
> GameCenterLeaderboardSetV2VersionsLinkagesResponse GameCenterLeaderboardSetsV2VersionsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardSetsV2VersionsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardSetV2VersionsLinkagesResponse result = apiInstance.GameCenterLeaderboardSetsV2VersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2VersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetsV2VersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetV2VersionsLinkagesResponse> response = apiInstance.GameCenterLeaderboardSetsV2VersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetsApi.GameCenterLeaderboardSetsV2VersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

