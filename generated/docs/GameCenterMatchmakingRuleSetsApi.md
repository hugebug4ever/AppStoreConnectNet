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
    public class GameCenterMatchmakingRuleSetsCreateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var gameCenterMatchmakingRuleSetCreateRequest = new GameCenterMatchmakingRuleSetCreateRequest(); // GameCenterMatchmakingRuleSetCreateRequest | GameCenterMatchmakingRuleSet representation

            try
            {
                GameCenterMatchmakingRuleSetResponse result = apiInstance.GameCenterMatchmakingRuleSetsCreateInstance(gameCenterMatchmakingRuleSetCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetResponse> response = apiInstance.GameCenterMatchmakingRuleSetsCreateInstanceWithHttpInfo(gameCenterMatchmakingRuleSetCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsdeleteinstance"></a>
# **GameCenterMatchmakingRuleSetsDeleteInstance**
> void GameCenterMatchmakingRuleSetsDeleteInstance (string id)



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
    public class GameCenterMatchmakingRuleSetsDeleteInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterMatchmakingRuleSetsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterMatchmakingRuleSetsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecentermatchmakingrulesetsgetcollection"></a>
# **GameCenterMatchmakingRuleSetsGetCollection**
> GameCenterMatchmakingRuleSetsResponse GameCenterMatchmakingRuleSetsGetCollection (List<string>? fieldsGameCenterMatchmakingRuleSets = null, List<string>? fieldsGameCenterMatchmakingTeams = null, List<string>? fieldsGameCenterMatchmakingRules = null, List<string>? fieldsGameCenterMatchmakingQueues = null, int? limit = null, List<string>? include = null, int? limitMatchmakingQueues = null, int? limitRules = null, int? limitTeams = null)



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
    public class GameCenterMatchmakingRuleSetsGetCollectionExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var fieldsGameCenterMatchmakingRuleSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional) 
            var fieldsGameCenterMatchmakingTeams = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional) 
            var fieldsGameCenterMatchmakingRules = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRules (optional) 
            var fieldsGameCenterMatchmakingQueues = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitMatchmakingQueues = 56;  // int? | maximum number of related matchmakingQueues returned (when they are included) (optional) 
            var limitRules = 56;  // int? | maximum number of related rules returned (when they are included) (optional) 
            var limitTeams = 56;  // int? | maximum number of related teams returned (when they are included) (optional) 

            try
            {
                GameCenterMatchmakingRuleSetsResponse result = apiInstance.GameCenterMatchmakingRuleSetsGetCollection(fieldsGameCenterMatchmakingRuleSets, fieldsGameCenterMatchmakingTeams, fieldsGameCenterMatchmakingRules, fieldsGameCenterMatchmakingQueues, limit, include, limitMatchmakingQueues, limitRules, limitTeams);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetsResponse> response = apiInstance.GameCenterMatchmakingRuleSetsGetCollectionWithHttpInfo(fieldsGameCenterMatchmakingRuleSets, fieldsGameCenterMatchmakingTeams, fieldsGameCenterMatchmakingRules, fieldsGameCenterMatchmakingQueues, limit, include, limitMatchmakingQueues, limitRules, limitTeams);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMatchmakingQueues** | **int?** | maximum number of related matchmakingQueues returned (when they are included) | [optional]  |
| **limitRules** | **int?** | maximum number of related rules returned (when they are included) | [optional]  |
| **limitTeams** | **int?** | maximum number of related teams returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsgetinstance"></a>
# **GameCenterMatchmakingRuleSetsGetInstance**
> GameCenterMatchmakingRuleSetResponse GameCenterMatchmakingRuleSetsGetInstance (string id, List<string>? fieldsGameCenterMatchmakingRuleSets = null, List<string>? fieldsGameCenterMatchmakingTeams = null, List<string>? fieldsGameCenterMatchmakingRules = null, List<string>? fieldsGameCenterMatchmakingQueues = null, List<string>? include = null, int? limitMatchmakingQueues = null, int? limitRules = null, int? limitTeams = null)



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
    public class GameCenterMatchmakingRuleSetsGetInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterMatchmakingRuleSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional) 
            var fieldsGameCenterMatchmakingTeams = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional) 
            var fieldsGameCenterMatchmakingRules = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRules (optional) 
            var fieldsGameCenterMatchmakingQueues = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitMatchmakingQueues = 56;  // int? | maximum number of related matchmakingQueues returned (when they are included) (optional) 
            var limitRules = 56;  // int? | maximum number of related rules returned (when they are included) (optional) 
            var limitTeams = 56;  // int? | maximum number of related teams returned (when they are included) (optional) 

            try
            {
                GameCenterMatchmakingRuleSetResponse result = apiInstance.GameCenterMatchmakingRuleSetsGetInstance(id, fieldsGameCenterMatchmakingRuleSets, fieldsGameCenterMatchmakingTeams, fieldsGameCenterMatchmakingRules, fieldsGameCenterMatchmakingQueues, include, limitMatchmakingQueues, limitRules, limitTeams);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetResponse> response = apiInstance.GameCenterMatchmakingRuleSetsGetInstanceWithHttpInfo(id, fieldsGameCenterMatchmakingRuleSets, fieldsGameCenterMatchmakingTeams, fieldsGameCenterMatchmakingRules, fieldsGameCenterMatchmakingQueues, include, limitMatchmakingQueues, limitRules, limitTeams);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitMatchmakingQueues** | **int?** | maximum number of related matchmakingQueues returned (when they are included) | [optional]  |
| **limitRules** | **int?** | maximum number of related rules returned (when they are included) | [optional]  |
| **limitTeams** | **int?** | maximum number of related teams returned (when they are included) | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated**
> GameCenterMatchmakingQueuesResponse GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated (string id, List<string>? fieldsGameCenterMatchmakingQueues = null, List<string>? fieldsGameCenterMatchmakingRuleSets = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelatedExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterMatchmakingQueues = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional) 
            var fieldsGameCenterMatchmakingRuleSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterMatchmakingQueuesResponse result = apiInstance.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated(id, fieldsGameCenterMatchmakingQueues, fieldsGameCenterMatchmakingRuleSets, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueuesResponse> response = apiInstance.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelatedWithHttpInfo(id, fieldsGameCenterMatchmakingQueues, fieldsGameCenterMatchmakingRuleSets, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **fieldsGameCenterMatchmakingRuleSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsmatchmakingqueuesgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship**
> GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationshipExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse result = apiInstance.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse> response = apiInstance.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsMatchmakingQueuesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsrulesgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsRulesGetToManyRelated**
> GameCenterMatchmakingRulesResponse GameCenterMatchmakingRuleSetsRulesGetToManyRelated (string id, List<string>? fieldsGameCenterMatchmakingRules = null, int? limit = null)



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
    public class GameCenterMatchmakingRuleSetsRulesGetToManyRelatedExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterMatchmakingRules = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingRules (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterMatchmakingRulesResponse result = apiInstance.GameCenterMatchmakingRuleSetsRulesGetToManyRelated(id, fieldsGameCenterMatchmakingRules, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsRulesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsRulesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRulesResponse> response = apiInstance.GameCenterMatchmakingRuleSetsRulesGetToManyRelatedWithHttpInfo(id, fieldsGameCenterMatchmakingRules, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsRulesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingRules** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingRules | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsrulesgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsRulesGetToManyRelationship**
> GameCenterMatchmakingRuleSetRulesLinkagesResponse GameCenterMatchmakingRuleSetsRulesGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterMatchmakingRuleSetsRulesGetToManyRelationshipExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterMatchmakingRuleSetRulesLinkagesResponse result = apiInstance.GameCenterMatchmakingRuleSetsRulesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsRulesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsRulesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetRulesLinkagesResponse> response = apiInstance.GameCenterMatchmakingRuleSetsRulesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsRulesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsteamsgettomanyrelated"></a>
# **GameCenterMatchmakingRuleSetsTeamsGetToManyRelated**
> GameCenterMatchmakingTeamsResponse GameCenterMatchmakingRuleSetsTeamsGetToManyRelated (string id, List<string>? fieldsGameCenterMatchmakingTeams = null, int? limit = null)



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
    public class GameCenterMatchmakingRuleSetsTeamsGetToManyRelatedExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterMatchmakingTeams = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterMatchmakingTeamsResponse result = apiInstance.GameCenterMatchmakingRuleSetsTeamsGetToManyRelated(id, fieldsGameCenterMatchmakingTeams, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsTeamsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsTeamsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingTeamsResponse> response = apiInstance.GameCenterMatchmakingRuleSetsTeamsGetToManyRelatedWithHttpInfo(id, fieldsGameCenterMatchmakingTeams, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsTeamsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingTeams** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsteamsgettomanyrelationship"></a>
# **GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship**
> GameCenterMatchmakingRuleSetTeamsLinkagesResponse GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterMatchmakingRuleSetsTeamsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterMatchmakingRuleSetTeamsLinkagesResponse result = apiInstance.GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsTeamsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsTeamsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetTeamsLinkagesResponse> response = apiInstance.GameCenterMatchmakingRuleSetsTeamsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsTeamsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesetsupdateinstance"></a>
# **GameCenterMatchmakingRuleSetsUpdateInstance**
> GameCenterMatchmakingRuleSetResponse GameCenterMatchmakingRuleSetsUpdateInstance (string id, GameCenterMatchmakingRuleSetUpdateRequest gameCenterMatchmakingRuleSetUpdateRequest)



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
    public class GameCenterMatchmakingRuleSetsUpdateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRuleSetsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterMatchmakingRuleSetUpdateRequest = new GameCenterMatchmakingRuleSetUpdateRequest(); // GameCenterMatchmakingRuleSetUpdateRequest | GameCenterMatchmakingRuleSet representation

            try
            {
                GameCenterMatchmakingRuleSetResponse result = apiInstance.GameCenterMatchmakingRuleSetsUpdateInstance(id, gameCenterMatchmakingRuleSetUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRuleSetsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleSetResponse> response = apiInstance.GameCenterMatchmakingRuleSetsUpdateInstanceWithHttpInfo(id, gameCenterMatchmakingRuleSetUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRuleSetsApi.GameCenterMatchmakingRuleSetsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

