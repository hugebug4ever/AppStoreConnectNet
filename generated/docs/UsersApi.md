# AppStoreConnect.Net.Api.UsersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**UsersDeleteInstance**](UsersApi.md#usersdeleteinstance) | **DELETE** /v1/users/{id} |  |
| [**UsersGetCollection**](UsersApi.md#usersgetcollection) | **GET** /v1/users |  |
| [**UsersGetInstance**](UsersApi.md#usersgetinstance) | **GET** /v1/users/{id} |  |
| [**UsersUpdateInstance**](UsersApi.md#usersupdateinstance) | **PATCH** /v1/users/{id} |  |
| [**UsersVisibleAppsCreateToManyRelationship**](UsersApi.md#usersvisibleappscreatetomanyrelationship) | **POST** /v1/users/{id}/relationships/visibleApps |  |
| [**UsersVisibleAppsDeleteToManyRelationship**](UsersApi.md#usersvisibleappsdeletetomanyrelationship) | **DELETE** /v1/users/{id}/relationships/visibleApps |  |
| [**UsersVisibleAppsGetToManyRelated**](UsersApi.md#usersvisibleappsgettomanyrelated) | **GET** /v1/users/{id}/visibleApps |  |
| [**UsersVisibleAppsGetToManyRelationship**](UsersApi.md#usersvisibleappsgettomanyrelationship) | **GET** /v1/users/{id}/relationships/visibleApps |  |
| [**UsersVisibleAppsReplaceToManyRelationship**](UsersApi.md#usersvisibleappsreplacetomanyrelationship) | **PATCH** /v1/users/{id}/relationships/visibleApps |  |

<a id="usersdeleteinstance"></a>
# **UsersDeleteInstance**
> void UsersDeleteInstance (string id)



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
    public class UsersDeleteInstanceExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.UsersDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.UsersDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="usersgetcollection"></a>
# **UsersGetCollection**
> UsersResponse UsersGetCollection (List<string>? filterUsername = null, List<string>? filterRoles = null, List<string>? filterVisibleApps = null, List<string>? sort = null, List<string>? fieldsUsers = null, List<string>? fieldsApps = null, int? limit = null, List<string>? include = null, int? limitVisibleApps = null)



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
    public class UsersGetCollectionExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var filterUsername = new List<string>?(); // List<string>? | filter by attribute 'username' (optional) 
            var filterRoles = new List<string>?(); // List<string>? | filter by attribute 'roles' (optional) 
            var filterVisibleApps = new List<string>?(); // List<string>? | filter by id(s) of related 'visibleApps' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsUsers = new List<string>?(); // List<string>? | the fields to include for returned resources of type users (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVisibleApps = 56;  // int? | maximum number of related visibleApps returned (when they are included) (optional) 

            try
            {
                UsersResponse result = apiInstance.UsersGetCollection(filterUsername, filterRoles, filterVisibleApps, sort, fieldsUsers, fieldsApps, limit, include, limitVisibleApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<UsersResponse> response = apiInstance.UsersGetCollectionWithHttpInfo(filterUsername, filterRoles, filterVisibleApps, sort, fieldsUsers, fieldsApps, limit, include, limitVisibleApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterUsername** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;username&#39; | [optional]  |
| **filterRoles** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;roles&#39; | [optional]  |
| **filterVisibleApps** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;visibleApps&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsUsers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type users | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVisibleApps** | **int?** | maximum number of related visibleApps returned (when they are included) | [optional]  |

### Return type

[**UsersResponse**](UsersResponse.md)

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
| **200** | List of Users |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="usersgetinstance"></a>
# **UsersGetInstance**
> UserResponse UsersGetInstance (string id, List<string>? fieldsUsers = null, List<string>? fieldsApps = null, List<string>? include = null, int? limitVisibleApps = null)



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
    public class UsersGetInstanceExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsUsers = new List<string>?(); // List<string>? | the fields to include for returned resources of type users (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitVisibleApps = 56;  // int? | maximum number of related visibleApps returned (when they are included) (optional) 

            try
            {
                UserResponse result = apiInstance.UsersGetInstance(id, fieldsUsers, fieldsApps, include, limitVisibleApps);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<UserResponse> response = apiInstance.UsersGetInstanceWithHttpInfo(id, fieldsUsers, fieldsApps, include, limitVisibleApps);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsUsers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type users | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVisibleApps** | **int?** | maximum number of related visibleApps returned (when they are included) | [optional]  |

### Return type

[**UserResponse**](UserResponse.md)

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
| **200** | Single User |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="usersupdateinstance"></a>
# **UsersUpdateInstance**
> UserResponse UsersUpdateInstance (string id, UserUpdateRequest userUpdateRequest)



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
    public class UsersUpdateInstanceExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var userUpdateRequest = new UserUpdateRequest(); // UserUpdateRequest | User representation

            try
            {
                UserResponse result = apiInstance.UsersUpdateInstance(id, userUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<UserResponse> response = apiInstance.UsersUpdateInstanceWithHttpInfo(id, userUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **userUpdateRequest** | [**UserUpdateRequest**](UserUpdateRequest.md) | User representation |  |

### Return type

[**UserResponse**](UserResponse.md)

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
| **200** | Single User |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="usersvisibleappscreatetomanyrelationship"></a>
# **UsersVisibleAppsCreateToManyRelationship**
> void UsersVisibleAppsCreateToManyRelationship (string id, UserVisibleAppsLinkagesRequest userVisibleAppsLinkagesRequest)



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
    public class UsersVisibleAppsCreateToManyRelationshipExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var userVisibleAppsLinkagesRequest = new UserVisibleAppsLinkagesRequest(); // UserVisibleAppsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.UsersVisibleAppsCreateToManyRelationship(id, userVisibleAppsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersVisibleAppsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersVisibleAppsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.UsersVisibleAppsCreateToManyRelationshipWithHttpInfo(id, userVisibleAppsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersVisibleAppsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **userVisibleAppsLinkagesRequest** | [**UserVisibleAppsLinkagesRequest**](UserVisibleAppsLinkagesRequest.md) | List of related linkages |  |

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

<a id="usersvisibleappsdeletetomanyrelationship"></a>
# **UsersVisibleAppsDeleteToManyRelationship**
> void UsersVisibleAppsDeleteToManyRelationship (string id, UserVisibleAppsLinkagesRequest userVisibleAppsLinkagesRequest)



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
    public class UsersVisibleAppsDeleteToManyRelationshipExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var userVisibleAppsLinkagesRequest = new UserVisibleAppsLinkagesRequest(); // UserVisibleAppsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.UsersVisibleAppsDeleteToManyRelationship(id, userVisibleAppsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersVisibleAppsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersVisibleAppsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.UsersVisibleAppsDeleteToManyRelationshipWithHttpInfo(id, userVisibleAppsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersVisibleAppsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **userVisibleAppsLinkagesRequest** | [**UserVisibleAppsLinkagesRequest**](UserVisibleAppsLinkagesRequest.md) | List of related linkages |  |

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

<a id="usersvisibleappsgettomanyrelated"></a>
# **UsersVisibleAppsGetToManyRelated**
> AppsWithoutIncludesResponse UsersVisibleAppsGetToManyRelated (string id, List<string>? fieldsApps = null, int? limit = null)



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
    public class UsersVisibleAppsGetToManyRelatedExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppsWithoutIncludesResponse result = apiInstance.UsersVisibleAppsGetToManyRelated(id, fieldsApps, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersVisibleAppsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersVisibleAppsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppsWithoutIncludesResponse> response = apiInstance.UsersVisibleAppsGetToManyRelatedWithHttpInfo(id, fieldsApps, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersVisibleAppsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AppsWithoutIncludesResponse**](AppsWithoutIncludesResponse.md)

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
| **200** | List of Apps with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="usersvisibleappsgettomanyrelationship"></a>
# **UsersVisibleAppsGetToManyRelationship**
> UserVisibleAppsLinkagesResponse UsersVisibleAppsGetToManyRelationship (string id, int? limit = null)



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
    public class UsersVisibleAppsGetToManyRelationshipExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                UserVisibleAppsLinkagesResponse result = apiInstance.UsersVisibleAppsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersVisibleAppsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersVisibleAppsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<UserVisibleAppsLinkagesResponse> response = apiInstance.UsersVisibleAppsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersVisibleAppsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**UserVisibleAppsLinkagesResponse**](UserVisibleAppsLinkagesResponse.md)

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

<a id="usersvisibleappsreplacetomanyrelationship"></a>
# **UsersVisibleAppsReplaceToManyRelationship**
> void UsersVisibleAppsReplaceToManyRelationship (string id, UserVisibleAppsLinkagesRequest userVisibleAppsLinkagesRequest)



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
    public class UsersVisibleAppsReplaceToManyRelationshipExample
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
            var apiInstance = new UsersApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var userVisibleAppsLinkagesRequest = new UserVisibleAppsLinkagesRequest(); // UserVisibleAppsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.UsersVisibleAppsReplaceToManyRelationship(id, userVisibleAppsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UsersApi.UsersVisibleAppsReplaceToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the UsersVisibleAppsReplaceToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.UsersVisibleAppsReplaceToManyRelationshipWithHttpInfo(id, userVisibleAppsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UsersApi.UsersVisibleAppsReplaceToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **userVisibleAppsLinkagesRequest** | [**UserVisibleAppsLinkagesRequest**](UserVisibleAppsLinkagesRequest.md) | List of related linkages |  |

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

