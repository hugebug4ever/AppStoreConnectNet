# AppStoreConnect.Net.Api.BetaBuildLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaBuildLocalizationsBuildGetToOneRelated**](BetaBuildLocalizationsApi.md#betabuildlocalizationsbuildgettoonerelated) | **GET** /v1/betaBuildLocalizations/{id}/build |  |
| [**BetaBuildLocalizationsBuildGetToOneRelationship**](BetaBuildLocalizationsApi.md#betabuildlocalizationsbuildgettoonerelationship) | **GET** /v1/betaBuildLocalizations/{id}/relationships/build |  |
| [**BetaBuildLocalizationsCreateInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationscreateinstance) | **POST** /v1/betaBuildLocalizations |  |
| [**BetaBuildLocalizationsDeleteInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsdeleteinstance) | **DELETE** /v1/betaBuildLocalizations/{id} |  |
| [**BetaBuildLocalizationsGetCollection**](BetaBuildLocalizationsApi.md#betabuildlocalizationsgetcollection) | **GET** /v1/betaBuildLocalizations |  |
| [**BetaBuildLocalizationsGetInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsgetinstance) | **GET** /v1/betaBuildLocalizations/{id} |  |
| [**BetaBuildLocalizationsUpdateInstance**](BetaBuildLocalizationsApi.md#betabuildlocalizationsupdateinstance) | **PATCH** /v1/betaBuildLocalizations/{id} |  |

<a id="betabuildlocalizationsbuildgettoonerelated"></a>
# **BetaBuildLocalizationsBuildGetToOneRelated**
> BuildWithoutIncludesResponse BetaBuildLocalizationsBuildGetToOneRelated (string id, List<string>? fieldsBuilds = null)



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
    public class BetaBuildLocalizationsBuildGetToOneRelatedExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 

            try
            {
                BuildWithoutIncludesResponse result = apiInstance.BetaBuildLocalizationsBuildGetToOneRelated(id, fieldsBuilds);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsBuildGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsBuildGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BuildWithoutIncludesResponse> response = apiInstance.BetaBuildLocalizationsBuildGetToOneRelatedWithHttpInfo(id, fieldsBuilds);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsBuildGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |

### Return type

[**BuildWithoutIncludesResponse**](BuildWithoutIncludesResponse.md)

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
| **200** | Single Build with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betabuildlocalizationsbuildgettoonerelationship"></a>
# **BetaBuildLocalizationsBuildGetToOneRelationship**
> BetaBuildLocalizationBuildLinkageResponse BetaBuildLocalizationsBuildGetToOneRelationship (string id)



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
    public class BetaBuildLocalizationsBuildGetToOneRelationshipExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                BetaBuildLocalizationBuildLinkageResponse result = apiInstance.BetaBuildLocalizationsBuildGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsBuildGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsBuildGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationBuildLinkageResponse> response = apiInstance.BetaBuildLocalizationsBuildGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsBuildGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaBuildLocalizationBuildLinkageResponse**](BetaBuildLocalizationBuildLinkageResponse.md)

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

<a id="betabuildlocalizationscreateinstance"></a>
# **BetaBuildLocalizationsCreateInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsCreateInstance (BetaBuildLocalizationCreateRequest betaBuildLocalizationCreateRequest)



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
    public class BetaBuildLocalizationsCreateInstanceExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var betaBuildLocalizationCreateRequest = new BetaBuildLocalizationCreateRequest(); // BetaBuildLocalizationCreateRequest | BetaBuildLocalization representation

            try
            {
                BetaBuildLocalizationResponse result = apiInstance.BetaBuildLocalizationsCreateInstance(betaBuildLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationResponse> response = apiInstance.BetaBuildLocalizationsCreateInstanceWithHttpInfo(betaBuildLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaBuildLocalizationCreateRequest** | [**BetaBuildLocalizationCreateRequest**](BetaBuildLocalizationCreateRequest.md) | BetaBuildLocalization representation |  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

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
| **201** | Single BetaBuildLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betabuildlocalizationsdeleteinstance"></a>
# **BetaBuildLocalizationsDeleteInstance**
> void BetaBuildLocalizationsDeleteInstance (string id)



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
    public class BetaBuildLocalizationsDeleteInstanceExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.BetaBuildLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.BetaBuildLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="betabuildlocalizationsgetcollection"></a>
# **BetaBuildLocalizationsGetCollection**
> BetaBuildLocalizationsResponse BetaBuildLocalizationsGetCollection (List<string>? filterLocale = null, List<string>? filterBuild = null, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsBuilds = null, int? limit = null, List<string>? include = null)



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
    public class BetaBuildLocalizationsGetCollectionExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var filterLocale = new List<string>?(); // List<string>? | filter by attribute 'locale' (optional) 
            var filterBuild = new List<string>?(); // List<string>? | filter by id(s) of related 'build' (optional) 
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaBuildLocalizationsResponse result = apiInstance.BetaBuildLocalizationsGetCollection(filterLocale, filterBuild, fieldsBetaBuildLocalizations, fieldsBuilds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationsResponse> response = apiInstance.BetaBuildLocalizationsGetCollectionWithHttpInfo(filterLocale, filterBuild, fieldsBetaBuildLocalizations, fieldsBuilds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterLocale** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **filterBuild** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;build&#39; | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaBuildLocalizationsResponse**](BetaBuildLocalizationsResponse.md)

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
| **200** | List of BetaBuildLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betabuildlocalizationsgetinstance"></a>
# **BetaBuildLocalizationsGetInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsGetInstance (string id, List<string>? fieldsBetaBuildLocalizations = null, List<string>? fieldsBuilds = null, List<string>? include = null)



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
    public class BetaBuildLocalizationsGetInstanceExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBetaBuildLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type betaBuildLocalizations (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BetaBuildLocalizationResponse result = apiInstance.BetaBuildLocalizationsGetInstance(id, fieldsBetaBuildLocalizations, fieldsBuilds, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationResponse> response = apiInstance.BetaBuildLocalizationsGetInstanceWithHttpInfo(id, fieldsBetaBuildLocalizations, fieldsBuilds, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

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
| **200** | Single BetaBuildLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="betabuildlocalizationsupdateinstance"></a>
# **BetaBuildLocalizationsUpdateInstance**
> BetaBuildLocalizationResponse BetaBuildLocalizationsUpdateInstance (string id, BetaBuildLocalizationUpdateRequest betaBuildLocalizationUpdateRequest)



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
    public class BetaBuildLocalizationsUpdateInstanceExample
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
            var apiInstance = new BetaBuildLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var betaBuildLocalizationUpdateRequest = new BetaBuildLocalizationUpdateRequest(); // BetaBuildLocalizationUpdateRequest | BetaBuildLocalization representation

            try
            {
                BetaBuildLocalizationResponse result = apiInstance.BetaBuildLocalizationsUpdateInstance(id, betaBuildLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BetaBuildLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BetaBuildLocalizationResponse> response = apiInstance.BetaBuildLocalizationsUpdateInstanceWithHttpInfo(id, betaBuildLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BetaBuildLocalizationsApi.BetaBuildLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaBuildLocalizationUpdateRequest** | [**BetaBuildLocalizationUpdateRequest**](BetaBuildLocalizationUpdateRequest.md) | BetaBuildLocalization representation |  |

### Return type

[**BetaBuildLocalizationResponse**](BetaBuildLocalizationResponse.md)

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
| **200** | Single BetaBuildLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

