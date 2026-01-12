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
    public class GameCenterLeaderboardsActivityUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardActivityLinkageRequest = new GameCenterLeaderboardActivityLinkageRequest(); // GameCenterLeaderboardActivityLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardsActivityUpdateToOneRelationship(id, gameCenterLeaderboardActivityLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsActivityUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsActivityUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsActivityUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardActivityLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsActivityUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardschallengeupdatetoonerelationship"></a>
# **GameCenterLeaderboardsChallengeUpdateToOneRelationship**
> void GameCenterLeaderboardsChallengeUpdateToOneRelationship (string id, GameCenterLeaderboardChallengeLinkageRequest gameCenterLeaderboardChallengeLinkageRequest)



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
    public class GameCenterLeaderboardsChallengeUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardChallengeLinkageRequest = new GameCenterLeaderboardChallengeLinkageRequest(); // GameCenterLeaderboardChallengeLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardsChallengeUpdateToOneRelationship(id, gameCenterLeaderboardChallengeLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsChallengeUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsChallengeUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsChallengeUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardChallengeLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsChallengeUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardscreateinstance"></a>
# **GameCenterLeaderboardsCreateInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsCreateInstance (GameCenterLeaderboardCreateRequest gameCenterLeaderboardCreateRequest)



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
    public class GameCenterLeaderboardsCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardCreateRequest = new GameCenterLeaderboardCreateRequest(); // GameCenterLeaderboardCreateRequest | GameCenterLeaderboard representation

            try
            {
                GameCenterLeaderboardResponse result = apiInstance.GameCenterLeaderboardsCreateInstance(gameCenterLeaderboardCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardResponse> response = apiInstance.GameCenterLeaderboardsCreateInstanceWithHttpInfo(gameCenterLeaderboardCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsdeleteinstance"></a>
# **GameCenterLeaderboardsDeleteInstance**
> void GameCenterLeaderboardsDeleteInstance (string id)



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
    public class GameCenterLeaderboardsDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsgetinstance"></a>
# **GameCenterLeaderboardsGetInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsGetInstance (string id, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardsGetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardResponse result = apiInstance.GameCenterLeaderboardsGetInstance(id, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardResponse> response = apiInstance.GameCenterLeaderboardsGetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsgroupleaderboardgettoonerelated"></a>
# **GameCenterLeaderboardsGroupLeaderboardGetToOneRelated**
> GameCenterLeaderboardResponse GameCenterLeaderboardsGroupLeaderboardGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardsGroupLeaderboardGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterGroups (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboardReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional) 
            var fieldsGameCenterActivities = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterActivities (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardResponse result = apiInstance.GameCenterLeaderboardsGroupLeaderboardGetToOneRelated(id, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsGroupLeaderboardGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardResponse> response = apiInstance.GameCenterLeaderboardsGroupLeaderboardGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterGroups | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterActivities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterActivities | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsgroupleaderboardgettoonerelationship"></a>
# **GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship**
> GameCenterLeaderboardGroupLeaderboardLinkageResponse GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardsGroupLeaderboardGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardGroupLeaderboardLinkageResponse result = apiInstance.GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsGroupLeaderboardGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardGroupLeaderboardLinkageResponse> response = apiInstance.GameCenterLeaderboardsGroupLeaderboardGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsgroupleaderboardupdatetoonerelationship"></a>
# **GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship**
> void GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship (string id, GameCenterLeaderboardGroupLeaderboardLinkageRequest gameCenterLeaderboardGroupLeaderboardLinkageRequest)



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
    public class GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardGroupLeaderboardLinkageRequest = new GameCenterLeaderboardGroupLeaderboardLinkageRequest(); // GameCenterLeaderboardGroupLeaderboardLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship(id, gameCenterLeaderboardGroupLeaderboardLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardGroupLeaderboardLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsGroupLeaderboardUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardslocalizationsgettomanyrelated"></a>
# **GameCenterLeaderboardsLocalizationsGetToManyRelated**
> GameCenterLeaderboardLocalizationsResponse GameCenterLeaderboardsLocalizationsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardImages = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardsLocalizationsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardLocalizationsResponse result = apiInstance.GameCenterLeaderboardsLocalizationsGetToManyRelated(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardImages, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationsResponse> response = apiInstance.GameCenterLeaderboardsLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardImages, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardslocalizationsgettomanyrelationship"></a>
# **GameCenterLeaderboardsLocalizationsGetToManyRelationship**
> GameCenterLeaderboardLocalizationsLinkagesResponse GameCenterLeaderboardsLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardsLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardLocalizationsLinkagesResponse result = apiInstance.GameCenterLeaderboardsLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardLocalizationsLinkagesResponse> response = apiInstance.GameCenterLeaderboardsLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsreleasesgettomanyrelated"></a>
# **GameCenterLeaderboardsReleasesGetToManyRelated**
> GameCenterLeaderboardReleasesResponse GameCenterLeaderboardsReleasesGetToManyRelated (string id, List<string>? filterLive = null, List<string>? filterGameCenterDetail = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterLeaderboards = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardsReleasesGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterLive = new List<string>?(); // List<string>? | filter by attribute 'live' (optional) 
            var filterGameCenterDetail = new List<string>?(); // List<string>? | filter by id(s) of related 'gameCenterDetail' (optional) 
            var fieldsGameCenterLeaderboardReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional) 
            var fieldsGameCenterDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterDetails (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardReleasesResponse result = apiInstance.GameCenterLeaderboardsReleasesGetToManyRelated(id, filterLive, filterGameCenterDetail, fieldsGameCenterLeaderboardReleases, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsReleasesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsReleasesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardReleasesResponse> response = apiInstance.GameCenterLeaderboardsReleasesGetToManyRelatedWithHttpInfo(id, filterLive, filterGameCenterDetail, fieldsGameCenterLeaderboardReleases, fieldsGameCenterDetails, fieldsGameCenterLeaderboards, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsReleasesGetToManyRelatedWithHttpInfo: " + e.Message);
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
| **fieldsGameCenterLeaderboardReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional]  |
| **fieldsGameCenterDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterDetails | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsreleasesgettomanyrelationship"></a>
# **GameCenterLeaderboardsReleasesGetToManyRelationship**
> GameCenterLeaderboardReleasesLinkagesResponse GameCenterLeaderboardsReleasesGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardsReleasesGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardReleasesLinkagesResponse result = apiInstance.GameCenterLeaderboardsReleasesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsReleasesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsReleasesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardReleasesLinkagesResponse> response = apiInstance.GameCenterLeaderboardsReleasesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsReleasesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsupdateinstance"></a>
# **GameCenterLeaderboardsUpdateInstance**
> GameCenterLeaderboardResponse GameCenterLeaderboardsUpdateInstance (string id, GameCenterLeaderboardUpdateRequest gameCenterLeaderboardUpdateRequest)



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
    public class GameCenterLeaderboardsUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardUpdateRequest = new GameCenterLeaderboardUpdateRequest(); // GameCenterLeaderboardUpdateRequest | GameCenterLeaderboard representation

            try
            {
                GameCenterLeaderboardResponse result = apiInstance.GameCenterLeaderboardsUpdateInstance(id, gameCenterLeaderboardUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardResponse> response = apiInstance.GameCenterLeaderboardsUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2activityupdatetoonerelationship"></a>
# **GameCenterLeaderboardsV2ActivityUpdateToOneRelationship**
> void GameCenterLeaderboardsV2ActivityUpdateToOneRelationship (string id, GameCenterLeaderboardV2ActivityLinkageRequest gameCenterLeaderboardV2ActivityLinkageRequest)



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
    public class GameCenterLeaderboardsV2ActivityUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardV2ActivityLinkageRequest = new GameCenterLeaderboardV2ActivityLinkageRequest(); // GameCenterLeaderboardV2ActivityLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardsV2ActivityUpdateToOneRelationship(id, gameCenterLeaderboardV2ActivityLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2ActivityUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2ActivityUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsV2ActivityUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardV2ActivityLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2ActivityUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2challengeupdatetoonerelationship"></a>
# **GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship**
> void GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship (string id, GameCenterLeaderboardV2ChallengeLinkageRequest gameCenterLeaderboardV2ChallengeLinkageRequest)



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
    public class GameCenterLeaderboardsV2ChallengeUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardV2ChallengeLinkageRequest = new GameCenterLeaderboardV2ChallengeLinkageRequest(); // GameCenterLeaderboardV2ChallengeLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship(id, gameCenterLeaderboardV2ChallengeLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2ChallengeUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2ChallengeUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsV2ChallengeUpdateToOneRelationshipWithHttpInfo(id, gameCenterLeaderboardV2ChallengeLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2ChallengeUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2createinstance"></a>
# **GameCenterLeaderboardsV2CreateInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2CreateInstance (GameCenterLeaderboardV2CreateRequest gameCenterLeaderboardV2CreateRequest)



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
    public class GameCenterLeaderboardsV2CreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardV2CreateRequest = new GameCenterLeaderboardV2CreateRequest(); // GameCenterLeaderboardV2CreateRequest | GameCenterLeaderboard representation

            try
            {
                GameCenterLeaderboardV2Response result = apiInstance.GameCenterLeaderboardsV2CreateInstance(gameCenterLeaderboardV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardV2Response> response = apiInstance.GameCenterLeaderboardsV2CreateInstanceWithHttpInfo(gameCenterLeaderboardV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2deleteinstance"></a>
# **GameCenterLeaderboardsV2DeleteInstance**
> void GameCenterLeaderboardsV2DeleteInstance (string id)



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
    public class GameCenterLeaderboardsV2DeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsv2getinstance"></a>
# **GameCenterLeaderboardsV2GetInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2GetInstance (string id, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardVersions = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitVersions = null)



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
    public class GameCenterLeaderboardsV2GetInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitGameCenterLeaderboardSets = 56;  // int? | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardV2Response result = apiInstance.GameCenterLeaderboardsV2GetInstance(id, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardVersions, include, limitGameCenterLeaderboardSets, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardV2Response> response = apiInstance.GameCenterLeaderboardsV2GetInstanceWithHttpInfo(id, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardVersions, include, limitGameCenterLeaderboardSets, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitGameCenterLeaderboardSets** | **int?** | maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2updateinstance"></a>
# **GameCenterLeaderboardsV2UpdateInstance**
> GameCenterLeaderboardV2Response GameCenterLeaderboardsV2UpdateInstance (string id, GameCenterLeaderboardV2UpdateRequest gameCenterLeaderboardV2UpdateRequest)



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
    public class GameCenterLeaderboardsV2UpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardV2UpdateRequest = new GameCenterLeaderboardV2UpdateRequest(); // GameCenterLeaderboardV2UpdateRequest | GameCenterLeaderboard representation

            try
            {
                GameCenterLeaderboardV2Response result = apiInstance.GameCenterLeaderboardsV2UpdateInstance(id, gameCenterLeaderboardV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardV2Response> response = apiInstance.GameCenterLeaderboardsV2UpdateInstanceWithHttpInfo(id, gameCenterLeaderboardV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2versionsgettomanyrelated"></a>
# **GameCenterLeaderboardsV2VersionsGetToManyRelated**
> GameCenterLeaderboardVersionsV2Response GameCenterLeaderboardsV2VersionsGetToManyRelated (string id, List<string>? fieldsGameCenterLeaderboardVersions = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class GameCenterLeaderboardsV2VersionsGetToManyRelatedExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterLeaderboardVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardVersions (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var fieldsGameCenterLeaderboardLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                GameCenterLeaderboardVersionsV2Response result = apiInstance.GameCenterLeaderboardsV2VersionsGetToManyRelated(id, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardLocalizations, limit, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2VersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2VersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardVersionsV2Response> response = apiInstance.GameCenterLeaderboardsV2VersionsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardVersions, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardLocalizations, limit, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2VersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **fieldsGameCenterLeaderboardLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsv2versionsgettomanyrelationship"></a>
# **GameCenterLeaderboardsV2VersionsGetToManyRelationship**
> GameCenterLeaderboardV2VersionsLinkagesResponse GameCenterLeaderboardsV2VersionsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterLeaderboardsV2VersionsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterLeaderboardV2VersionsLinkagesResponse result = apiInstance.GameCenterLeaderboardsV2VersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2VersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardsV2VersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardV2VersionsLinkagesResponse> response = apiInstance.GameCenterLeaderboardsV2VersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardsApi.GameCenterLeaderboardsV2VersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

