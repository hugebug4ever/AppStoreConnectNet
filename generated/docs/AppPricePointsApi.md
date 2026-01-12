# AppStoreConnect.Net.Api.AppPricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppPricePointsV3EqualizationsGetToManyRelated**](AppPricePointsApi.md#apppricepointsv3equalizationsgettomanyrelated) | **GET** /v3/appPricePoints/{id}/equalizations |  |
| [**AppPricePointsV3EqualizationsGetToManyRelationship**](AppPricePointsApi.md#apppricepointsv3equalizationsgettomanyrelationship) | **GET** /v3/appPricePoints/{id}/relationships/equalizations |  |
| [**AppPricePointsV3GetInstance**](AppPricePointsApi.md#apppricepointsv3getinstance) | **GET** /v3/appPricePoints/{id} |  |

<a id="apppricepointsv3equalizationsgettomanyrelated"></a>
# **AppPricePointsV3EqualizationsGetToManyRelated**
> AppPricePointsV3Response AppPricePointsV3EqualizationsGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsAppPricePoints = null, List<string>? fieldsApps = null, List<string>? fieldsTerritories = null, int? limit = null, List<string>? include = null)



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
    public class AppPricePointsV3EqualizationsGetToManyRelatedExample
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
            var apiInstance = new AppPricePointsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsAppPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPricePoints (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                AppPricePointsV3Response result = apiInstance.AppPricePointsV3EqualizationsGetToManyRelated(id, filterTerritory, fieldsAppPricePoints, fieldsApps, fieldsTerritories, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3EqualizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppPricePointsV3EqualizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPricePointsV3Response> response = apiInstance.AppPricePointsV3EqualizationsGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsAppPricePoints, fieldsApps, fieldsTerritories, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3EqualizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricePointsV3Response**](AppPricePointsV3Response.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of AppPricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apppricepointsv3equalizationsgettomanyrelationship"></a>
# **AppPricePointsV3EqualizationsGetToManyRelationship**
> AppPricePointV3EqualizationsLinkagesResponse AppPricePointsV3EqualizationsGetToManyRelationship (string id, int? limit = null)



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
    public class AppPricePointsV3EqualizationsGetToManyRelationshipExample
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
            var apiInstance = new AppPricePointsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppPricePointV3EqualizationsLinkagesResponse result = apiInstance.AppPricePointsV3EqualizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3EqualizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppPricePointsV3EqualizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPricePointV3EqualizationsLinkagesResponse> response = apiInstance.AppPricePointsV3EqualizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3EqualizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppPricePointV3EqualizationsLinkagesResponse**](AppPricePointV3EqualizationsLinkagesResponse.md)

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

<a id="apppricepointsv3getinstance"></a>
# **AppPricePointsV3GetInstance**
> AppPricePointV3Response AppPricePointsV3GetInstance (string id, List<string>? fieldsAppPricePoints = null, List<string>? include = null)



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
    public class AppPricePointsV3GetInstanceExample
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
            var apiInstance = new AppPricePointsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPricePoints (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                AppPricePointV3Response result = apiInstance.AppPricePointsV3GetInstance(id, fieldsAppPricePoints, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppPricePointsV3GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPricePointV3Response> response = apiInstance.AppPricePointsV3GetInstanceWithHttpInfo(id, fieldsAppPricePoints, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppPricePointsApi.AppPricePointsV3GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPricePoints | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppPricePointV3Response**](AppPricePointV3Response.md)

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
| **200** | Single AppPricePoint |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

