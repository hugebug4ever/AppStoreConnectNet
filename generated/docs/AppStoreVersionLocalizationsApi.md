# AppStoreConnect.Net.Api.AppStoreVersionLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/appPreviewSets |  |
| [**AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/appScreenshotSets |  |
| [**AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppStoreVersionLocalizationsCreateInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationscreateinstance) | **POST** /v1/appStoreVersionLocalizations |  |
| [**AppStoreVersionLocalizationsDeleteInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsdeleteinstance) | **DELETE** /v1/appStoreVersionLocalizations/{id} |  |
| [**AppStoreVersionLocalizationsGetInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsgetinstance) | **GET** /v1/appStoreVersionLocalizations/{id} |  |
| [**AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordscreatetomanyrelationship) | **POST** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsdeletetomanyrelationship) | **DELETE** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsgettomanyrelated) | **GET** /v1/appStoreVersionLocalizations/{id}/searchKeywords |  |
| [**AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationssearchkeywordsgettomanyrelationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords |  |
| [**AppStoreVersionLocalizationsUpdateInstance**](AppStoreVersionLocalizationsApi.md#appstoreversionlocalizationsupdateinstance) | **PATCH** /v1/appStoreVersionLocalizations/{id} |  |

<a id="appstoreversionlocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string>? filterPreviewType = null, List<string>? filterAppCustomProductPageLocalization = null, List<string>? filterAppStoreVersionExperimentTreatmentLocalization = null, List<string>? fieldsAppPreviewSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppPreviews = null, int? limit = null, List<string>? include = null, int? limitAppPreviews = null)



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
    public class AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPreviewType = new List<string>?(); // List<string>? | filter by attribute 'previewType' (optional) 
            var filterAppCustomProductPageLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appCustomProductPageLocalization' (optional) 
            var filterAppStoreVersionExperimentTreatmentLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionExperimentTreatmentLocalization' (optional) 
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
                AppPreviewSetsResponse result = apiInstance.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated(id, filterPreviewType, filterAppCustomProductPageLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPreviewSetsResponse> response = apiInstance.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo(id, filterPreviewType, filterAppCustomProductPageLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPreviewType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;previewType&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **filterAppStoreVersionExperimentTreatmentLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional]  |
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

<a id="appstoreversionlocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship**
> AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse result = apiInstance.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse> response = apiInstance.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse**](AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string>? filterScreenshotDisplayType = null, List<string>? filterAppCustomProductPageLocalization = null, List<string>? filterAppStoreVersionExperimentTreatmentLocalization = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppScreenshots = null, int? limit = null, List<string>? include = null, int? limitAppScreenshots = null)



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
    public class AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterScreenshotDisplayType = new List<string>?(); // List<string>? | filter by attribute 'screenshotDisplayType' (optional) 
            var filterAppCustomProductPageLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appCustomProductPageLocalization' (optional) 
            var filterAppStoreVersionExperimentTreatmentLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionExperimentTreatmentLocalization' (optional) 
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
                AppScreenshotSetsResponse result = apiInstance.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated(id, filterScreenshotDisplayType, filterAppCustomProductPageLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppScreenshotSetsResponse> response = apiInstance.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo(id, filterScreenshotDisplayType, filterAppCustomProductPageLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterScreenshotDisplayType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;screenshotDisplayType&#39; | [optional]  |
| **filterAppCustomProductPageLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional]  |
| **filterAppStoreVersionExperimentTreatmentLocalization** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional]  |
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

<a id="appstoreversionlocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse result = apiInstance.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse> response = apiInstance.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse**](AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationscreateinstance"></a>
# **AppStoreVersionLocalizationsCreateInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsCreateInstance (AppStoreVersionLocalizationCreateRequest appStoreVersionLocalizationCreateRequest)



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
    public class AppStoreVersionLocalizationsCreateInstanceExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var appStoreVersionLocalizationCreateRequest = new AppStoreVersionLocalizationCreateRequest(); // AppStoreVersionLocalizationCreateRequest | AppStoreVersionLocalization representation

            try
            {
                AppStoreVersionLocalizationResponse result = apiInstance.AppStoreVersionLocalizationsCreateInstance(appStoreVersionLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationResponse> response = apiInstance.AppStoreVersionLocalizationsCreateInstanceWithHttpInfo(appStoreVersionLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionLocalizationCreateRequest** | [**AppStoreVersionLocalizationCreateRequest**](AppStoreVersionLocalizationCreateRequest.md) | AppStoreVersionLocalization representation |  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **201** | Single AppStoreVersionLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionlocalizationsdeleteinstance"></a>
# **AppStoreVersionLocalizationsDeleteInstance**
> void AppStoreVersionLocalizationsDeleteInstance (string id)



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
    public class AppStoreVersionLocalizationsDeleteInstanceExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppStoreVersionLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appstoreversionlocalizationsgetinstance"></a>
# **AppStoreVersionLocalizationsGetInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsGetInstance (string id, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppPreviewSets = null, List<string>? include = null, int? limitAppPreviewSets = null, int? limitAppScreenshotSets = null, int? limitSearchKeywords = null)



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
    public class AppStoreVersionLocalizationsGetInstanceExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionLocalizations (optional) 
            var fieldsAppScreenshotSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshotSets (optional) 
            var fieldsAppPreviewSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviewSets (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppPreviewSets = 56;  // int? | maximum number of related appPreviewSets returned (when they are included) (optional) 
            var limitAppScreenshotSets = 56;  // int? | maximum number of related appScreenshotSets returned (when they are included) (optional) 
            var limitSearchKeywords = 56;  // int? | maximum number of related searchKeywords returned (when they are included) (optional) 

            try
            {
                AppStoreVersionLocalizationResponse result = apiInstance.AppStoreVersionLocalizationsGetInstance(id, fieldsAppStoreVersionLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets, limitSearchKeywords);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationResponse> response = apiInstance.AppStoreVersionLocalizationsGetInstanceWithHttpInfo(id, fieldsAppStoreVersionLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets, limitSearchKeywords);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int?** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int?** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int?** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **200** | Single AppStoreVersionLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionlocalizationssearchkeywordscreatetomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship**
> void AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship (string id, AppStoreVersionLocalizationSearchKeywordsLinkagesRequest appStoreVersionLocalizationSearchKeywordsLinkagesRequest)



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
    public class AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appStoreVersionLocalizationSearchKeywordsLinkagesRequest = new AppStoreVersionLocalizationSearchKeywordsLinkagesRequest(); // AppStoreVersionLocalizationSearchKeywordsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship(id, appStoreVersionLocalizationSearchKeywordsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo(id, appStoreVersionLocalizationSearchKeywordsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationSearchKeywordsLinkagesRequest** | [**AppStoreVersionLocalizationSearchKeywordsLinkagesRequest**](AppStoreVersionLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appstoreversionlocalizationssearchkeywordsdeletetomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship**
> void AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship (string id, AppStoreVersionLocalizationSearchKeywordsLinkagesRequest appStoreVersionLocalizationSearchKeywordsLinkagesRequest)



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
    public class AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appStoreVersionLocalizationSearchKeywordsLinkagesRequest = new AppStoreVersionLocalizationSearchKeywordsLinkagesRequest(); // AppStoreVersionLocalizationSearchKeywordsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship(id, appStoreVersionLocalizationSearchKeywordsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo(id, appStoreVersionLocalizationSearchKeywordsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationSearchKeywordsLinkagesRequest** | [**AppStoreVersionLocalizationSearchKeywordsLinkagesRequest**](AppStoreVersionLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appstoreversionlocalizationssearchkeywordsgettomanyrelated"></a>
# **AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated**
> AppKeywordsResponse AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated (string id, List<string>? filterPlatform = null, List<string>? filterLocale = null, List<string>? fieldsAppKeywords = null, int? limit = null)



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
    public class AppStoreVersionLocalizationsSearchKeywordsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPlatform = new List<string>?(); // List<string>? | filter by platform (optional) 
            var filterLocale = new List<string>?(); // List<string>? | filter by locale (optional) 
            var fieldsAppKeywords = new List<string>?(); // List<string>? | the fields to include for returned resources of type appKeywords (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppKeywordsResponse result = apiInstance.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated(id, filterPlatform, filterLocale, fieldsAppKeywords, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppKeywordsResponse> response = apiInstance.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo(id, filterPlatform, filterLocale, fieldsAppKeywords, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPlatform** | [**List&lt;string&gt;?**](string.md) | filter by platform | [optional]  |
| **filterLocale** | [**List&lt;string&gt;?**](string.md) | filter by locale | [optional]  |
| **fieldsAppKeywords** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appKeywords | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**AppKeywordsResponse**](AppKeywordsResponse.md)

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
| **200** | List of AppKeywords |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionlocalizationssearchkeywordsgettomanyrelationship"></a>
# **AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship**
> AppStoreVersionLocalizationSearchKeywordsLinkagesResponse AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionLocalizationSearchKeywordsLinkagesResponse result = apiInstance.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationSearchKeywordsLinkagesResponse> response = apiInstance.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionLocalizationSearchKeywordsLinkagesResponse**](AppStoreVersionLocalizationSearchKeywordsLinkagesResponse.md)

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

<a id="appstoreversionlocalizationsupdateinstance"></a>
# **AppStoreVersionLocalizationsUpdateInstance**
> AppStoreVersionLocalizationResponse AppStoreVersionLocalizationsUpdateInstance (string id, AppStoreVersionLocalizationUpdateRequest appStoreVersionLocalizationUpdateRequest)



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
    public class AppStoreVersionLocalizationsUpdateInstanceExample
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
            var apiInstance = new AppStoreVersionLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appStoreVersionLocalizationUpdateRequest = new AppStoreVersionLocalizationUpdateRequest(); // AppStoreVersionLocalizationUpdateRequest | AppStoreVersionLocalization representation

            try
            {
                AppStoreVersionLocalizationResponse result = apiInstance.AppStoreVersionLocalizationsUpdateInstance(id, appStoreVersionLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionLocalizationResponse> response = apiInstance.AppStoreVersionLocalizationsUpdateInstanceWithHttpInfo(id, appStoreVersionLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionLocalizationsApi.AppStoreVersionLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionLocalizationUpdateRequest** | [**AppStoreVersionLocalizationUpdateRequest**](AppStoreVersionLocalizationUpdateRequest.md) | AppStoreVersionLocalization representation |  |

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
| **200** | Single AppStoreVersionLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

