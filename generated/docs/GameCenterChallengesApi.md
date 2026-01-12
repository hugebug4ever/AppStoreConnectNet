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
    public class GameCenterChallengesCreateInstanceExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var gameCenterChallengeCreateRequest = new GameCenterChallengeCreateRequest(); // GameCenterChallengeCreateRequest | GameCenterChallenge representation

            try
            {
                GameCenterChallengeResponse result = apiInstance.GameCenterChallengesCreateInstance(gameCenterChallengeCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeResponse> response = apiInstance.GameCenterChallengesCreateInstanceWithHttpInfo(gameCenterChallengeCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesdeleteinstance"></a>
# **GameCenterChallengesDeleteInstance**
> void GameCenterChallengesDeleteInstance (string id)



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
    public class GameCenterChallengesDeleteInstanceExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterChallengesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterChallengesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecenterchallengesgetinstance"></a>
# **GameCenterChallengesGetInstance**
> GameCenterChallengeResponse GameCenterChallengesGetInstance (string id, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterChallengeVersions = null, List<string>? include = null, int? limitVersions = null)



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
    public class GameCenterChallengesGetInstanceExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var fieldsGameCenterChallengeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVersions = 56;  // int? | maximum number of related versions returned (when they are included) (optional) 

            try
            {
                GameCenterChallengeResponse result = apiInstance.GameCenterChallengesGetInstance(id, fieldsGameCenterChallenges, fieldsGameCenterChallengeVersions, include, limitVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeResponse> response = apiInstance.GameCenterChallengesGetInstanceWithHttpInfo(id, fieldsGameCenterChallenges, fieldsGameCenterChallengeVersions, include, limitVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVersions** | **int?** | maximum number of related versions returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesleaderboardupdatetoonerelationship"></a>
# **GameCenterChallengesLeaderboardUpdateToOneRelationship**
> void GameCenterChallengesLeaderboardUpdateToOneRelationship (string id, GameCenterChallengeLeaderboardLinkageRequest gameCenterChallengeLeaderboardLinkageRequest)



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
    public class GameCenterChallengesLeaderboardUpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterChallengeLeaderboardLinkageRequest = new GameCenterChallengeLeaderboardLinkageRequest(); // GameCenterChallengeLeaderboardLinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterChallengesLeaderboardUpdateToOneRelationship(id, gameCenterChallengeLeaderboardLinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesLeaderboardUpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesLeaderboardUpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterChallengesLeaderboardUpdateToOneRelationshipWithHttpInfo(id, gameCenterChallengeLeaderboardLinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesLeaderboardUpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesleaderboardv2updatetoonerelationship"></a>
# **GameCenterChallengesLeaderboardV2UpdateToOneRelationship**
> void GameCenterChallengesLeaderboardV2UpdateToOneRelationship (string id, GameCenterChallengeLeaderboardV2LinkageRequest gameCenterChallengeLeaderboardV2LinkageRequest)



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
    public class GameCenterChallengesLeaderboardV2UpdateToOneRelationshipExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterChallengeLeaderboardV2LinkageRequest = new GameCenterChallengeLeaderboardV2LinkageRequest(); // GameCenterChallengeLeaderboardV2LinkageRequest | Related linkage

            try
            {
                apiInstance.GameCenterChallengesLeaderboardV2UpdateToOneRelationship(id, gameCenterChallengeLeaderboardV2LinkageRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesLeaderboardV2UpdateToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesLeaderboardV2UpdateToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterChallengesLeaderboardV2UpdateToOneRelationshipWithHttpInfo(id, gameCenterChallengeLeaderboardV2LinkageRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesLeaderboardV2UpdateToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesupdateinstance"></a>
# **GameCenterChallengesUpdateInstance**
> GameCenterChallengeResponse GameCenterChallengesUpdateInstance (string id, GameCenterChallengeUpdateRequest gameCenterChallengeUpdateRequest)



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
    public class GameCenterChallengesUpdateInstanceExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterChallengeUpdateRequest = new GameCenterChallengeUpdateRequest(); // GameCenterChallengeUpdateRequest | GameCenterChallenge representation

            try
            {
                GameCenterChallengeResponse result = apiInstance.GameCenterChallengesUpdateInstance(id, gameCenterChallengeUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeResponse> response = apiInstance.GameCenterChallengesUpdateInstanceWithHttpInfo(id, gameCenterChallengeUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesversionsgettomanyrelated"></a>
# **GameCenterChallengesVersionsGetToManyRelated**
> GameCenterChallengeVersionsResponse GameCenterChallengesVersionsGetToManyRelated (string id, List<string>? fieldsGameCenterChallengeVersions = null, List<string>? fieldsGameCenterChallenges = null, List<string>? fieldsGameCenterChallengeLocalizations = null, List<string>? fieldsGameCenterChallengeVersionReleases = null, List<string>? fieldsGameCenterChallengeImages = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null, int? limitReleases = null)



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
    public class GameCenterChallengesVersionsGetToManyRelatedExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterChallengeVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersions (optional) 
            var fieldsGameCenterChallenges = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallenges (optional) 
            var fieldsGameCenterChallengeLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional) 
            var fieldsGameCenterChallengeVersionReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional) 
            var fieldsGameCenterChallengeImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterChallengeImages (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 
            var limitReleases = 56;  // int? | maximum number of related releases returned (when they are included) (optional) 

            try
            {
                GameCenterChallengeVersionsResponse result = apiInstance.GameCenterChallengesVersionsGetToManyRelated(id, fieldsGameCenterChallengeVersions, fieldsGameCenterChallenges, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeVersionReleases, fieldsGameCenterChallengeImages, limit, include, limitLocalizations, limitReleases);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionsResponse> response = apiInstance.GameCenterChallengesVersionsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterChallengeVersions, fieldsGameCenterChallenges, fieldsGameCenterChallengeLocalizations, fieldsGameCenterChallengeVersionReleases, fieldsGameCenterChallengeImages, limit, include, limitLocalizations, limitReleases);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterChallenges** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallenges | [optional]  |
| **fieldsGameCenterChallengeLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional]  |
| **fieldsGameCenterChallengeVersionReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional]  |
| **fieldsGameCenterChallengeImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterChallengeImages | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |
| **limitReleases** | **int?** | maximum number of related releases returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterchallengesversionsgettomanyrelationship"></a>
# **GameCenterChallengesVersionsGetToManyRelationship**
> GameCenterChallengeVersionsLinkagesResponse GameCenterChallengesVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterChallengesVersionsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterChallengesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterChallengeVersionsLinkagesResponse result = apiInstance.GameCenterChallengesVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterChallengesVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterChallengeVersionsLinkagesResponse> response = apiInstance.GameCenterChallengesVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterChallengesApi.GameCenterChallengesVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

