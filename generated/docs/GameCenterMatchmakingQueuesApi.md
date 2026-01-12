# AppStoreConnect.Net.Api.GameCenterMatchmakingQueuesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterMatchmakingQueuesCreateInstance**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuescreateinstance) | **POST** /v1/gameCenterMatchmakingQueues |  |
| [**GameCenterMatchmakingQueuesDeleteInstance**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesdeleteinstance) | **DELETE** /v1/gameCenterMatchmakingQueues/{id} |  |
| [**GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesexperimentmatchmakingqueuesizesgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingQueueSizes |  |
| [**GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesexperimentmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingRequests |  |
| [**GameCenterMatchmakingQueuesGetCollection**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesgetcollection) | **GET** /v1/gameCenterMatchmakingQueues |  |
| [**GameCenterMatchmakingQueuesGetInstance**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesgetinstance) | **GET** /v1/gameCenterMatchmakingQueues/{id} |  |
| [**GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesmatchmakingqueuesizesgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingQueueSizes |  |
| [**GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesmatchmakingrequestsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingRequests |  |
| [**GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesmatchmakingsessionsgetmetrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingSessions |  |
| [**GameCenterMatchmakingQueuesUpdateInstance**](GameCenterMatchmakingQueuesApi.md#gamecentermatchmakingqueuesupdateinstance) | **PATCH** /v1/gameCenterMatchmakingQueues/{id} |  |

<a id="gamecentermatchmakingqueuescreateinstance"></a>
# **GameCenterMatchmakingQueuesCreateInstance**
> GameCenterMatchmakingQueueResponse GameCenterMatchmakingQueuesCreateInstance (GameCenterMatchmakingQueueCreateRequest gameCenterMatchmakingQueueCreateRequest)



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
    public class GameCenterMatchmakingQueuesCreateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
            var gameCenterMatchmakingQueueCreateRequest = new GameCenterMatchmakingQueueCreateRequest(); // GameCenterMatchmakingQueueCreateRequest | GameCenterMatchmakingQueue representation

            try
            {
                GameCenterMatchmakingQueueResponse result = apiInstance.GameCenterMatchmakingQueuesCreateInstance(gameCenterMatchmakingQueueCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueResponse> response = apiInstance.GameCenterMatchmakingQueuesCreateInstanceWithHttpInfo(gameCenterMatchmakingQueueCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterMatchmakingQueueCreateRequest** | [**GameCenterMatchmakingQueueCreateRequest**](GameCenterMatchmakingQueueCreateRequest.md) | GameCenterMatchmakingQueue representation |  |

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
| **201** | Single GameCenterMatchmakingQueue |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingqueuesdeleteinstance"></a>
# **GameCenterMatchmakingQueuesDeleteInstance**
> void GameCenterMatchmakingQueuesDeleteInstance (string id)



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
    public class GameCenterMatchmakingQueuesDeleteInstanceExample
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.GameCenterMatchmakingQueuesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterMatchmakingQueuesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesDeleteInstanceWithHttpInfo: " + e.Message);
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesExperimentMatchmakingQueueSizesGetMetricsWithHttpInfo: " + e.Message);
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesExperimentMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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

<a id="gamecentermatchmakingqueuesgetcollection"></a>
# **GameCenterMatchmakingQueuesGetCollection**
> GameCenterMatchmakingQueuesResponse GameCenterMatchmakingQueuesGetCollection (List<string>? fieldsGameCenterMatchmakingQueues = null, int? limit = null, List<string>? include = null)



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
    public class GameCenterMatchmakingQueuesGetCollectionExample
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
            var fieldsGameCenterMatchmakingQueues = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterMatchmakingQueuesResponse result = apiInstance.GameCenterMatchmakingQueuesGetCollection(fieldsGameCenterMatchmakingQueues, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueuesResponse> response = apiInstance.GameCenterMatchmakingQueuesGetCollectionWithHttpInfo(fieldsGameCenterMatchmakingQueues, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
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
| **200** | List of GameCenterMatchmakingQueues |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecentermatchmakingqueuesgetinstance"></a>
# **GameCenterMatchmakingQueuesGetInstance**
> GameCenterMatchmakingQueueResponse GameCenterMatchmakingQueuesGetInstance (string id, List<string>? fieldsGameCenterMatchmakingQueues = null, List<string>? include = null)



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
    public class GameCenterMatchmakingQueuesGetInstanceExample
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterMatchmakingQueues = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                GameCenterMatchmakingQueueResponse result = apiInstance.GameCenterMatchmakingQueuesGetInstance(id, fieldsGameCenterMatchmakingQueues, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueResponse> response = apiInstance.GameCenterMatchmakingQueuesGetInstanceWithHttpInfo(id, fieldsGameCenterMatchmakingQueues, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterMatchmakingQueues** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
| **200** | Single GameCenterMatchmakingQueue |  -  |
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingQueueSizesGetMetricsWithHttpInfo: " + e.Message);
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingRequestsGetMetricsWithHttpInfo: " + e.Message);
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesMatchmakingSessionsGetMetricsWithHttpInfo: " + e.Message);
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

<a id="gamecentermatchmakingqueuesupdateinstance"></a>
# **GameCenterMatchmakingQueuesUpdateInstance**
> GameCenterMatchmakingQueueResponse GameCenterMatchmakingQueuesUpdateInstance (string id, GameCenterMatchmakingQueueUpdateRequest gameCenterMatchmakingQueueUpdateRequest)



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
    public class GameCenterMatchmakingQueuesUpdateInstanceExample
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
            var apiInstance = new GameCenterMatchmakingQueuesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterMatchmakingQueueUpdateRequest = new GameCenterMatchmakingQueueUpdateRequest(); // GameCenterMatchmakingQueueUpdateRequest | GameCenterMatchmakingQueue representation

            try
            {
                GameCenterMatchmakingQueueResponse result = apiInstance.GameCenterMatchmakingQueuesUpdateInstance(id, gameCenterMatchmakingQueueUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterMatchmakingQueuesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterMatchmakingQueueResponse> response = apiInstance.GameCenterMatchmakingQueuesUpdateInstanceWithHttpInfo(id, gameCenterMatchmakingQueueUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterMatchmakingQueuesApi.GameCenterMatchmakingQueuesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterMatchmakingQueueUpdateRequest** | [**GameCenterMatchmakingQueueUpdateRequest**](GameCenterMatchmakingQueueUpdateRequest.md) | GameCenterMatchmakingQueue representation |  |

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
| **200** | Single GameCenterMatchmakingQueue |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

