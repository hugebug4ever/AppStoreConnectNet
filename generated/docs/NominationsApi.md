# AppStoreConnect.Net.Api.NominationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**NominationsCreateInstance**](NominationsApi.md#nominationscreateinstance) | **POST** /v1/nominations |  |
| [**NominationsDeleteInstance**](NominationsApi.md#nominationsdeleteinstance) | **DELETE** /v1/nominations/{id} |  |
| [**NominationsGetCollection**](NominationsApi.md#nominationsgetcollection) | **GET** /v1/nominations |  |
| [**NominationsGetInstance**](NominationsApi.md#nominationsgetinstance) | **GET** /v1/nominations/{id} |  |
| [**NominationsUpdateInstance**](NominationsApi.md#nominationsupdateinstance) | **PATCH** /v1/nominations/{id} |  |

<a id="nominationscreateinstance"></a>
# **NominationsCreateInstance**
> NominationResponse NominationsCreateInstance (NominationCreateRequest nominationCreateRequest)



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
    public class NominationsCreateInstanceExample
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
            var apiInstance = new NominationsApi(httpClient, config, httpClientHandler);
            var nominationCreateRequest = new NominationCreateRequest(); // NominationCreateRequest | Nomination representation

            try
            {
                NominationResponse result = apiInstance.NominationsCreateInstance(nominationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NominationsApi.NominationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NominationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<NominationResponse> response = apiInstance.NominationsCreateInstanceWithHttpInfo(nominationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NominationsApi.NominationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **nominationCreateRequest** | [**NominationCreateRequest**](NominationCreateRequest.md) | Nomination representation |  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **201** | Single Nomination |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="nominationsdeleteinstance"></a>
# **NominationsDeleteInstance**
> void NominationsDeleteInstance (string id)



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
    public class NominationsDeleteInstanceExample
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
            var apiInstance = new NominationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.NominationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NominationsApi.NominationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NominationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.NominationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NominationsApi.NominationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="nominationsgetcollection"></a>
# **NominationsGetCollection**
> NominationsResponse NominationsGetCollection (List<string> filterState, List<string>? filterType = null, List<string>? filterRelatedApps = null, List<string>? sort = null, List<string>? fieldsNominations = null, int? limit = null, List<string>? include = null, int? limitInAppEvents = null, int? limitRelatedApps = null, int? limitSupportedTerritories = null)



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
    public class NominationsGetCollectionExample
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
            var apiInstance = new NominationsApi(httpClient, config, httpClientHandler);
            var filterState = new List<string>(); // List<string> | filter by attribute 'state'
            var filterType = new List<string>?(); // List<string>? | filter by attribute 'type' (optional) 
            var filterRelatedApps = new List<string>?(); // List<string>? | filter by id(s) of related 'relatedApps' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsNominations = new List<string>?(); // List<string>? | the fields to include for returned resources of type nominations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitInAppEvents = 56;  // int? | maximum number of related inAppEvents returned (when they are included) (optional) 
            var limitRelatedApps = 56;  // int? | maximum number of related relatedApps returned (when they are included) (optional) 
            var limitSupportedTerritories = 56;  // int? | maximum number of related supportedTerritories returned (when they are included) (optional) 

            try
            {
                NominationsResponse result = apiInstance.NominationsGetCollection(filterState, filterType, filterRelatedApps, sort, fieldsNominations, limit, include, limitInAppEvents, limitRelatedApps, limitSupportedTerritories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NominationsApi.NominationsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NominationsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<NominationsResponse> response = apiInstance.NominationsGetCollectionWithHttpInfo(filterState, filterType, filterRelatedApps, sort, fieldsNominations, limit, include, limitInAppEvents, limitRelatedApps, limitSupportedTerritories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NominationsApi.NominationsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; |  |
| **filterType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;type&#39; | [optional]  |
| **filterRelatedApps** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;relatedApps&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsNominations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type nominations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitInAppEvents** | **int?** | maximum number of related inAppEvents returned (when they are included) | [optional]  |
| **limitRelatedApps** | **int?** | maximum number of related relatedApps returned (when they are included) | [optional]  |
| **limitSupportedTerritories** | **int?** | maximum number of related supportedTerritories returned (when they are included) | [optional]  |

### Return type

[**NominationsResponse**](NominationsResponse.md)

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
| **200** | List of Nominations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="nominationsgetinstance"></a>
# **NominationsGetInstance**
> NominationResponse NominationsGetInstance (string id, List<string>? fieldsNominations = null, List<string>? include = null, int? limitInAppEvents = null, int? limitRelatedApps = null, int? limitSupportedTerritories = null)



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
    public class NominationsGetInstanceExample
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
            var apiInstance = new NominationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsNominations = new List<string>?(); // List<string>? | the fields to include for returned resources of type nominations (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitInAppEvents = 56;  // int? | maximum number of related inAppEvents returned (when they are included) (optional) 
            var limitRelatedApps = 56;  // int? | maximum number of related relatedApps returned (when they are included) (optional) 
            var limitSupportedTerritories = 56;  // int? | maximum number of related supportedTerritories returned (when they are included) (optional) 

            try
            {
                NominationResponse result = apiInstance.NominationsGetInstance(id, fieldsNominations, include, limitInAppEvents, limitRelatedApps, limitSupportedTerritories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NominationsApi.NominationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NominationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<NominationResponse> response = apiInstance.NominationsGetInstanceWithHttpInfo(id, fieldsNominations, include, limitInAppEvents, limitRelatedApps, limitSupportedTerritories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NominationsApi.NominationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsNominations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type nominations | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitInAppEvents** | **int?** | maximum number of related inAppEvents returned (when they are included) | [optional]  |
| **limitRelatedApps** | **int?** | maximum number of related relatedApps returned (when they are included) | [optional]  |
| **limitSupportedTerritories** | **int?** | maximum number of related supportedTerritories returned (when they are included) | [optional]  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **200** | Single Nomination |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="nominationsupdateinstance"></a>
# **NominationsUpdateInstance**
> NominationResponse NominationsUpdateInstance (string id, NominationUpdateRequest nominationUpdateRequest)



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
    public class NominationsUpdateInstanceExample
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
            var apiInstance = new NominationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var nominationUpdateRequest = new NominationUpdateRequest(); // NominationUpdateRequest | Nomination representation

            try
            {
                NominationResponse result = apiInstance.NominationsUpdateInstance(id, nominationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NominationsApi.NominationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NominationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<NominationResponse> response = apiInstance.NominationsUpdateInstanceWithHttpInfo(id, nominationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NominationsApi.NominationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **nominationUpdateRequest** | [**NominationUpdateRequest**](NominationUpdateRequest.md) | Nomination representation |  |

### Return type

[**NominationResponse**](NominationResponse.md)

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
| **200** | Single Nomination |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

