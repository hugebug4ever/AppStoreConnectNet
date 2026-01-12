# AppStoreConnect.Net.Api.AppStoreVersionExperimentTreatmentLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsCreateInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationscreateinstance) | **POST** /v1/appStoreVersionExperimentTreatmentLocalizations |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsdeleteinstance) | **DELETE** /v1/appStoreVersionExperimentTreatmentLocalizations/{id} |  |
| [**AppStoreVersionExperimentTreatmentLocalizationsGetInstance**](AppStoreVersionExperimentTreatmentLocalizationsApi.md#appstoreversionexperimenttreatmentlocalizationsgetinstance) | **GET** /v1/appStoreVersionExperimentTreatmentLocalizations/{id} |  |

<a id="appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string>? filterPreviewType = null, List<string>? filterAppStoreVersionLocalization = null, List<string>? filterAppCustomProductPageLocalization = null, List<string>? fieldsAppPreviewSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppPreviews = null, int? limit = null, List<string>? include = null, int? limitAppPreviews = null)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPreviewType = new List<string>?(); // List<string>? | filter by attribute 'previewType' (optional) 
            var filterAppStoreVersionLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionLocalization' (optional) 
            var filterAppCustomProductPageLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appCustomProductPageLocalization' (optional) 
            var fieldsAppPreviewSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviewSets (optional) 
            var fieldsAppStoreVersionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionLocalizations (optional) 
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var fieldsAppStoreVersionExperimentTreatmentLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional) 
            var fieldsAppPreviews = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviews (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppPreviews = 56;  // int? | maximum number of related appPreviews returned (when they are included) (optional) 

            try
            {
                AppPreviewSetsResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated(id, filterPreviewType, filterAppStoreVersionLocalization, filterAppCustomProductPageLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPreviewSetsResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo(id, filterPreviewType, filterAppStoreVersionLocalization, filterAppCustomProductPageLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPreviewType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;previewType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppPreviews** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviews | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviews** | **int?** | maximum number of related appPreviews returned (when they are included) | [optional]  |

### Return type

[**AppPreviewSetsResponse**](AppPreviewSetsResponse.md)

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
| **200** | List of AppPreviewSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship**
> AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse**](AppStoreVersionExperimentTreatmentLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string>? filterScreenshotDisplayType = null, List<string>? filterAppStoreVersionLocalization = null, List<string>? filterAppCustomProductPageLocalization = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppScreenshots = null, int? limit = null, List<string>? include = null, int? limitAppScreenshots = null)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterScreenshotDisplayType = new List<string>?(); // List<string>? | filter by attribute 'screenshotDisplayType' (optional) 
            var filterAppStoreVersionLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionLocalization' (optional) 
            var filterAppCustomProductPageLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appCustomProductPageLocalization' (optional) 
            var fieldsAppScreenshotSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshotSets (optional) 
            var fieldsAppStoreVersionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionLocalizations (optional) 
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var fieldsAppStoreVersionExperimentTreatmentLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional) 
            var fieldsAppScreenshots = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshots (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppScreenshots = 56;  // int? | maximum number of related appScreenshots returned (when they are included) (optional) 

            try
            {
                AppScreenshotSetsResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated(id, filterScreenshotDisplayType, filterAppStoreVersionLocalization, filterAppCustomProductPageLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppScreenshotSetsResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo(id, filterScreenshotDisplayType, filterAppStoreVersionLocalization, filterAppCustomProductPageLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterScreenshotDisplayType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;screenshotDisplayType&#39; | [optional]  |
| **filterAppStoreVersionLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appStoreVersionLocalization&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppScreenshots** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshots | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppScreenshots** | **int?** | maximum number of related appScreenshots returned (when they are included) | [optional]  |

### Return type

[**AppScreenshotSetsResponse**](AppScreenshotSetsResponse.md)

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
| **200** | List of AppScreenshotSets |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse**](AppStoreVersionExperimentTreatmentLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appstoreversionexperimenttreatmentlocalizationscreateinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsCreateInstance**
> AppStoreVersionExperimentTreatmentLocalizationResponse AppStoreVersionExperimentTreatmentLocalizationsCreateInstance (AppStoreVersionExperimentTreatmentLocalizationCreateRequest appStoreVersionExperimentTreatmentLocalizationCreateRequest)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsCreateInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var appStoreVersionExperimentTreatmentLocalizationCreateRequest = new AppStoreVersionExperimentTreatmentLocalizationCreateRequest(); // AppStoreVersionExperimentTreatmentLocalizationCreateRequest | AppStoreVersionExperimentTreatmentLocalization representation

            try
            {
                AppStoreVersionExperimentTreatmentLocalizationResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsCreateInstance(appStoreVersionExperimentTreatmentLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentLocalizationResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsCreateInstanceWithHttpInfo(appStoreVersionExperimentTreatmentLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentTreatmentLocalizationCreateRequest** | [**AppStoreVersionExperimentTreatmentLocalizationCreateRequest**](AppStoreVersionExperimentTreatmentLocalizationCreateRequest.md) | AppStoreVersionExperimentTreatmentLocalization representation |  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationResponse**](AppStoreVersionExperimentTreatmentLocalizationResponse.md)

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
| **201** | Single AppStoreVersionExperimentTreatmentLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimenttreatmentlocalizationsdeleteinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance**
> void AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance (string id)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsDeleteInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionExperimentTreatmentLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appstoreversionexperimenttreatmentlocalizationsgetinstance"></a>
# **AppStoreVersionExperimentTreatmentLocalizationsGetInstance**
> AppStoreVersionExperimentTreatmentLocalizationResponse AppStoreVersionExperimentTreatmentLocalizationsGetInstance (string id, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppPreviewSets = null, List<string>? include = null, int? limitAppPreviewSets = null, int? limitAppScreenshotSets = null)



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
    public class AppStoreVersionExperimentTreatmentLocalizationsGetInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentTreatmentLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionExperimentTreatmentLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional) 
            var fieldsAppScreenshotSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshotSets (optional) 
            var fieldsAppPreviewSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviewSets (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppPreviewSets = 56;  // int? | maximum number of related appPreviewSets returned (when they are included) (optional) 
            var limitAppScreenshotSets = 56;  // int? | maximum number of related appScreenshotSets returned (when they are included) (optional) 

            try
            {
                AppStoreVersionExperimentTreatmentLocalizationResponse result = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsGetInstance(id, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentTreatmentLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentLocalizationResponse> response = apiInstance.AppStoreVersionExperimentTreatmentLocalizationsGetInstanceWithHttpInfo(id, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentTreatmentLocalizationsApi.AppStoreVersionExperimentTreatmentLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int?** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int?** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationResponse**](AppStoreVersionExperimentTreatmentLocalizationResponse.md)

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
| **200** | Single AppStoreVersionExperimentTreatmentLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

