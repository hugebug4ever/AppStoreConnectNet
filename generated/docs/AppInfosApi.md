# AppStoreConnect.Net.Api.AppInfosApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppInfosAgeRatingDeclarationGetToOneRelated**](AppInfosApi.md#appinfosageratingdeclarationgettoonerelated) | **GET** /v1/appInfos/{id}/ageRatingDeclaration |  |
| [**AppInfosAgeRatingDeclarationGetToOneRelationship**](AppInfosApi.md#appinfosageratingdeclarationgettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/ageRatingDeclaration |  |
| [**AppInfosAppInfoLocalizationsGetToManyRelated**](AppInfosApi.md#appinfosappinfolocalizationsgettomanyrelated) | **GET** /v1/appInfos/{id}/appInfoLocalizations |  |
| [**AppInfosAppInfoLocalizationsGetToManyRelationship**](AppInfosApi.md#appinfosappinfolocalizationsgettomanyrelationship) | **GET** /v1/appInfos/{id}/relationships/appInfoLocalizations |  |
| [**AppInfosGetInstance**](AppInfosApi.md#appinfosgetinstance) | **GET** /v1/appInfos/{id} |  |
| [**AppInfosPrimaryCategoryGetToOneRelated**](AppInfosApi.md#appinfosprimarycategorygettoonerelated) | **GET** /v1/appInfos/{id}/primaryCategory |  |
| [**AppInfosPrimaryCategoryGetToOneRelationship**](AppInfosApi.md#appinfosprimarycategorygettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primaryCategory |  |
| [**AppInfosPrimarySubcategoryOneGetToOneRelated**](AppInfosApi.md#appinfosprimarysubcategoryonegettoonerelated) | **GET** /v1/appInfos/{id}/primarySubcategoryOne |  |
| [**AppInfosPrimarySubcategoryOneGetToOneRelationship**](AppInfosApi.md#appinfosprimarysubcategoryonegettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryOne |  |
| [**AppInfosPrimarySubcategoryTwoGetToOneRelated**](AppInfosApi.md#appinfosprimarysubcategorytwogettoonerelated) | **GET** /v1/appInfos/{id}/primarySubcategoryTwo |  |
| [**AppInfosPrimarySubcategoryTwoGetToOneRelationship**](AppInfosApi.md#appinfosprimarysubcategorytwogettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryTwo |  |
| [**AppInfosSecondaryCategoryGetToOneRelated**](AppInfosApi.md#appinfossecondarycategorygettoonerelated) | **GET** /v1/appInfos/{id}/secondaryCategory |  |
| [**AppInfosSecondaryCategoryGetToOneRelationship**](AppInfosApi.md#appinfossecondarycategorygettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondaryCategory |  |
| [**AppInfosSecondarySubcategoryOneGetToOneRelated**](AppInfosApi.md#appinfossecondarysubcategoryonegettoonerelated) | **GET** /v1/appInfos/{id}/secondarySubcategoryOne |  |
| [**AppInfosSecondarySubcategoryOneGetToOneRelationship**](AppInfosApi.md#appinfossecondarysubcategoryonegettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryOne |  |
| [**AppInfosSecondarySubcategoryTwoGetToOneRelated**](AppInfosApi.md#appinfossecondarysubcategorytwogettoonerelated) | **GET** /v1/appInfos/{id}/secondarySubcategoryTwo |  |
| [**AppInfosSecondarySubcategoryTwoGetToOneRelationship**](AppInfosApi.md#appinfossecondarysubcategorytwogettoonerelationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryTwo |  |
| [**AppInfosTerritoryAgeRatingsGetToManyRelated**](AppInfosApi.md#appinfosterritoryageratingsgettomanyrelated) | **GET** /v1/appInfos/{id}/territoryAgeRatings |  |
| [**AppInfosTerritoryAgeRatingsGetToManyRelationship**](AppInfosApi.md#appinfosterritoryageratingsgettomanyrelationship) | **GET** /v1/appInfos/{id}/relationships/territoryAgeRatings |  |
| [**AppInfosUpdateInstance**](AppInfosApi.md#appinfosupdateinstance) | **PATCH** /v1/appInfos/{id} |  |

<a id="appinfosageratingdeclarationgettoonerelated"></a>
# **AppInfosAgeRatingDeclarationGetToOneRelated**
> AgeRatingDeclarationResponse AppInfosAgeRatingDeclarationGetToOneRelated (string id, List<string>? fieldsAgeRatingDeclarations = null)



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
    public class AppInfosAgeRatingDeclarationGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAgeRatingDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type ageRatingDeclarations (optional) 

            try
            {
                AgeRatingDeclarationResponse result = apiInstance.AppInfosAgeRatingDeclarationGetToOneRelated(id, fieldsAgeRatingDeclarations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosAgeRatingDeclarationGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosAgeRatingDeclarationGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AgeRatingDeclarationResponse> response = apiInstance.AppInfosAgeRatingDeclarationGetToOneRelatedWithHttpInfo(id, fieldsAgeRatingDeclarations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosAgeRatingDeclarationGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |

### Return type

[**AgeRatingDeclarationResponse**](AgeRatingDeclarationResponse.md)

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
| **200** | Single AgeRatingDeclaration |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosageratingdeclarationgettoonerelationship"></a>
# **AppInfosAgeRatingDeclarationGetToOneRelationship**
> AppInfoAgeRatingDeclarationLinkageResponse AppInfosAgeRatingDeclarationGetToOneRelationship (string id)



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
    public class AppInfosAgeRatingDeclarationGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoAgeRatingDeclarationLinkageResponse result = apiInstance.AppInfosAgeRatingDeclarationGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosAgeRatingDeclarationGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosAgeRatingDeclarationGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoAgeRatingDeclarationLinkageResponse> response = apiInstance.AppInfosAgeRatingDeclarationGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosAgeRatingDeclarationGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoAgeRatingDeclarationLinkageResponse**](AppInfoAgeRatingDeclarationLinkageResponse.md)

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

<a id="appinfosappinfolocalizationsgettomanyrelated"></a>
# **AppInfosAppInfoLocalizationsGetToManyRelated**
> AppInfoLocalizationsResponse AppInfosAppInfoLocalizationsGetToManyRelated (string id, List<string>? filterLocale = null, List<string>? fieldsAppInfoLocalizations = null, List<string>? fieldsAppInfos = null, int? limit = null, List<string>? include = null)



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
    public class AppInfosAppInfoLocalizationsGetToManyRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterLocale = new List<string>?(); // List<string>? | filter by attribute 'locale' (optional) 
            var fieldsAppInfoLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appInfoLocalizations (optional) 
            var fieldsAppInfos = new List<string>?(); // List<string>? | the fields to include for returned resources of type appInfos (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                AppInfoLocalizationsResponse result = apiInstance.AppInfosAppInfoLocalizationsGetToManyRelated(id, filterLocale, fieldsAppInfoLocalizations, fieldsAppInfos, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosAppInfoLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosAppInfoLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoLocalizationsResponse> response = apiInstance.AppInfosAppInfoLocalizationsGetToManyRelatedWithHttpInfo(id, filterLocale, fieldsAppInfoLocalizations, fieldsAppInfos, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosAppInfoLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterLocale** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;locale&#39; | [optional]  |
| **fieldsAppInfoLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appInfoLocalizations | [optional]  |
| **fieldsAppInfos** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**AppInfoLocalizationsResponse**](AppInfoLocalizationsResponse.md)

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
| **200** | List of AppInfoLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosappinfolocalizationsgettomanyrelationship"></a>
# **AppInfosAppInfoLocalizationsGetToManyRelationship**
> AppInfoAppInfoLocalizationsLinkagesResponse AppInfosAppInfoLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class AppInfosAppInfoLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppInfoAppInfoLocalizationsLinkagesResponse result = apiInstance.AppInfosAppInfoLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosAppInfoLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosAppInfoLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoAppInfoLocalizationsLinkagesResponse> response = apiInstance.AppInfosAppInfoLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosAppInfoLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppInfoAppInfoLocalizationsLinkagesResponse**](AppInfoAppInfoLocalizationsLinkagesResponse.md)

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

<a id="appinfosgetinstance"></a>
# **AppInfosGetInstance**
> AppInfoResponse AppInfosGetInstance (string id, List<string>? fieldsAppInfos = null, List<string>? fieldsAgeRatingDeclarations = null, List<string>? fieldsAppInfoLocalizations = null, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitAppInfoLocalizations = null)



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
    public class AppInfosGetInstanceExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppInfos = new List<string>?(); // List<string>? | the fields to include for returned resources of type appInfos (optional) 
            var fieldsAgeRatingDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type ageRatingDeclarations (optional) 
            var fieldsAppInfoLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appInfoLocalizations (optional) 
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppInfoLocalizations = 56;  // int? | maximum number of related appInfoLocalizations returned (when they are included) (optional) 

            try
            {
                AppInfoResponse result = apiInstance.AppInfosGetInstance(id, fieldsAppInfos, fieldsAgeRatingDeclarations, fieldsAppInfoLocalizations, fieldsAppCategories, include, limitAppInfoLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoResponse> response = apiInstance.AppInfosGetInstanceWithHttpInfo(id, fieldsAppInfos, fieldsAgeRatingDeclarations, fieldsAppInfoLocalizations, fieldsAppCategories, include, limitAppInfoLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppInfos** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appInfos | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppInfoLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appInfoLocalizations | [optional]  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppInfoLocalizations** | **int?** | maximum number of related appInfoLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
| **200** | Single AppInfo |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosprimarycategorygettoonerelated"></a>
# **AppInfosPrimaryCategoryGetToOneRelated**
> AppCategoryResponse AppInfosPrimaryCategoryGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosPrimaryCategoryGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosPrimaryCategoryGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimaryCategoryGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimaryCategoryGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosPrimaryCategoryGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimaryCategoryGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosprimarycategorygettoonerelationship"></a>
# **AppInfosPrimaryCategoryGetToOneRelationship**
> AppInfoPrimaryCategoryLinkageResponse AppInfosPrimaryCategoryGetToOneRelationship (string id)



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
    public class AppInfosPrimaryCategoryGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoPrimaryCategoryLinkageResponse result = apiInstance.AppInfosPrimaryCategoryGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimaryCategoryGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimaryCategoryGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoPrimaryCategoryLinkageResponse> response = apiInstance.AppInfosPrimaryCategoryGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimaryCategoryGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimaryCategoryLinkageResponse**](AppInfoPrimaryCategoryLinkageResponse.md)

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

<a id="appinfosprimarysubcategoryonegettoonerelated"></a>
# **AppInfosPrimarySubcategoryOneGetToOneRelated**
> AppCategoryResponse AppInfosPrimarySubcategoryOneGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosPrimarySubcategoryOneGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosPrimarySubcategoryOneGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryOneGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimarySubcategoryOneGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosPrimarySubcategoryOneGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryOneGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosprimarysubcategoryonegettoonerelationship"></a>
# **AppInfosPrimarySubcategoryOneGetToOneRelationship**
> AppInfoPrimarySubcategoryOneLinkageResponse AppInfosPrimarySubcategoryOneGetToOneRelationship (string id)



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
    public class AppInfosPrimarySubcategoryOneGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoPrimarySubcategoryOneLinkageResponse result = apiInstance.AppInfosPrimarySubcategoryOneGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryOneGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimarySubcategoryOneGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoPrimarySubcategoryOneLinkageResponse> response = apiInstance.AppInfosPrimarySubcategoryOneGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryOneGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimarySubcategoryOneLinkageResponse**](AppInfoPrimarySubcategoryOneLinkageResponse.md)

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

<a id="appinfosprimarysubcategorytwogettoonerelated"></a>
# **AppInfosPrimarySubcategoryTwoGetToOneRelated**
> AppCategoryResponse AppInfosPrimarySubcategoryTwoGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosPrimarySubcategoryTwoGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosPrimarySubcategoryTwoGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryTwoGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimarySubcategoryTwoGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosPrimarySubcategoryTwoGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryTwoGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosprimarysubcategorytwogettoonerelationship"></a>
# **AppInfosPrimarySubcategoryTwoGetToOneRelationship**
> AppInfoPrimarySubcategoryTwoLinkageResponse AppInfosPrimarySubcategoryTwoGetToOneRelationship (string id)



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
    public class AppInfosPrimarySubcategoryTwoGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoPrimarySubcategoryTwoLinkageResponse result = apiInstance.AppInfosPrimarySubcategoryTwoGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryTwoGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosPrimarySubcategoryTwoGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoPrimarySubcategoryTwoLinkageResponse> response = apiInstance.AppInfosPrimarySubcategoryTwoGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosPrimarySubcategoryTwoGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoPrimarySubcategoryTwoLinkageResponse**](AppInfoPrimarySubcategoryTwoLinkageResponse.md)

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

<a id="appinfossecondarycategorygettoonerelated"></a>
# **AppInfosSecondaryCategoryGetToOneRelated**
> AppCategoryResponse AppInfosSecondaryCategoryGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosSecondaryCategoryGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosSecondaryCategoryGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondaryCategoryGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondaryCategoryGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosSecondaryCategoryGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondaryCategoryGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfossecondarycategorygettoonerelationship"></a>
# **AppInfosSecondaryCategoryGetToOneRelationship**
> AppInfoSecondaryCategoryLinkageResponse AppInfosSecondaryCategoryGetToOneRelationship (string id)



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
    public class AppInfosSecondaryCategoryGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoSecondaryCategoryLinkageResponse result = apiInstance.AppInfosSecondaryCategoryGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondaryCategoryGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondaryCategoryGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoSecondaryCategoryLinkageResponse> response = apiInstance.AppInfosSecondaryCategoryGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondaryCategoryGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondaryCategoryLinkageResponse**](AppInfoSecondaryCategoryLinkageResponse.md)

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

<a id="appinfossecondarysubcategoryonegettoonerelated"></a>
# **AppInfosSecondarySubcategoryOneGetToOneRelated**
> AppCategoryResponse AppInfosSecondarySubcategoryOneGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosSecondarySubcategoryOneGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosSecondarySubcategoryOneGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryOneGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondarySubcategoryOneGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosSecondarySubcategoryOneGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryOneGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfossecondarysubcategoryonegettoonerelationship"></a>
# **AppInfosSecondarySubcategoryOneGetToOneRelationship**
> AppInfoSecondarySubcategoryOneLinkageResponse AppInfosSecondarySubcategoryOneGetToOneRelationship (string id)



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
    public class AppInfosSecondarySubcategoryOneGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoSecondarySubcategoryOneLinkageResponse result = apiInstance.AppInfosSecondarySubcategoryOneGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryOneGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondarySubcategoryOneGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoSecondarySubcategoryOneLinkageResponse> response = apiInstance.AppInfosSecondarySubcategoryOneGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryOneGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondarySubcategoryOneLinkageResponse**](AppInfoSecondarySubcategoryOneLinkageResponse.md)

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

<a id="appinfossecondarysubcategorytwogettoonerelated"></a>
# **AppInfosSecondarySubcategoryTwoGetToOneRelated**
> AppCategoryResponse AppInfosSecondarySubcategoryTwoGetToOneRelated (string id, List<string>? fieldsAppCategories = null, List<string>? include = null, int? limitSubcategories = null)



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
    public class AppInfosSecondarySubcategoryTwoGetToOneRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCategories = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCategories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitSubcategories = 56;  // int? | maximum number of related subcategories returned (when they are included) (optional) 

            try
            {
                AppCategoryResponse result = apiInstance.AppInfosSecondarySubcategoryTwoGetToOneRelated(id, fieldsAppCategories, include, limitSubcategories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryTwoGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondarySubcategoryTwoGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCategoryResponse> response = apiInstance.AppInfosSecondarySubcategoryTwoGetToOneRelatedWithHttpInfo(id, fieldsAppCategories, include, limitSubcategories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryTwoGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCategories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCategories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitSubcategories** | **int?** | maximum number of related subcategories returned (when they are included) | [optional]  |

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
| **200** | Single AppCategory |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfossecondarysubcategorytwogettoonerelationship"></a>
# **AppInfosSecondarySubcategoryTwoGetToOneRelationship**
> AppInfoSecondarySubcategoryTwoLinkageResponse AppInfosSecondarySubcategoryTwoGetToOneRelationship (string id)



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
    public class AppInfosSecondarySubcategoryTwoGetToOneRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                AppInfoSecondarySubcategoryTwoLinkageResponse result = apiInstance.AppInfosSecondarySubcategoryTwoGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryTwoGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosSecondarySubcategoryTwoGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoSecondarySubcategoryTwoLinkageResponse> response = apiInstance.AppInfosSecondarySubcategoryTwoGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosSecondarySubcategoryTwoGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**AppInfoSecondarySubcategoryTwoLinkageResponse**](AppInfoSecondarySubcategoryTwoLinkageResponse.md)

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

<a id="appinfosterritoryageratingsgettomanyrelated"></a>
# **AppInfosTerritoryAgeRatingsGetToManyRelated**
> TerritoryAgeRatingsResponse AppInfosTerritoryAgeRatingsGetToManyRelated (string id, List<string>? fieldsTerritoryAgeRatings = null, List<string>? fieldsTerritories = null, int? limit = null, List<string>? include = null)



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
    public class AppInfosTerritoryAgeRatingsGetToManyRelatedExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsTerritoryAgeRatings = new List<string>?(); // List<string>? | the fields to include for returned resources of type territoryAgeRatings (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                TerritoryAgeRatingsResponse result = apiInstance.AppInfosTerritoryAgeRatingsGetToManyRelated(id, fieldsTerritoryAgeRatings, fieldsTerritories, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosTerritoryAgeRatingsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosTerritoryAgeRatingsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TerritoryAgeRatingsResponse> response = apiInstance.AppInfosTerritoryAgeRatingsGetToManyRelatedWithHttpInfo(id, fieldsTerritoryAgeRatings, fieldsTerritories, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosTerritoryAgeRatingsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritoryAgeRatings** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territoryAgeRatings | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**TerritoryAgeRatingsResponse**](TerritoryAgeRatingsResponse.md)

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
| **200** | List of TerritoryAgeRatings |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appinfosterritoryageratingsgettomanyrelationship"></a>
# **AppInfosTerritoryAgeRatingsGetToManyRelationship**
> AppInfoTerritoryAgeRatingsLinkagesResponse AppInfosTerritoryAgeRatingsGetToManyRelationship (string id, int? limit = null)



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
    public class AppInfosTerritoryAgeRatingsGetToManyRelationshipExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppInfoTerritoryAgeRatingsLinkagesResponse result = apiInstance.AppInfosTerritoryAgeRatingsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosTerritoryAgeRatingsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosTerritoryAgeRatingsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoTerritoryAgeRatingsLinkagesResponse> response = apiInstance.AppInfosTerritoryAgeRatingsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosTerritoryAgeRatingsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppInfoTerritoryAgeRatingsLinkagesResponse**](AppInfoTerritoryAgeRatingsLinkagesResponse.md)

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

<a id="appinfosupdateinstance"></a>
# **AppInfosUpdateInstance**
> AppInfoResponse AppInfosUpdateInstance (string id, AppInfoUpdateRequest appInfoUpdateRequest)



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
    public class AppInfosUpdateInstanceExample
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
            var apiInstance = new AppInfosApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appInfoUpdateRequest = new AppInfoUpdateRequest(); // AppInfoUpdateRequest | AppInfo representation

            try
            {
                AppInfoResponse result = apiInstance.AppInfosUpdateInstance(id, appInfoUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppInfosApi.AppInfosUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppInfosUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppInfoResponse> response = apiInstance.AppInfosUpdateInstanceWithHttpInfo(id, appInfoUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppInfosApi.AppInfosUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appInfoUpdateRequest** | [**AppInfoUpdateRequest**](AppInfoUpdateRequest.md) | AppInfo representation |  |

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
| **200** | Single AppInfo |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

