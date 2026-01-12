# AppStoreConnect.Net.Api.MetricsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppsBetaTesterUsagesGetMetrics**](MetricsApi.md#appsbetatesterusagesgetmetrics) | **GET** /v1/apps/{id}/metrics/betaTesterUsages |  |
| [**BetaGroupsBetaTesterUsagesGetMetrics**](MetricsApi.md#betagroupsbetatesterusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/betaTesterUsages |  |
| [**BetaGroupsPublicLinkUsagesGetMetrics**](MetricsApi.md#betagroupspubliclinkusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/publicLinkUsages |  |
| [**BetaTestersBetaTesterUsagesGetMetrics**](MetricsApi.md#betatestersbetatesterusagesgetmetrics) | **GET** /v1/betaTesters/{id}/metrics/betaTesterUsages |  |
| [**BuildsBetaBuildUsagesGetMetrics**](MetricsApi.md#buildsbetabuildusagesgetmetrics) | **GET** /v1/builds/{id}/metrics/betaBuildUsages |  |
| [**GameCenterDetailsClassicMatchmakingRequestsGetMetrics**](MetricsApi.md#gamecenterdetailsclassicmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterDetails/{id}/metrics/classicMatchmakingRequests |  |
| [**GameCenterDetailsRuleBasedMatchmakingRequestsGetMetrics**](MetricsApi.md#gamecenterdetailsrulebasedmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterDetails/{id}/metrics/ruleBasedMatchmakingRequests |  |
| [**GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics**](MetricsApi.md#gamecentermatchmakingqueuesexperimentmatchmakingqueuesizesgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingQueueSizes |  |
| [**GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics**](MetricsApi.md#gamecentermatchmakingqueuesexperimentmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingRequests |  |
| [**GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics**](MetricsApi.md#gamecentermatchmakingqueuesmatchmakingqueuesizesgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingQueueSizes |  |
| [**GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics**](MetricsApi.md#gamecentermatchmakingqueuesmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingRequests |  |
| [**GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics**](MetricsApi.md#gamecentermatchmakingqueuesmatchmakingsessionsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingSessions |  |
| [**GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics**](MetricsApi.md#gamecentermatchmakingrulesmatchmakingbooleanruleresultsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingBooleanRuleResults |  |
| [**GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics**](MetricsApi.md#gamecentermatchmakingrulesmatchmakingnumberruleresultsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingNumberRuleResults |  |
| [**GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics**](MetricsApi.md#gamecentermatchmakingrulesmatchmakingruleerrorsgetmetrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingRuleErrors |  |

<a id="appsbetatesterusagesgetmetrics"></a>
# **AppsBetaTesterUsagesGetMetrics**
> AppsBetaTesterUsagesV1MetricResponse AppsBetaTesterUsagesGetMetrics (string id, string? period = null, List<string>? groupBy = null, string? filterBetaTesters = null, int? limit = null)



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
    public class AppsBetaTesterUsagesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var period = P7D;  // string? | the duration of the reporting period (optional) 
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterBetaTesters = "filterBetaTesters_example";  // string? | filter by 'betaTesters' relationship dimension (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                AppsBetaTesterUsagesV1MetricResponse result = apiInstance.AppsBetaTesterUsagesGetMetrics(id, period, groupBy, filterBetaTesters, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.AppsBetaTesterUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppsBetaTesterUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppsBetaTesterUsagesV1MetricResponse> response = apiInstance.AppsBetaTesterUsagesGetMetricsWithHttpInfo(id, period, groupBy, filterBetaTesters, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.AppsBetaTesterUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **period** | **string?** | the duration of the reporting period | [optional]  |
| **groupBy** | [**List&lt;string&gt;?**](string.md) | the dimension by which to group the results | [optional]  |
| **filterBetaTesters** | **string?** | filter by &#39;betaTesters&#39; relationship dimension | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**AppsBetaTesterUsagesV1MetricResponse**](AppsBetaTesterUsagesV1MetricResponse.md)

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

<a id="betagroupsbetatesterusagesgetmetrics"></a>
# **BetaGroupsBetaTesterUsagesGetMetrics**
> AppsBetaTesterUsagesV1MetricResponse BetaGroupsBetaTesterUsagesGetMetrics (string id, string? period = null, List<string>? groupBy = null, string? filterBetaTesters = null, int? limit = null)



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
    public class BetaGroupsBetaTesterUsagesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var period = P7D;  // string? | the duration of the reporting period (optional) 
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterBetaTesters = "filterBetaTesters_example";  // string? | filter by 'betaTesters' relationship dimension (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                AppsBetaTesterUsagesV1MetricResponse result = apiInstance.BetaGroupsBetaTesterUsagesGetMetrics(id, period, groupBy, filterBetaTesters, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.BetaGroupsBetaTesterUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaTesterUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppsBetaTesterUsagesV1MetricResponse> response = apiInstance.BetaGroupsBetaTesterUsagesGetMetricsWithHttpInfo(id, period, groupBy, filterBetaTesters, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.BetaGroupsBetaTesterUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **period** | **string?** | the duration of the reporting period | [optional]  |
| **groupBy** | [**List&lt;string&gt;?**](string.md) | the dimension by which to group the results | [optional]  |
| **filterBetaTesters** | **string?** | filter by &#39;betaTesters&#39; relationship dimension | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**AppsBetaTesterUsagesV1MetricResponse**](AppsBetaTesterUsagesV1MetricResponse.md)

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

<a id="betagroupspubliclinkusagesgetmetrics"></a>
# **BetaGroupsPublicLinkUsagesGetMetrics**
> BetaPublicLinkUsagesV1MetricResponse BetaGroupsPublicLinkUsagesGetMetrics (string id, int? limit = null)



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
    public class BetaGroupsPublicLinkUsagesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                BetaPublicLinkUsagesV1MetricResponse result = apiInstance.BetaGroupsPublicLinkUsagesGetMetrics(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.BetaGroupsPublicLinkUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsPublicLinkUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaPublicLinkUsagesV1MetricResponse> response = apiInstance.BetaGroupsPublicLinkUsagesGetMetricsWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.BetaGroupsPublicLinkUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaPublicLinkUsagesV1MetricResponse**](BetaPublicLinkUsagesV1MetricResponse.md)

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

<a id="betatestersbetatesterusagesgetmetrics"></a>
# **BetaTestersBetaTesterUsagesGetMetrics**
> BetaTesterUsagesV1MetricResponse BetaTestersBetaTesterUsagesGetMetrics (string id, string filterApps, string? period = null, int? limit = null)



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
    public class BetaTestersBetaTesterUsagesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterApps = "filterApps_example";  // string | filter by 'apps' relationship dimension
            var period = P7D;  // string? | the duration of the reporting period (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                BetaTesterUsagesV1MetricResponse result = apiInstance.BetaTestersBetaTesterUsagesGetMetrics(id, filterApps, period, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.BetaTestersBetaTesterUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaTestersBetaTesterUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaTesterUsagesV1MetricResponse> response = apiInstance.BetaTestersBetaTesterUsagesGetMetricsWithHttpInfo(id, filterApps, period, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.BetaTestersBetaTesterUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterApps** | **string** | filter by &#39;apps&#39; relationship dimension |  |
| **period** | **string?** | the duration of the reporting period | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaTesterUsagesV1MetricResponse**](BetaTesterUsagesV1MetricResponse.md)

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

<a id="buildsbetabuildusagesgetmetrics"></a>
# **BuildsBetaBuildUsagesGetMetrics**
> BetaBuildUsagesV1MetricResponse BuildsBetaBuildUsagesGetMetrics (string id, int? limit = null)



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
    public class BuildsBetaBuildUsagesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                BetaBuildUsagesV1MetricResponse result = apiInstance.BuildsBetaBuildUsagesGetMetrics(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.BuildsBetaBuildUsagesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BuildsBetaBuildUsagesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildUsagesV1MetricResponse> response = apiInstance.BuildsBetaBuildUsagesGetMetricsWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.BuildsBetaBuildUsagesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaBuildUsagesV1MetricResponse**](BetaBuildUsagesV1MetricResponse.md)

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

<a id="gamecenterdetailsclassicmatchmakingrequestsgetmetrics"></a>
# **GameCenterDetailsClassicMatchmakingRequestsGetMetrics**
> GameCenterMatchmakingAppRequestsV1MetricResponse GameCenterDetailsClassicMatchmakingRequestsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterResult = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterDetailsClassicMatchmakingRequestsGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterResult = "MATCHED";  // string? | filter by 'result' attribute dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingAppRequestsV1MetricResponse result = apiInstance.GameCenterDetailsClassicMatchmakingRequestsGetMetrics(id, granularity, groupBy, filterResult, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterDetailsClassicMatchmakingRequestsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterDetailsClassicMatchmakingRequestsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingAppRequestsV1MetricResponse> response = apiInstance.GameCenterDetailsClassicMatchmakingRequestsGetMetricsWithHttpInfo(id, granularity, groupBy, filterResult, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterDetailsClassicMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingAppRequestsV1MetricResponse**](GameCenterMatchmakingAppRequestsV1MetricResponse.md)

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

<a id="gamecenterdetailsrulebasedmatchmakingrequestsgetmetrics"></a>
# **GameCenterDetailsRuleBasedMatchmakingRequestsGetMetrics**
> GameCenterMatchmakingAppRequestsV1MetricResponse GameCenterDetailsRuleBasedMatchmakingRequestsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterResult = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterDetailsRuleBasedMatchmakingRequestsGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterResult = "MATCHED";  // string? | filter by 'result' attribute dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingAppRequestsV1MetricResponse result = apiInstance.GameCenterDetailsRuleBasedMatchmakingRequestsGetMetrics(id, granularity, groupBy, filterResult, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterDetailsRuleBasedMatchmakingRequestsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterDetailsRuleBasedMatchmakingRequestsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingAppRequestsV1MetricResponse> response = apiInstance.GameCenterDetailsRuleBasedMatchmakingRequestsGetMetricsWithHttpInfo(id, granularity, groupBy, filterResult, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterDetailsRuleBasedMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingAppRequestsV1MetricResponse**](GameCenterMatchmakingAppRequestsV1MetricResponse.md)

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

<a id="gamecentermatchmakingqueuesexperimentmatchmakingqueuesizesgetmetrics"></a>
# **GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics**
> GameCenterMatchmakingQueueSizesV1MetricResponse GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics (string id, string granularity, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingQueueSizesV1MetricResponse result = apiInstance.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics(id, granularity, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueSizesV1MetricResponse> response = apiInstance.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetricsWithHttpInfo(id, granularity, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingQueueSizesV1MetricResponse**](GameCenterMatchmakingQueueSizesV1MetricResponse.md)

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

<a id="gamecentermatchmakingqueuesexperimentmatchmakingrequestsgetmetrics"></a>
# **GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics**
> GameCenterMatchmakingQueueRequestsV1MetricResponse GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterResult = null, string? filterGameCenterDetail = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterResult = "MATCHED";  // string? | filter by 'result' attribute dimension (optional) 
            var filterGameCenterDetail = "filterGameCenterDetail_example";  // string? | filter by 'gameCenterDetail' relationship dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingQueueRequestsV1MetricResponse result = apiInstance.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics(id, granularity, groupBy, filterResult, filterGameCenterDetail, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueRequestsV1MetricResponse> response = apiInstance.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetricsWithHttpInfo(id, granularity, groupBy, filterResult, filterGameCenterDetail, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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
| **filterGameCenterDetail** | **string?** | filter by &#39;gameCenterDetail&#39; relationship dimension | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingQueueRequestsV1MetricResponse**](GameCenterMatchmakingQueueRequestsV1MetricResponse.md)

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

<a id="gamecentermatchmakingqueuesmatchmakingqueuesizesgetmetrics"></a>
# **GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics**
> GameCenterMatchmakingQueueSizesV1MetricResponse GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics (string id, string granularity, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingQueueSizesV1MetricResponse result = apiInstance.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics(id, granularity, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueSizesV1MetricResponse> response = apiInstance.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetricsWithHttpInfo(id, granularity, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingQueueSizesV1MetricResponse**](GameCenterMatchmakingQueueSizesV1MetricResponse.md)

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

<a id="gamecentermatchmakingqueuesmatchmakingrequestsgetmetrics"></a>
# **GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics**
> GameCenterMatchmakingQueueRequestsV1MetricResponse GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics (string id, string granularity, List<string>? groupBy = null, string? filterResult = null, string? filterGameCenterDetail = null, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingQueuesMatchmakingRequestsGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var groupBy = new List<string>?(); // List<string>? | the dimension by which to group the results (optional) 
            var filterResult = "MATCHED";  // string? | filter by 'result' attribute dimension (optional) 
            var filterGameCenterDetail = "filterGameCenterDetail_example";  // string? | filter by 'gameCenterDetail' relationship dimension (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingQueueRequestsV1MetricResponse result = apiInstance.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics(id, granularity, groupBy, filterResult, filterGameCenterDetail, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesMatchmakingRequestsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueRequestsV1MetricResponse> response = apiInstance.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetricsWithHttpInfo(id, granularity, groupBy, filterResult, filterGameCenterDetail, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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
| **filterGameCenterDetail** | **string?** | filter by &#39;gameCenterDetail&#39; relationship dimension | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingQueueRequestsV1MetricResponse**](GameCenterMatchmakingQueueRequestsV1MetricResponse.md)

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

<a id="gamecentermatchmakingqueuesmatchmakingsessionsgetmetrics"></a>
# **GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics**
> GameCenterMatchmakingSessionsV1MetricResponse GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics (string id, string granularity, List<string>? sort = null, int? limit = null)



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
    public class GameCenterMatchmakingQueuesMatchmakingSessionsGetMetricsExample
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var granularity = P7D;  // string | the granularity of the per-group dataset
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; metrics will be sorted as specified (optional) 
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                GameCenterMatchmakingSessionsV1MetricResponse result = apiInstance.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics(id, granularity, sort, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesMatchmakingSessionsGetMetricsWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingSessionsV1MetricResponse> response = apiInstance.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetricsWithHttpInfo(id, granularity, sort, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetricsWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **granularity** | **string** | the granularity of the per-group dataset |  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; metrics will be sorted as specified | [optional]  |
| **limit** | **int?** | maximum number of groups to return per page | [optional]  |

### Return type

[**GameCenterMatchmakingSessionsV1MetricResponse**](GameCenterMatchmakingSessionsV1MetricResponse.md)

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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingBooleanRuleResultsGetMetricsWithHttpInfo: " + e.Message);
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingNumberRuleResultsGetMetricsWithHttpInfo: " + e.Message);
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
            var apiInstance = new MetricsApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling MetricsApi.GameCenterMatchmakingRulesMatchmakingRuleErrorsGetMetricsWithHttpInfo: " + e.Message);
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

