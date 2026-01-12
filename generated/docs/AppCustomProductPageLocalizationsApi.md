# AppStoreConnect.Net.Api.AppCustomProductPageLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsapppreviewsetsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/appPreviewSets |  |
| [**AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsapppreviewsetsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/appPreviewSets |  |
| [**AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/appScreenshotSets |  |
| [**AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/appScreenshotSets |  |
| [**AppCustomProductPageLocalizationsCreateInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationscreateinstance) | **POST** /v1/appCustomProductPageLocalizations |  |
| [**AppCustomProductPageLocalizationsDeleteInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsdeleteinstance) | **DELETE** /v1/appCustomProductPageLocalizations/{id} |  |
| [**AppCustomProductPageLocalizationsGetInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsgetinstance) | **GET** /v1/appCustomProductPageLocalizations/{id} |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordscreatetomanyrelationship) | **POST** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsdeletetomanyrelationship) | **DELETE** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsgettomanyrelated) | **GET** /v1/appCustomProductPageLocalizations/{id}/searchKeywords |  |
| [**AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationssearchkeywordsgettomanyrelationship) | **GET** /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords |  |
| [**AppCustomProductPageLocalizationsUpdateInstance**](AppCustomProductPageLocalizationsApi.md#appcustomproductpagelocalizationsupdateinstance) | **PATCH** /v1/appCustomProductPageLocalizations/{id} |  |

<a id="appcustomproductpagelocalizationsapppreviewsetsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated**
> AppPreviewSetsResponse AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated (string id, List<string>? filterPreviewType = null, List<string>? filterAppStoreVersionLocalization = null, List<string>? filterAppStoreVersionExperimentTreatmentLocalization = null, List<string>? fieldsAppPreviewSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppPreviews = null, int? limit = null, List<string>? include = null, int? limitAppPreviews = null)



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
    public class AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelatedExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPreviewType = new List<string>?(); // List<string>? | filter by attribute 'previewType' (optional) 
            var filterAppStoreVersionLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionLocalization' (optional) 
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
                AppPreviewSetsResponse result = apiInstance.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated(id, filterPreviewType, filterAppStoreVersionLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppPreviewSetsResponse> response = apiInstance.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo(id, filterPreviewType, filterAppStoreVersionLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppPreviewSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppPreviews, limit, include, limitAppPreviews);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="appcustomproductpagelocalizationsapppreviewsetsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship**
> AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse result = apiInstance.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse> response = apiInstance.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppPreviewSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse**](AppCustomProductPageLocalizationAppPreviewSetsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated**
> AppScreenshotSetsResponse AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated (string id, List<string>? filterScreenshotDisplayType = null, List<string>? filterAppStoreVersionLocalization = null, List<string>? filterAppStoreVersionExperimentTreatmentLocalization = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, List<string>? fieldsAppScreenshots = null, int? limit = null, List<string>? include = null, int? limitAppScreenshots = null)



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
    public class AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelatedExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterScreenshotDisplayType = new List<string>?(); // List<string>? | filter by attribute 'screenshotDisplayType' (optional) 
            var filterAppStoreVersionLocalization = new List<string>?(); // List<string>? | filter by id(s) of related 'appStoreVersionLocalization' (optional) 
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
                AppScreenshotSetsResponse result = apiInstance.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated(id, filterScreenshotDisplayType, filterAppStoreVersionLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppScreenshotSetsResponse> response = apiInstance.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo(id, filterScreenshotDisplayType, filterAppStoreVersionLocalization, filterAppStoreVersionExperimentTreatmentLocalization, fieldsAppScreenshotSets, fieldsAppStoreVersionLocalizations, fieldsAppCustomProductPageLocalizations, fieldsAppStoreVersionExperimentTreatmentLocalizations, fieldsAppScreenshots, limit, include, limitAppScreenshots);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="appcustomproductpagelocalizationsappscreenshotsetsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship**
> AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship (string id, int? limit = null)



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
    public class AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse result = apiInstance.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse> response = apiInstance.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsAppScreenshotSetsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse**](AppCustomProductPageLocalizationAppScreenshotSetsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationscreateinstance"></a>
# **AppCustomProductPageLocalizationsCreateInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsCreateInstance (AppCustomProductPageLocalizationCreateRequest appCustomProductPageLocalizationCreateRequest)



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
    public class AppCustomProductPageLocalizationsCreateInstanceExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var appCustomProductPageLocalizationCreateRequest = new AppCustomProductPageLocalizationCreateRequest(); // AppCustomProductPageLocalizationCreateRequest | AppCustomProductPageLocalization representation

            try
            {
                AppCustomProductPageLocalizationResponse result = apiInstance.AppCustomProductPageLocalizationsCreateInstance(appCustomProductPageLocalizationCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationResponse> response = apiInstance.AppCustomProductPageLocalizationsCreateInstanceWithHttpInfo(appCustomProductPageLocalizationCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appCustomProductPageLocalizationCreateRequest** | [**AppCustomProductPageLocalizationCreateRequest**](AppCustomProductPageLocalizationCreateRequest.md) | AppCustomProductPageLocalization representation |  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **201** | Single AppCustomProductPageLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpagelocalizationsdeleteinstance"></a>
# **AppCustomProductPageLocalizationsDeleteInstance**
> void AppCustomProductPageLocalizationsDeleteInstance (string id)



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
    public class AppCustomProductPageLocalizationsDeleteInstanceExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppCustomProductPageLocalizationsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppCustomProductPageLocalizationsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appcustomproductpagelocalizationsgetinstance"></a>
# **AppCustomProductPageLocalizationsGetInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsGetInstance (string id, List<string>? fieldsAppCustomProductPageLocalizations = null, List<string>? fieldsAppScreenshotSets = null, List<string>? fieldsAppPreviewSets = null, List<string>? include = null, int? limitAppPreviewSets = null, int? limitAppScreenshotSets = null, int? limitSearchKeywords = null)



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
    public class AppCustomProductPageLocalizationsGetInstanceExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppCustomProductPageLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appCustomProductPageLocalizations (optional) 
            var fieldsAppScreenshotSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appScreenshotSets (optional) 
            var fieldsAppPreviewSets = new List<string>?(); // List<string>? | the fields to include for returned resources of type appPreviewSets (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppPreviewSets = 56;  // int? | maximum number of related appPreviewSets returned (when they are included) (optional) 
            var limitAppScreenshotSets = 56;  // int? | maximum number of related appScreenshotSets returned (when they are included) (optional) 
            var limitSearchKeywords = 56;  // int? | maximum number of related searchKeywords returned (when they are included) (optional) 

            try
            {
                AppCustomProductPageLocalizationResponse result = apiInstance.AppCustomProductPageLocalizationsGetInstance(id, fieldsAppCustomProductPageLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets, limitSearchKeywords);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationResponse> response = apiInstance.AppCustomProductPageLocalizationsGetInstanceWithHttpInfo(id, fieldsAppCustomProductPageLocalizations, fieldsAppScreenshotSets, fieldsAppPreviewSets, include, limitAppPreviewSets, limitAppScreenshotSets, limitSearchKeywords);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppCustomProductPageLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appCustomProductPageLocalizations | [optional]  |
| **fieldsAppScreenshotSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appScreenshotSets | [optional]  |
| **fieldsAppPreviewSets** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appPreviewSets | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppPreviewSets** | **int?** | maximum number of related appPreviewSets returned (when they are included) | [optional]  |
| **limitAppScreenshotSets** | **int?** | maximum number of related appScreenshotSets returned (when they are included) | [optional]  |
| **limitSearchKeywords** | **int?** | maximum number of related searchKeywords returned (when they are included) | [optional]  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **200** | Single AppCustomProductPageLocalization |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appcustomproductpagelocalizationssearchkeywordscreatetomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship**
> void AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship (string id, AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest appCustomProductPageLocalizationSearchKeywordsLinkagesRequest)



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
    public class AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appCustomProductPageLocalizationSearchKeywordsLinkagesRequest = new AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest(); // AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship(id, appCustomProductPageLocalizationSearchKeywordsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo(id, appCustomProductPageLocalizationSearchKeywordsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationSearchKeywordsLinkagesRequest** | [**AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest**](AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appcustomproductpagelocalizationssearchkeywordsdeletetomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship**
> void AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship (string id, AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest appCustomProductPageLocalizationSearchKeywordsLinkagesRequest)



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
    public class AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appCustomProductPageLocalizationSearchKeywordsLinkagesRequest = new AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest(); // AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship(id, appCustomProductPageLocalizationSearchKeywordsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo(id, appCustomProductPageLocalizationSearchKeywordsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationSearchKeywordsLinkagesRequest** | [**AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest**](AppCustomProductPageLocalizationSearchKeywordsLinkagesRequest.md) | List of related linkages |  |

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

<a id="appcustomproductpagelocalizationssearchkeywordsgettomanyrelated"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated**
> AppKeywordsResponse AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated (string id, List<string>? filterPlatform = null, List<string>? filterLocale = null, List<string>? fieldsAppKeywords = null, int? limit = null)



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
    public class AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelatedExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterPlatform = new List<string>?(); // List<string>? | filter by platform (optional) 
            var filterLocale = new List<string>?(); // List<string>? | filter by locale (optional) 
            var fieldsAppKeywords = new List<string>?(); // List<string>? | the fields to include for returned resources of type appKeywords (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppKeywordsResponse result = apiInstance.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated(id, filterPlatform, filterLocale, fieldsAppKeywords, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppKeywordsResponse> response = apiInstance.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo(id, filterPlatform, filterLocale, fieldsAppKeywords, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="appcustomproductpagelocalizationssearchkeywordsgettomanyrelationship"></a>
# **AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship**
> AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship (string id, int? limit = null)



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
    public class AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationshipExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse result = apiInstance.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse> response = apiInstance.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsSearchKeywordsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse**](AppCustomProductPageLocalizationSearchKeywordsLinkagesResponse.md)

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

<a id="appcustomproductpagelocalizationsupdateinstance"></a>
# **AppCustomProductPageLocalizationsUpdateInstance**
> AppCustomProductPageLocalizationResponse AppCustomProductPageLocalizationsUpdateInstance (string id, AppCustomProductPageLocalizationUpdateRequest appCustomProductPageLocalizationUpdateRequest)



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
    public class AppCustomProductPageLocalizationsUpdateInstanceExample
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
            var apiInstance = new AppCustomProductPageLocalizationsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appCustomProductPageLocalizationUpdateRequest = new AppCustomProductPageLocalizationUpdateRequest(); // AppCustomProductPageLocalizationUpdateRequest | AppCustomProductPageLocalization representation

            try
            {
                AppCustomProductPageLocalizationResponse result = apiInstance.AppCustomProductPageLocalizationsUpdateInstance(id, appCustomProductPageLocalizationUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppCustomProductPageLocalizationsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppCustomProductPageLocalizationResponse> response = apiInstance.AppCustomProductPageLocalizationsUpdateInstanceWithHttpInfo(id, appCustomProductPageLocalizationUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppCustomProductPageLocalizationsApi.AppCustomProductPageLocalizationsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appCustomProductPageLocalizationUpdateRequest** | [**AppCustomProductPageLocalizationUpdateRequest**](AppCustomProductPageLocalizationUpdateRequest.md) | AppCustomProductPageLocalization representation |  |

### Return type

[**AppCustomProductPageLocalizationResponse**](AppCustomProductPageLocalizationResponse.md)

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
| **200** | Single AppCustomProductPageLocalization |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

