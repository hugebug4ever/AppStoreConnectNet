# AppStoreConnect.Net.Api.AppClipsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppClipsAppClipAdvancedExperiencesGetToManyRelated**](AppClipsApi.md#appclipsappclipadvancedexperiencesgettomanyrelated) | **GET** /v1/appClips/{id}/appClipAdvancedExperiences |  |
| [**AppClipsAppClipAdvancedExperiencesGetToManyRelationship**](AppClipsApi.md#appclipsappclipadvancedexperiencesgettomanyrelationship) | **GET** /v1/appClips/{id}/relationships/appClipAdvancedExperiences |  |
| [**AppClipsAppClipDefaultExperiencesGetToManyRelated**](AppClipsApi.md#appclipsappclipdefaultexperiencesgettomanyrelated) | **GET** /v1/appClips/{id}/appClipDefaultExperiences |  |
| [**AppClipsAppClipDefaultExperiencesGetToManyRelationship**](AppClipsApi.md#appclipsappclipdefaultexperiencesgettomanyrelationship) | **GET** /v1/appClips/{id}/relationships/appClipDefaultExperiences |  |
| [**AppClipsGetInstance**](AppClipsApi.md#appclipsgetinstance) | **GET** /v1/appClips/{id} |  |

<a id="appclipsappclipadvancedexperiencesgettomanyrelated"></a>
# **AppClipsAppClipAdvancedExperiencesGetToManyRelated**
> AppClipAdvancedExperiencesResponse AppClipsAppClipAdvancedExperiencesGetToManyRelated (string id, List<string>? filterStatus = null, List<string>? filterPlaceStatus = null, List<string>? filterAction = null, List<string>? fieldsAppClipAdvancedExperiences = null, List<string>? fieldsAppClips = null, List<string>? fieldsAppClipAdvancedExperienceImages = null, List<string>? fieldsAppClipAdvancedExperienceLocalizations = null, int? limit = null, List<string>? include = null, int? limitLocalizations = null)



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
    public class AppClipsAppClipAdvancedExperiencesGetToManyRelatedExample
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
            var apiInstance = new AppClipsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterStatus = new List<string>?(); // List<string>? | filter by attribute 'status' (optional) 
            var filterPlaceStatus = new List<string>?(); // List<string>? | filter by attribute 'placeStatus' (optional) 
            var filterAction = new List<string>?(); // List<string>? | filter by attribute 'action' (optional) 
            var fieldsAppClipAdvancedExperiences = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipAdvancedExperiences (optional) 
            var fieldsAppClips = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClips (optional) 
            var fieldsAppClipAdvancedExperienceImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipAdvancedExperienceImages (optional) 
            var fieldsAppClipAdvancedExperienceLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipAdvancedExperienceLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitLocalizations = 56;  // int? | maximum number of related localizations returned (when they are included) (optional) 

            try
            {
                AppClipAdvancedExperiencesResponse result = apiInstance.AppClipsAppClipAdvancedExperiencesGetToManyRelated(id, filterStatus, filterPlaceStatus, filterAction, fieldsAppClipAdvancedExperiences, fieldsAppClips, fieldsAppClipAdvancedExperienceImages, fieldsAppClipAdvancedExperienceLocalizations, limit, include, limitLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipAdvancedExperiencesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppClipsAppClipAdvancedExperiencesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipAdvancedExperiencesResponse> response = apiInstance.AppClipsAppClipAdvancedExperiencesGetToManyRelatedWithHttpInfo(id, filterStatus, filterPlaceStatus, filterAction, fieldsAppClipAdvancedExperiences, fieldsAppClips, fieldsAppClipAdvancedExperienceImages, fieldsAppClipAdvancedExperienceLocalizations, limit, include, limitLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipAdvancedExperiencesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterStatus** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;status&#39; | [optional]  |
| **filterPlaceStatus** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;placeStatus&#39; | [optional]  |
| **filterAction** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;action&#39; | [optional]  |
| **fieldsAppClipAdvancedExperiences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipAdvancedExperiences | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppClipAdvancedExperienceImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipAdvancedExperienceImages | [optional]  |
| **fieldsAppClipAdvancedExperienceLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipAdvancedExperienceLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitLocalizations** | **int?** | maximum number of related localizations returned (when they are included) | [optional]  |

### Return type

[**AppClipAdvancedExperiencesResponse**](AppClipAdvancedExperiencesResponse.md)

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
| **200** | List of AppClipAdvancedExperiences |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appclipsappclipadvancedexperiencesgettomanyrelationship"></a>
# **AppClipsAppClipAdvancedExperiencesGetToManyRelationship**
> AppClipAppClipAdvancedExperiencesLinkagesResponse AppClipsAppClipAdvancedExperiencesGetToManyRelationship (string id, int? limit = null)



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
    public class AppClipsAppClipAdvancedExperiencesGetToManyRelationshipExample
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
            var apiInstance = new AppClipsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppClipAppClipAdvancedExperiencesLinkagesResponse result = apiInstance.AppClipsAppClipAdvancedExperiencesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipAdvancedExperiencesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppClipsAppClipAdvancedExperiencesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipAppClipAdvancedExperiencesLinkagesResponse> response = apiInstance.AppClipsAppClipAdvancedExperiencesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipAdvancedExperiencesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppClipAppClipAdvancedExperiencesLinkagesResponse**](AppClipAppClipAdvancedExperiencesLinkagesResponse.md)

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

<a id="appclipsappclipdefaultexperiencesgettomanyrelated"></a>
# **AppClipsAppClipDefaultExperiencesGetToManyRelated**
> AppClipDefaultExperiencesResponse AppClipsAppClipDefaultExperiencesGetToManyRelated (string id, bool? existsReleaseWithAppStoreVersion = null, List<string>? fieldsAppClipDefaultExperiences = null, List<string>? fieldsAppClips = null, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsAppClipDefaultExperienceLocalizations = null, List<string>? fieldsAppClipAppStoreReviewDetails = null, int? limit = null, List<string>? include = null, int? limitAppClipDefaultExperienceLocalizations = null)



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
    public class AppClipsAppClipDefaultExperiencesGetToManyRelatedExample
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
            var apiInstance = new AppClipsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var existsReleaseWithAppStoreVersion = true;  // bool? | filter by existence or non-existence of related 'releaseWithAppStoreVersion' (optional) 
            var fieldsAppClipDefaultExperiences = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDefaultExperiences (optional) 
            var fieldsAppClips = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClips (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsAppClipDefaultExperienceLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional) 
            var fieldsAppClipAppStoreReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipAppStoreReviewDetails (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppClipDefaultExperienceLocalizations = 56;  // int? | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) (optional) 

            try
            {
                AppClipDefaultExperiencesResponse result = apiInstance.AppClipsAppClipDefaultExperiencesGetToManyRelated(id, existsReleaseWithAppStoreVersion, fieldsAppClipDefaultExperiences, fieldsAppClips, fieldsAppStoreVersions, fieldsAppClipDefaultExperienceLocalizations, fieldsAppClipAppStoreReviewDetails, limit, include, limitAppClipDefaultExperienceLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipDefaultExperiencesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppClipsAppClipDefaultExperiencesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipDefaultExperiencesResponse> response = apiInstance.AppClipsAppClipDefaultExperiencesGetToManyRelatedWithHttpInfo(id, existsReleaseWithAppStoreVersion, fieldsAppClipDefaultExperiences, fieldsAppClips, fieldsAppStoreVersions, fieldsAppClipDefaultExperienceLocalizations, fieldsAppClipAppStoreReviewDetails, limit, include, limitAppClipDefaultExperienceLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipDefaultExperiencesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **existsReleaseWithAppStoreVersion** | **bool?** | filter by existence or non-existence of related &#39;releaseWithAppStoreVersion&#39; | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppClips** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsAppClipDefaultExperienceLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional]  |
| **fieldsAppClipAppStoreReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppClipDefaultExperienceLocalizations** | **int?** | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppClipDefaultExperiencesResponse**](AppClipDefaultExperiencesResponse.md)

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
| **200** | List of AppClipDefaultExperiences |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appclipsappclipdefaultexperiencesgettomanyrelationship"></a>
# **AppClipsAppClipDefaultExperiencesGetToManyRelationship**
> AppClipAppClipDefaultExperiencesLinkagesResponse AppClipsAppClipDefaultExperiencesGetToManyRelationship (string id, int? limit = null)



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
    public class AppClipsAppClipDefaultExperiencesGetToManyRelationshipExample
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
            var apiInstance = new AppClipsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppClipAppClipDefaultExperiencesLinkagesResponse result = apiInstance.AppClipsAppClipDefaultExperiencesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipDefaultExperiencesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppClipsAppClipDefaultExperiencesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipAppClipDefaultExperiencesLinkagesResponse> response = apiInstance.AppClipsAppClipDefaultExperiencesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppClipsApi.AppClipsAppClipDefaultExperiencesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppClipAppClipDefaultExperiencesLinkagesResponse**](AppClipAppClipDefaultExperiencesLinkagesResponse.md)

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

<a id="appclipsgetinstance"></a>
# **AppClipsGetInstance**
> AppClipResponse AppClipsGetInstance (string id, List<string>? fieldsAppClips = null, List<string>? fieldsAppClipDefaultExperiences = null, List<string>? include = null, int? limitAppClipDefaultExperiences = null)



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
    public class AppClipsGetInstanceExample
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
            var apiInstance = new AppClipsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppClips = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClips (optional) 
            var fieldsAppClipDefaultExperiences = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDefaultExperiences (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppClipDefaultExperiences = 56;  // int? | maximum number of related appClipDefaultExperiences returned (when they are included) (optional) 

            try
            {
                AppClipResponse result = apiInstance.AppClipsGetInstance(id, fieldsAppClips, fieldsAppClipDefaultExperiences, include, limitAppClipDefaultExperiences);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppClipsApi.AppClipsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppClipsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppClipResponse> response = apiInstance.AppClipsGetInstanceWithHttpInfo(id, fieldsAppClips, fieldsAppClipDefaultExperiences, include, limitAppClipDefaultExperiences);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppClipsApi.AppClipsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppClips** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClips | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppClipDefaultExperiences** | **int?** | maximum number of related appClipDefaultExperiences returned (when they are included) | [optional]  |

### Return type

[**AppClipResponse**](AppClipResponse.md)

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
| **200** | Single AppClip |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

