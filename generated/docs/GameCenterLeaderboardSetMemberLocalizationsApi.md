# AppStoreConnect.Net.Api.GameCenterLeaderboardSetMemberLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterLeaderboardSetMemberLocalizationsCreateInstance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationscreateinstance) | **POST** /v1/gameCenterLeaderboardSetMemberLocalizations |  |
| [**GameCenterLeaderboardSetMemberLocalizationsDeleteInstance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsdeleteinstance) | **DELETE** /v1/gameCenterLeaderboardSetMemberLocalizations/{id} |  |
| [**GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelated**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardgettoonerelated) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/gameCenterLeaderboard |  |
| [**GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationship**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardgettoonerelationship) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/relationships/gameCenterLeaderboard |  |
| [**GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelated**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardsetgettoonerelated) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/gameCenterLeaderboardSet |  |
| [**GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationship**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardsetgettoonerelationship) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/relationships/gameCenterLeaderboardSet |  |
| [**GameCenterLeaderboardSetMemberLocalizationsGetCollection**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsgetcollection) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations |  |
| [**GameCenterLeaderboardSetMemberLocalizationsUpdateInstance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#gamecenterleaderboardsetmemberlocalizationsupdateinstance) | **PATCH** /v1/gameCenterLeaderboardSetMemberLocalizations/{id} |  |

<a id="gamecenterleaderboardsetmemberlocalizationscreateinstance"></a>
# **GameCenterLeaderboardSetMemberLocalizationsCreateInstance**
> GameCenterLeaderboardSetMemberLocalizationResponse GameCenterLeaderboardSetMemberLocalizationsCreateInstance (GameCenterLeaderboardSetMemberLocalizationCreateRequest gameCenterLeaderboardSetMemberLocalizationCreateRequest)



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
    public class GameCenterLeaderboardSetMemberLocalizationsCreateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var gameCenterLeaderboardSetMemberLocalizationCreateRequest = new GameCenterLeaderboardSetMemberLocalizationCreateRequest(); // GameCenterLeaderboardSetMemberLocalizationCreateRequest | GameCenterLeaderboardSetMemberLocalization representation

            try
            {
                GameCenterLeaderboardSetMemberLocalizationResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsCreateInstance(gameCenterLeaderboardSetMemberLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetMemberLocalizationResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsCreateInstanceWithHttpInfo(gameCenterLeaderboardSetMemberLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterLeaderboardSetMemberLocalizationCreateRequest** | [**GameCenterLeaderboardSetMemberLocalizationCreateRequest**](GameCenterLeaderboardSetMemberLocalizationCreateRequest.md) | GameCenterLeaderboardSetMemberLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetMemberLocalizationResponse**](GameCenterLeaderboardSetMemberLocalizationResponse.md)

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
| **201** | Single GameCenterLeaderboardSetMemberLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetmemberlocalizationsdeleteinstance"></a>
# **GameCenterLeaderboardSetMemberLocalizationsDeleteInstance**
> void GameCenterLeaderboardSetMemberLocalizationsDeleteInstance (string id)



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
    public class GameCenterLeaderboardSetMemberLocalizationsDeleteInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterLeaderboardSetMemberLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterLeaderboardSetMemberLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardgettoonerelated"></a>
# **GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelated**
> GameCenterLeaderboardResponse GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboardLocalizations = null, List<string>? fieldsGameCenterLeaderboardReleases = null, List<string>? fieldsGameCenterActivities = null, List<string>? fieldsGameCenterChallenges = null, List<string>? include = null, int? limitGameCenterLeaderboardSets = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
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
                GameCenterLeaderboardResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelated(id, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboards, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboardLocalizations, fieldsGameCenterLeaderboardReleases, fieldsGameCenterActivities, fieldsGameCenterChallenges, include, limitGameCenterLeaderboardSets, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardgettoonerelationship"></a>
# **GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationship**
> GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse**](GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse.md)

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

<a id="gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardsetgettoonerelated"></a>
# **GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelated**
> GameCenterLeaderboardSetResponse GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelated (string id, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterDetails = null, List<string>? fieldsGameCenterGroups = null, List<string>? fieldsGameCenterLeaderboardSetLocalizations = null, List<string>? fieldsGameCenterLeaderboards = null, List<string>? fieldsGameCenterLeaderboardSetReleases = null, List<string>? include = null, int? limitLocalizations = null, int? limitGameCenterLeaderboards = null, int? limitReleases = null)



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
    public class GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelatedExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
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
                GameCenterLeaderboardSetResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelated(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelatedWithHttpInfo(id, fieldsGameCenterLeaderboardSets, fieldsGameCenterDetails, fieldsGameCenterGroups, fieldsGameCenterLeaderboardSetLocalizations, fieldsGameCenterLeaderboards, fieldsGameCenterLeaderboardSetReleases, include, limitLocalizations, limitGameCenterLeaderboards, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="gamecenterleaderboardsetmemberlocalizationsgamecenterleaderboardsetgettoonerelationship"></a>
# **GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationship**
> GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationship (string id)



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
    public class GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationshipExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGameCenterLeaderboardSetGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse**](GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse.md)

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

<a id="gamecenterleaderboardsetmemberlocalizationsgetcollection"></a>
# **GameCenterLeaderboardSetMemberLocalizationsGetCollection**
> GameCenterLeaderboardSetMemberLocalizationsResponse GameCenterLeaderboardSetMemberLocalizationsGetCollection (List<string> filterGameCenterLeaderboardSet, List<string> filterGameCenterLeaderboard, List<string>? fieldsGameCenterLeaderboardSetMemberLocalizations = null, List<string>? fieldsGameCenterLeaderboardSets = null, List<string>? fieldsGameCenterLeaderboards = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterLeaderboardSetMemberLocalizationsGetCollectionExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var filterGameCenterLeaderboardSet = new List<string>(); // List<string> | filter by id(s) of related 'gameCenterLeaderboardSet'
            var filterGameCenterLeaderboard = new List<string>(); // List<string> | filter by id(s) of related 'gameCenterLeaderboard'
            var fieldsGameCenterLeaderboardSetMemberLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSetMemberLocalizations (optional) 
            var fieldsGameCenterLeaderboardSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboardSets (optional) 
            var fieldsGameCenterLeaderboards = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterLeaderboards (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterLeaderboardSetMemberLocalizationsResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGetCollection(filterGameCenterLeaderboardSet, filterGameCenterLeaderboard, fieldsGameCenterLeaderboardSetMemberLocalizations, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboards, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetMemberLocalizationsResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsGetCollectionWithHttpInfo(filterGameCenterLeaderboardSet, filterGameCenterLeaderboard, fieldsGameCenterLeaderboardSetMemberLocalizations, fieldsGameCenterLeaderboardSets, fieldsGameCenterLeaderboards, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterGameCenterLeaderboardSet** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterLeaderboardSet&#39; |  |
| **filterGameCenterLeaderboard** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;gameCenterLeaderboard&#39; |  |
| **fieldsGameCenterLeaderboardSetMemberLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetMemberLocalizations | [optional]  |
| **fieldsGameCenterLeaderboardSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSets | [optional]  |
| **fieldsGameCenterLeaderboards** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterLeaderboards | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterLeaderboardSetMemberLocalizationsResponse**](GameCenterLeaderboardSetMemberLocalizationsResponse.md)

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
| **200** | List of GameCenterLeaderboardSetMemberLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterleaderboardsetmemberlocalizationsupdateinstance"></a>
# **GameCenterLeaderboardSetMemberLocalizationsUpdateInstance**
> GameCenterLeaderboardSetMemberLocalizationResponse GameCenterLeaderboardSetMemberLocalizationsUpdateInstance (string id, GameCenterLeaderboardSetMemberLocalizationUpdateRequest gameCenterLeaderboardSetMemberLocalizationUpdateRequest)



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
    public class GameCenterLeaderboardSetMemberLocalizationsUpdateInstanceExample
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
            var apiInstance = new GameCenterLeaderboardSetMemberLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterLeaderboardSetMemberLocalizationUpdateRequest = new GameCenterLeaderboardSetMemberLocalizationUpdateRequest(); // GameCenterLeaderboardSetMemberLocalizationUpdateRequest | GameCenterLeaderboardSetMemberLocalization representation

            try
            {
                GameCenterLeaderboardSetMemberLocalizationResponse result = apiInstance.GameCenterLeaderboardSetMemberLocalizationsUpdateInstance(id, gameCenterLeaderboardSetMemberLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterLeaderboardSetMemberLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterLeaderboardSetMemberLocalizationResponse> response = apiInstance.GameCenterLeaderboardSetMemberLocalizationsUpdateInstanceWithHttpInfo(id, gameCenterLeaderboardSetMemberLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi.GameCenterLeaderboardSetMemberLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterLeaderboardSetMemberLocalizationUpdateRequest** | [**GameCenterLeaderboardSetMemberLocalizationUpdateRequest**](GameCenterLeaderboardSetMemberLocalizationUpdateRequest.md) | GameCenterLeaderboardSetMemberLocalization representation |  |

### Return type

[**GameCenterLeaderboardSetMemberLocalizationResponse**](GameCenterLeaderboardSetMemberLocalizationResponse.md)

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
| **200** | Single GameCenterLeaderboardSetMemberLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

