# AppStoreConnect.Net.Api.BetaGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaGroupsAppGetToOneRelated**](BetaGroupsApi.md#betagroupsappgettoonerelated) | **GET** /v1/betaGroups/{id}/app |  |
| [**BetaGroupsAppGetToOneRelationship**](BetaGroupsApi.md#betagroupsappgettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/app |  |
| [**BetaGroupsBetaRecruitmentCriteriaGetToOneRelated**](BetaGroupsApi.md#betagroupsbetarecruitmentcriteriagettoonerelated) | **GET** /v1/betaGroups/{id}/betaRecruitmentCriteria |  |
| [**BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship**](BetaGroupsApi.md#betagroupsbetarecruitmentcriteriagettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/betaRecruitmentCriteria |  |
| [**BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated**](BetaGroupsApi.md#betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelated) | **GET** /v1/betaGroups/{id}/betaRecruitmentCriterionCompatibleBuildCheck |  |
| [**BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship**](BetaGroupsApi.md#betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/betaRecruitmentCriterionCompatibleBuildCheck |  |
| [**BetaGroupsBetaTesterUsagesGetMetrics**](BetaGroupsApi.md#betagroupsbetatesterusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/betaTesterUsages |  |
| [**BetaGroupsBetaTestersCreateToManyRelationship**](BetaGroupsApi.md#betagroupsbetatesterscreatetomanyrelationship) | **POST** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBetaTestersDeleteToManyRelationship**](BetaGroupsApi.md#betagroupsbetatestersdeletetomanyrelationship) | **DELETE** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBetaTestersGetToManyRelated**](BetaGroupsApi.md#betagroupsbetatestersgettomanyrelated) | **GET** /v1/betaGroups/{id}/betaTesters |  |
| [**BetaGroupsBetaTestersGetToManyRelationship**](BetaGroupsApi.md#betagroupsbetatestersgettomanyrelationship) | **GET** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBuildsCreateToManyRelationship**](BetaGroupsApi.md#betagroupsbuildscreatetomanyrelationship) | **POST** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsBuildsDeleteToManyRelationship**](BetaGroupsApi.md#betagroupsbuildsdeletetomanyrelationship) | **DELETE** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsBuildsGetToManyRelated**](BetaGroupsApi.md#betagroupsbuildsgettomanyrelated) | **GET** /v1/betaGroups/{id}/builds |  |
| [**BetaGroupsBuildsGetToManyRelationship**](BetaGroupsApi.md#betagroupsbuildsgettomanyrelationship) | **GET** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsCreateInstance**](BetaGroupsApi.md#betagroupscreateinstance) | **POST** /v1/betaGroups |  |
| [**BetaGroupsDeleteInstance**](BetaGroupsApi.md#betagroupsdeleteinstance) | **DELETE** /v1/betaGroups/{id} |  |
| [**BetaGroupsGetCollection**](BetaGroupsApi.md#betagroupsgetcollection) | **GET** /v1/betaGroups |  |
| [**BetaGroupsGetInstance**](BetaGroupsApi.md#betagroupsgetinstance) | **GET** /v1/betaGroups/{id} |  |
| [**BetaGroupsPublicLinkUsagesGetMetrics**](BetaGroupsApi.md#betagroupspubliclinkusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/publicLinkUsages |  |
| [**BetaGroupsUpdateInstance**](BetaGroupsApi.md#betagroupsupdateinstance) | **PATCH** /v1/betaGroups/{id} |  |

<a id="betagroupsappgettoonerelated"></a>
# **BetaGroupsAppGetToOneRelated**
> AppWithoutIncludesResponse BetaGroupsAppGetToOneRelated (string id, List<string>? fieldsApps = null)



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
    public class BetaGroupsAppGetToOneRelatedExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 

            try
            {
                AppWithoutIncludesResponse result = apiInstance.BetaGroupsAppGetToOneRelated(id, fieldsApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsAppGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsAppGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppWithoutIncludesResponse> response = apiInstance.BetaGroupsAppGetToOneRelatedWithHttpInfo(id, fieldsApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsAppGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsappgettoonerelationship"></a>
# **BetaGroupsAppGetToOneRelationship**
> BetaGroupAppLinkageResponse BetaGroupsAppGetToOneRelationship (string id)



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
    public class BetaGroupsAppGetToOneRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaGroupAppLinkageResponse result = apiInstance.BetaGroupsAppGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsAppGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsAppGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupAppLinkageResponse> response = apiInstance.BetaGroupsAppGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsAppGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupAppLinkageResponse**](BetaGroupAppLinkageResponse.md)

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

<a id="betagroupsbetarecruitmentcriteriagettoonerelated"></a>
# **BetaGroupsBetaRecruitmentCriteriaGetToOneRelated**
> BetaRecruitmentCriterionResponse BetaGroupsBetaRecruitmentCriteriaGetToOneRelated (string id, List<string>? fieldsBetaRecruitmentCriteria = null)



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
    public class BetaGroupsBetaRecruitmentCriteriaGetToOneRelatedExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaRecruitmentCriteria = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaRecruitmentCriteria (optional) 

            try
            {
                BetaRecruitmentCriterionResponse result = apiInstance.BetaGroupsBetaRecruitmentCriteriaGetToOneRelated(id, fieldsBetaRecruitmentCriteria);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriteriaGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaRecruitmentCriteriaGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaRecruitmentCriterionResponse> response = apiInstance.BetaGroupsBetaRecruitmentCriteriaGetToOneRelatedWithHttpInfo(id, fieldsBetaRecruitmentCriteria);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriteriaGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **200** | Single BetaRecruitmentCriterion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsbetarecruitmentcriteriagettoonerelationship"></a>
# **BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship**
> BetaGroupBetaRecruitmentCriteriaLinkageResponse BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship (string id)



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
    public class BetaGroupsBetaRecruitmentCriteriaGetToOneRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaGroupBetaRecruitmentCriteriaLinkageResponse result = apiInstance.BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaRecruitmentCriteriaGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupBetaRecruitmentCriteriaLinkageResponse> response = apiInstance.BetaGroupsBetaRecruitmentCriteriaGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriteriaGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupBetaRecruitmentCriteriaLinkageResponse**](BetaGroupBetaRecruitmentCriteriaLinkageResponse.md)

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

<a id="betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelated"></a>
# **BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated**
> BetaRecruitmentCriterionCompatibleBuildCheckResponse BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated (string id, List<string>? fieldsBetaRecruitmentCriterionCompatibleBuildChecks = null)



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
    public class BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelatedExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaRecruitmentCriterionCompatibleBuildChecks = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaRecruitmentCriterionCompatibleBuildChecks (optional) 

            try
            {
                BetaRecruitmentCriterionCompatibleBuildCheckResponse result = apiInstance.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated(id, fieldsBetaRecruitmentCriterionCompatibleBuildChecks);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaRecruitmentCriterionCompatibleBuildCheckResponse> response = apiInstance.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelatedWithHttpInfo(id, fieldsBetaRecruitmentCriterionCompatibleBuildChecks);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaRecruitmentCriterionCompatibleBuildChecks** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaRecruitmentCriterionCompatibleBuildChecks | [optional]  |

### Return type

[**BetaRecruitmentCriterionCompatibleBuildCheckResponse**](BetaRecruitmentCriterionCompatibleBuildCheckResponse.md)

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
| **200** | Single BetaRecruitmentCriterionCompatibleBuildCheck |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelationship"></a>
# **BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship**
> BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship (string id)



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
    public class BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse result = apiInstance.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse> response = apiInstance.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse**](BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse.md)

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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
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
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTesterUsagesGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTesterUsagesGetMetricsWithHttpInfo: " + e.Message);
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

<a id="betagroupsbetatesterscreatetomanyrelationship"></a>
# **BetaGroupsBetaTestersCreateToManyRelationship**
> void BetaGroupsBetaTestersCreateToManyRelationship (string id, BetaGroupBetaTestersLinkagesRequest betaGroupBetaTestersLinkagesRequest)



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
    public class BetaGroupsBetaTestersCreateToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaGroupBetaTestersLinkagesRequest = new BetaGroupBetaTestersLinkagesRequest(); // BetaGroupBetaTestersLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BetaGroupsBetaTestersCreateToManyRelationship(id, betaGroupBetaTestersLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaTestersCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaGroupsBetaTestersCreateToManyRelationshipWithHttpInfo(id, betaGroupBetaTestersLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBetaTestersLinkagesRequest** | [**BetaGroupBetaTestersLinkagesRequest**](BetaGroupBetaTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbetatestersdeletetomanyrelationship"></a>
# **BetaGroupsBetaTestersDeleteToManyRelationship**
> void BetaGroupsBetaTestersDeleteToManyRelationship (string id, BetaGroupBetaTestersLinkagesRequest betaGroupBetaTestersLinkagesRequest)



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
    public class BetaGroupsBetaTestersDeleteToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaGroupBetaTestersLinkagesRequest = new BetaGroupBetaTestersLinkagesRequest(); // BetaGroupBetaTestersLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BetaGroupsBetaTestersDeleteToManyRelationship(id, betaGroupBetaTestersLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaTestersDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaGroupsBetaTestersDeleteToManyRelationshipWithHttpInfo(id, betaGroupBetaTestersLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBetaTestersLinkagesRequest** | [**BetaGroupBetaTestersLinkagesRequest**](BetaGroupBetaTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbetatestersgettomanyrelated"></a>
# **BetaGroupsBetaTestersGetToManyRelated**
> BetaTestersWithoutIncludesResponse BetaGroupsBetaTestersGetToManyRelated (string id, List<string>? fieldsBetaTesters = null, int? limit = null)



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
    public class BetaGroupsBetaTestersGetToManyRelatedExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BetaTestersWithoutIncludesResponse result = apiInstance.BetaGroupsBetaTestersGetToManyRelated(id, fieldsBetaTesters, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaTestersGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaTestersWithoutIncludesResponse> response = apiInstance.BetaGroupsBetaTestersGetToManyRelatedWithHttpInfo(id, fieldsBetaTesters, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaTesters** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BetaTestersWithoutIncludesResponse**](BetaTestersWithoutIncludesResponse.md)

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
| **200** | List of BetaTesters with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsbetatestersgettomanyrelationship"></a>
# **BetaGroupsBetaTestersGetToManyRelationship**
> BetaGroupBetaTestersLinkagesResponse BetaGroupsBetaTestersGetToManyRelationship (string id, int? limit = null)



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
    public class BetaGroupsBetaTestersGetToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BetaGroupBetaTestersLinkagesResponse result = apiInstance.BetaGroupsBetaTestersGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBetaTestersGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupBetaTestersLinkagesResponse> response = apiInstance.BetaGroupsBetaTestersGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBetaTestersGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BetaGroupBetaTestersLinkagesResponse**](BetaGroupBetaTestersLinkagesResponse.md)

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

<a id="betagroupsbuildscreatetomanyrelationship"></a>
# **BetaGroupsBuildsCreateToManyRelationship**
> void BetaGroupsBuildsCreateToManyRelationship (string id, BetaGroupBuildsLinkagesRequest betaGroupBuildsLinkagesRequest)



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
    public class BetaGroupsBuildsCreateToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaGroupBuildsLinkagesRequest = new BetaGroupBuildsLinkagesRequest(); // BetaGroupBuildsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BetaGroupsBuildsCreateToManyRelationship(id, betaGroupBuildsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBuildsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaGroupsBuildsCreateToManyRelationshipWithHttpInfo(id, betaGroupBuildsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBuildsLinkagesRequest** | [**BetaGroupBuildsLinkagesRequest**](BetaGroupBuildsLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbuildsdeletetomanyrelationship"></a>
# **BetaGroupsBuildsDeleteToManyRelationship**
> void BetaGroupsBuildsDeleteToManyRelationship (string id, BetaGroupBuildsLinkagesRequest betaGroupBuildsLinkagesRequest)



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
    public class BetaGroupsBuildsDeleteToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaGroupBuildsLinkagesRequest = new BetaGroupBuildsLinkagesRequest(); // BetaGroupBuildsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.BetaGroupsBuildsDeleteToManyRelationship(id, betaGroupBuildsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBuildsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaGroupsBuildsDeleteToManyRelationshipWithHttpInfo(id, betaGroupBuildsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBuildsLinkagesRequest** | [**BetaGroupBuildsLinkagesRequest**](BetaGroupBuildsLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbuildsgettomanyrelated"></a>
# **BetaGroupsBuildsGetToManyRelated**
> BuildsWithoutIncludesResponse BetaGroupsBuildsGetToManyRelated (string id, List<string>? fieldsBuilds = null, int? limit = null)



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
    public class BetaGroupsBuildsGetToManyRelatedExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BuildsWithoutIncludesResponse result = apiInstance.BetaGroupsBuildsGetToManyRelated(id, fieldsBuilds, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBuildsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildsWithoutIncludesResponse> response = apiInstance.BetaGroupsBuildsGetToManyRelatedWithHttpInfo(id, fieldsBuilds, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**BuildsWithoutIncludesResponse**](BuildsWithoutIncludesResponse.md)

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
| **200** | List of Builds with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsbuildsgettomanyrelationship"></a>
# **BetaGroupsBuildsGetToManyRelationship**
> BetaGroupBuildsLinkagesResponse BetaGroupsBuildsGetToManyRelationship (string id, int? limit = null)



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
    public class BetaGroupsBuildsGetToManyRelationshipExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                BetaGroupBuildsLinkagesResponse result = apiInstance.BetaGroupsBuildsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsBuildsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupBuildsLinkagesResponse> response = apiInstance.BetaGroupsBuildsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsBuildsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**BetaGroupBuildsLinkagesResponse**](BetaGroupBuildsLinkagesResponse.md)

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

<a id="betagroupscreateinstance"></a>
# **BetaGroupsCreateInstance**
> BetaGroupResponse BetaGroupsCreateInstance (BetaGroupCreateRequest betaGroupCreateRequest)



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
    public class BetaGroupsCreateInstanceExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var betaGroupCreateRequest = new BetaGroupCreateRequest(); // BetaGroupCreateRequest | BetaGroup representation

            try
            {
                BetaGroupResponse result = apiInstance.BetaGroupsCreateInstance(betaGroupCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupResponse> response = apiInstance.BetaGroupsCreateInstanceWithHttpInfo(betaGroupCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaGroupCreateRequest** | [**BetaGroupCreateRequest**](BetaGroupCreateRequest.md) | BetaGroup representation |  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **201** | Single BetaGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsdeleteinstance"></a>
# **BetaGroupsDeleteInstance**
> void BetaGroupsDeleteInstance (string id)



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
    public class BetaGroupsDeleteInstanceExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.BetaGroupsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaGroupsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="betagroupsgetcollection"></a>
# **BetaGroupsGetCollection**
> BetaGroupsResponse BetaGroupsGetCollection (List<string>? filterName = null, List<string>? filterIsInternalGroup = null, List<string>? filterPublicLinkEnabled = null, List<string>? filterPublicLinkLimitEnabled = null, List<string>? filterPublicLink = null, List<string>? filterApp = null, List<string>? filterBuilds = null, List<string>? filterId = null, List<string>? sort = null, List<string>? fieldsBetaGroups = null, List<string>? fieldsApps = null, List<string>? fieldsBuilds = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaRecruitmentCriteria = null, int? limit = null, List<string>? include = null, int? limitBetaTesters = null, int? limitBuilds = null)



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
    public class BetaGroupsGetCollectionExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var filterName = new List<string>?(); // List<string>? | filter by attribute 'name' (optional) 
            var filterIsInternalGroup = new List<string>?(); // List<string>? | filter by attribute 'isInternalGroup' (optional) 
            var filterPublicLinkEnabled = new List<string>?(); // List<string>? | filter by attribute 'publicLinkEnabled' (optional) 
            var filterPublicLinkLimitEnabled = new List<string>?(); // List<string>? | filter by attribute 'publicLinkLimitEnabled' (optional) 
            var filterPublicLink = new List<string>?(); // List<string>? | filter by attribute 'publicLink' (optional) 
            var filterApp = new List<string>?(); // List<string>? | filter by id(s) of related 'app' (optional) 
            var filterBuilds = new List<string>?(); // List<string>? | filter by id(s) of related 'builds' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsBetaGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaGroups (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var fieldsBetaRecruitmentCriteria = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaRecruitmentCriteria (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBetaTesters = 56;  // int? | maximum number of related betaTesters returned (when they are included) (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                BetaGroupsResponse result = apiInstance.BetaGroupsGetCollection(filterName, filterIsInternalGroup, filterPublicLinkEnabled, filterPublicLinkLimitEnabled, filterPublicLink, filterApp, filterBuilds, filterId, sort, fieldsBetaGroups, fieldsApps, fieldsBuilds, fieldsBetaTesters, fieldsBetaRecruitmentCriteria, limit, include, limitBetaTesters, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupsResponse> response = apiInstance.BetaGroupsGetCollectionWithHttpInfo(filterName, filterIsInternalGroup, filterPublicLinkEnabled, filterPublicLinkLimitEnabled, filterPublicLink, filterApp, filterBuilds, filterId, sort, fieldsBetaGroups, fieldsApps, fieldsBuilds, fieldsBetaTesters, fieldsBetaRecruitmentCriteria, limit, include, limitBetaTesters, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIsInternalGroup** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;isInternalGroup&#39; | [optional]  |
| **filterPublicLinkEnabled** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;publicLinkEnabled&#39; | [optional]  |
| **filterPublicLinkLimitEnabled** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;publicLinkLimitEnabled&#39; | [optional]  |
| **filterPublicLink** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;publicLink&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaTesters** | **int?** | maximum number of related betaTesters returned (when they are included) | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaGroupsResponse**](BetaGroupsResponse.md)

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
| **200** | List of BetaGroups |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betagroupsgetinstance"></a>
# **BetaGroupsGetInstance**
> BetaGroupResponse BetaGroupsGetInstance (string id, List<string>? fieldsBetaGroups = null, List<string>? fieldsApps = null, List<string>? fieldsBuilds = null, List<string>? fieldsBetaTesters = null, List<string>? fieldsBetaRecruitmentCriteria = null, List<string>? include = null, int? limitBetaTesters = null, int? limitBuilds = null)



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
    public class BetaGroupsGetInstanceExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaGroups = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaGroups (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsBetaTesters = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaTesters (optional) 
            var fieldsBetaRecruitmentCriteria = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaRecruitmentCriteria (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitBetaTesters = 56;  // int? | maximum number of related betaTesters returned (when they are included) (optional) 
            var limitBuilds = 56;  // int? | maximum number of related builds returned (when they are included) (optional) 

            try
            {
                BetaGroupResponse result = apiInstance.BetaGroupsGetInstance(id, fieldsBetaGroups, fieldsApps, fieldsBuilds, fieldsBetaTesters, fieldsBetaRecruitmentCriteria, include, limitBetaTesters, limitBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupResponse> response = apiInstance.BetaGroupsGetInstanceWithHttpInfo(id, fieldsBetaGroups, fieldsApps, fieldsBuilds, fieldsBetaTesters, fieldsBetaRecruitmentCriteria, include, limitBetaTesters, limitBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaGroups** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaTesters** | **int?** | maximum number of related betaTesters returned (when they are included) | [optional]  |
| **limitBuilds** | **int?** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **200** | Single BetaGroup |  -  |
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum number of groups to return per page (optional) 

            try
            {
                BetaPublicLinkUsagesV1MetricResponse result = apiInstance.BetaGroupsPublicLinkUsagesGetMetrics(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsPublicLinkUsagesGetMetrics: " + e.Message);
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
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsPublicLinkUsagesGetMetricsWithHttpInfo: " + e.Message);
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

<a id="betagroupsupdateinstance"></a>
# **BetaGroupsUpdateInstance**
> BetaGroupResponse BetaGroupsUpdateInstance (string id, BetaGroupUpdateRequest betaGroupUpdateRequest)



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
    public class BetaGroupsUpdateInstanceExample
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
            var apiInstance = new BetaGroupsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaGroupUpdateRequest = new BetaGroupUpdateRequest(); // BetaGroupUpdateRequest | BetaGroup representation

            try
            {
                BetaGroupResponse result = apiInstance.BetaGroupsUpdateInstance(id, betaGroupUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaGroupsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaGroupResponse> response = apiInstance.BetaGroupsUpdateInstanceWithHttpInfo(id, betaGroupUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaGroupsApi.BetaGroupsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupUpdateRequest** | [**BetaGroupUpdateRequest**](BetaGroupUpdateRequest.md) | BetaGroup representation |  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **200** | Single BetaGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

