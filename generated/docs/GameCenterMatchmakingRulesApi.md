# AppStoreConnect.Net.Api.GameCenterMatchmakingRulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterMatchmakingRulesCreateInstance**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulescreateinstance) | **POST** /v1/gameCenterMatchmakingRules |  |
| [**GameCenterMatchmakingRulesDeleteInstance**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulesdeleteinstance) | **DELETE** /v1/gameCenterMatchmakingRules/{id} |  |
| [**GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulesmatchmakingbooleanruleresultsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingBooleanRuleResults |  |
| [**GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulesmatchmakingnumberruleresultsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingNumberRuleResults |  |
| [**GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulesmatchmakingruleerrorsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingRuleErrors |  |
| [**GameCenterMatchmakingRulesUpdateInstance**](GameCenterMatchmakingRulesApi.md#gamecentermatchmakingrulesupdateinstance) | **PATCH** /v1/gameCenterMatchmakingRules/{id} |  |

<a id="gamecentermatchmakingrulescreateinstance"></a>
# **GameCenterMatchmakingRulesCreateInstance**
> GameCenterMatchmakingRuleResponse GameCenterMatchmakingRulesCreateInstance (GameCenterMatchmakingRuleCreateRequest gameCenterMatchmakingRuleCreateRequest)



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
    public class GameCenterMatchmakingRulesCreateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var gameCenterMatchmakingRuleCreateRequest = new GameCenterMatchmakingRuleCreateRequest(); // GameCenterMatchmakingRuleCreateRequest | GameCenterMatchmakingRule representation

            try
            {
                GameCenterMatchmakingRuleResponse result = apiInstance.GameCenterMatchmakingRulesCreateInstance(gameCenterMatchmakingRuleCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleResponse> response = apiInstance.GameCenterMatchmakingRulesCreateInstanceWithHttpInfo(gameCenterMatchmakingRuleCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterMatchmakingRuleCreateRequest** | [**GameCenterMatchmakingRuleCreateRequest**](GameCenterMatchmakingRuleCreateRequest.md) | GameCenterMatchmakingRule representation |  |

### Return type

[**GameCenterMatchmakingRuleResponse**](GameCenterMatchmakingRuleResponse.md)

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
| **201** | Single GameCenterMatchmakingRule |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesdeleteinstance"></a>
# **GameCenterMatchmakingRulesDeleteInstance**
> void GameCenterMatchmakingRulesDeleteInstance (string id)



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
    public class GameCenterMatchmakingRulesDeleteInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterMatchmakingRulesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterMatchmakingRulesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="gamecentermatchmakingrulesmatchmakingbooleanruleresultsgetmetrics"></a>
# **GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics**
> GameCenterMatchmakingBooleanRuleResultsV1MetricResponse GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterResult = null, string? filterGameCenterMatchmakingQueue = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetricsExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterResult = "filterResult_example";  // string? | filter by 'result' attribute dimension (optional) 
            var filterGameCenterMatchmakingQueue = "filterGameCenterMatchmakingQueue_example";  // string? | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingBooleanRuleResultsV1MetricResponse result = apiInstance.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics(id, granularity, groupBy, filterResult, filterGameCenterMatchmakingQueue, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingBooleanRuleResultsV1MetricResponse> response = apiInstance.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetricsWithHttpInfo(id, granularity, groupBy, filterResult, filterGameCenterMatchmakingQueue, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **groupBy** | [**List&lt;string&gt;?**](string.md) | the dimension by which to group the results | [optional]  |
| **filterResult** | **string?** | filter by &#39;result&#39; attribute dimension | [optional]  |
| **filterGameCenterMatchmakingQueue** | **string?** | filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingBooleanRuleResultsV1MetricResponse**](GameCenterMatchmakingBooleanRuleResultsV1MetricResponse.md)

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
| **200** | Metrics data response |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesmatchmakingnumberruleresultsgetmetrics"></a>
# **GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics**
> GameCenterMatchmakingNumberRuleResultsV1MetricResponse GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterGameCenterMatchmakingQueue = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetricsExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterGameCenterMatchmakingQueue = "filterGameCenterMatchmakingQueue_example";  // string? | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingNumberRuleResultsV1MetricResponse result = apiInstance.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics(id, granularity, groupBy, filterGameCenterMatchmakingQueue, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingNumberRuleResultsV1MetricResponse> response = apiInstance.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetricsWithHttpInfo(id, granularity, groupBy, filterGameCenterMatchmakingQueue, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **groupBy** | [**List&lt;string&gt;?**](string.md) | the dimension by which to group the results | [optional]  |
| **filterGameCenterMatchmakingQueue** | **string?** | filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingNumberRuleResultsV1MetricResponse**](GameCenterMatchmakingNumberRuleResultsV1MetricResponse.md)

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
| **200** | Metrics data response |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesmatchmakingruleerrorsgetmetrics"></a>
# **GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics**
> GameCenterMatchmakingRuleErrorsV1MetricResponse GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterGameCenterMatchmakingQueue = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetricsExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterGameCenterMatchmakingQueue = "filterGameCenterMatchmakingQueue_example";  // string? | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingRuleErrorsV1MetricResponse result = apiInstance.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics(id, granularity, groupBy, filterGameCenterMatchmakingQueue, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleErrorsV1MetricResponse> response = apiInstance.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetricsWithHttpInfo(id, granularity, groupBy, filterGameCenterMatchmakingQueue, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **groupBy** | [**List&lt;string&gt;?**](string.md) | the dimension by which to group the results | [optional]  |
| **filterGameCenterMatchmakingQueue** | **string?** | filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingRuleErrorsV1MetricResponse**](GameCenterMatchmakingRuleErrorsV1MetricResponse.md)

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
| **200** | Metrics data response |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingrulesupdateinstance"></a>
# **GameCenterMatchmakingRulesUpdateInstance**
> GameCenterMatchmakingRuleResponse GameCenterMatchmakingRulesUpdateInstance (string id, GameCenterMatchmakingRuleUpdateRequest gameCenterMatchmakingRuleUpdateRequest)



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
    public class GameCenterMatchmakingRulesUpdateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingRulesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterMatchmakingRuleUpdateRequest = new GameCenterMatchmakingRuleUpdateRequest(); // GameCenterMatchmakingRuleUpdateRequest | GameCenterMatchmakingRule representation

            try
            {
                GameCenterMatchmakingRuleResponse result = apiInstance.GameCenterMatchmakingRulesUpdateInstance(id, gameCenterMatchmakingRuleUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingRulesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingRuleResponse> response = apiInstance.GameCenterMatchmakingRulesUpdateInstanceWithHttpInfo(id, gameCenterMatchmakingRuleUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingRulesApi.GameCenterMatchmakingRulesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterMatchmakingRuleUpdateRequest** | [**GameCenterMatchmakingRuleUpdateRequest**](GameCenterMatchmakingRuleUpdateRequest.md) | GameCenterMatchmakingRule representation |  |

### Return type

[**GameCenterMatchmakingRuleResponse**](GameCenterMatchmakingRuleResponse.md)

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
| **200** | Single GameCenterMatchmakingRule |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

