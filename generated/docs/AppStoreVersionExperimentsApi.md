# AppStoreConnect.Net.Api.AppStoreVersionExperimentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelated) | **GET** /v1/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelationship) | **GET** /v1/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsCreateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentscreateinstance) | **POST** /v1/appStoreVersionExperiments |  |
| [**AppStoreVersionExperimentsDeleteInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsdeleteinstance) | **DELETE** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsGetInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsgetinstance) | **GET** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsUpdateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsupdateinstance) | **PATCH** /v1/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelated) | **GET** /v2/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelationship) | **GET** /v2/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments |  |
| [**AppStoreVersionExperimentsV2CreateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2createinstance) | **POST** /v2/appStoreVersionExperiments |  |
| [**AppStoreVersionExperimentsV2DeleteInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2deleteinstance) | **DELETE** /v2/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2GetInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2getinstance) | **GET** /v2/appStoreVersionExperiments/{id} |  |
| [**AppStoreVersionExperimentsV2UpdateInstance**](AppStoreVersionExperimentsApi.md#appstoreversionexperimentsv2updateinstance) | **PATCH** /v2/appStoreVersionExperiments/{id} |  |

<a id="appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelated"></a>
# **AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated**
> AppStoreVersionExperimentTreatmentsResponse AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated (string id, List<string>? fieldsAppStoreVersionExperimentTreatments = null, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, int? limit = null, List<string>? include = null, int? limitAppStoreVersionExperimentTreatmentLocalizations = null)



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
    public class AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionExperimentTreatments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional) 
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAppStoreVersionExperimentTreatmentLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionExperimentTreatmentLocalizations = 56;  // int? | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) (optional) 

            try
            {
                AppStoreVersionExperimentTreatmentsResponse result = apiInstance.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated(id, fieldsAppStoreVersionExperimentTreatments, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatmentLocalizations, limit, include, limitAppStoreVersionExperimentTreatmentLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentsResponse> response = apiInstance.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo(id, fieldsAppStoreVersionExperimentTreatments, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatmentLocalizations, limit, include, limitAppStoreVersionExperimentTreatmentLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatmentLocalizations** | **int?** | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
| **200** | List of AppStoreVersionExperimentTreatments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsappstoreversionexperimenttreatmentsgettomanyrelationship"></a>
# **AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship**
> AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse result = apiInstance.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse> response = apiInstance.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsAppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

<a id="appstoreversionexperimentscreateinstance"></a>
# **AppStoreVersionExperimentsCreateInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsCreateInstance (AppStoreVersionExperimentCreateRequest appStoreVersionExperimentCreateRequest)



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
    public class AppStoreVersionExperimentsCreateInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var appStoreVersionExperimentCreateRequest = new AppStoreVersionExperimentCreateRequest(); // AppStoreVersionExperimentCreateRequest | AppStoreVersionExperiment representation

            try
            {
                AppStoreVersionExperimentResponse result = apiInstance.AppStoreVersionExperimentsCreateInstance(appStoreVersionExperimentCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentResponse> response = apiInstance.AppStoreVersionExperimentsCreateInstanceWithHttpInfo(appStoreVersionExperimentCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentCreateRequest** | [**AppStoreVersionExperimentCreateRequest**](AppStoreVersionExperimentCreateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **201** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsdeleteinstance"></a>
# **AppStoreVersionExperimentsDeleteInstance**
> void AppStoreVersionExperimentsDeleteInstance (string id)



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
    public class AppStoreVersionExperimentsDeleteInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppStoreVersionExperimentsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionExperimentsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appstoreversionexperimentsgetinstance"></a>
# **AppStoreVersionExperimentsGetInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsGetInstance (string id, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAppStoreVersionExperimentTreatments = null, List<string>? include = null, int? limitAppStoreVersionExperimentTreatments = null)



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
    public class AppStoreVersionExperimentsGetInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAppStoreVersionExperimentTreatments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionExperimentTreatments = 56;  // int? | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) (optional) 

            try
            {
                AppStoreVersionExperimentResponse result = apiInstance.AppStoreVersionExperimentsGetInstance(id, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatments, include, limitAppStoreVersionExperimentTreatments);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentResponse> response = apiInstance.AppStoreVersionExperimentsGetInstanceWithHttpInfo(id, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatments, include, limitAppStoreVersionExperimentTreatments);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatments** | **int?** | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsupdateinstance"></a>
# **AppStoreVersionExperimentsUpdateInstance**
> AppStoreVersionExperimentResponse AppStoreVersionExperimentsUpdateInstance (string id, AppStoreVersionExperimentUpdateRequest appStoreVersionExperimentUpdateRequest)



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
    public class AppStoreVersionExperimentsUpdateInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appStoreVersionExperimentUpdateRequest = new AppStoreVersionExperimentUpdateRequest(); // AppStoreVersionExperimentUpdateRequest | AppStoreVersionExperiment representation

            try
            {
                AppStoreVersionExperimentResponse result = apiInstance.AppStoreVersionExperimentsUpdateInstance(id, appStoreVersionExperimentUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentResponse> response = apiInstance.AppStoreVersionExperimentsUpdateInstanceWithHttpInfo(id, appStoreVersionExperimentUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionExperimentUpdateRequest** | [**AppStoreVersionExperimentUpdateRequest**](AppStoreVersionExperimentUpdateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelated"></a>
# **AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated**
> AppStoreVersionExperimentTreatmentsResponse AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated (string id, List<string>? fieldsAppStoreVersionExperimentTreatments = null, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAppStoreVersionExperimentTreatmentLocalizations = null, int? limit = null, List<string>? include = null, int? limitAppStoreVersionExperimentTreatmentLocalizations = null)



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
    public class AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelatedExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionExperimentTreatments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional) 
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAppStoreVersionExperimentTreatmentLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionExperimentTreatmentLocalizations = 56;  // int? | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) (optional) 

            try
            {
                AppStoreVersionExperimentTreatmentsResponse result = apiInstance.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated(id, fieldsAppStoreVersionExperimentTreatments, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatmentLocalizations, limit, include, limitAppStoreVersionExperimentTreatmentLocalizations);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentTreatmentsResponse> response = apiInstance.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo(id, fieldsAppStoreVersionExperimentTreatments, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatmentLocalizations, limit, include, limitAppStoreVersionExperimentTreatmentLocalizations);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatmentLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatmentLocalizations** | **int?** | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
| **200** | List of AppStoreVersionExperimentTreatments |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsv2appstoreversionexperimenttreatmentsgettomanyrelationship"></a>
# **AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship**
> AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship (string id, int? limit = null)



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
    public class AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationshipExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse result = apiInstance.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse> response = apiInstance.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2AppStoreVersionExperimentTreatmentsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

<a id="appstoreversionexperimentsv2createinstance"></a>
# **AppStoreVersionExperimentsV2CreateInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2CreateInstance (AppStoreVersionExperimentV2CreateRequest appStoreVersionExperimentV2CreateRequest)



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
    public class AppStoreVersionExperimentsV2CreateInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var appStoreVersionExperimentV2CreateRequest = new AppStoreVersionExperimentV2CreateRequest(); // AppStoreVersionExperimentV2CreateRequest | AppStoreVersionExperiment representation

            try
            {
                AppStoreVersionExperimentV2Response result = apiInstance.AppStoreVersionExperimentsV2CreateInstance(appStoreVersionExperimentV2CreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2CreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2CreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentV2Response> response = apiInstance.AppStoreVersionExperimentsV2CreateInstanceWithHttpInfo(appStoreVersionExperimentV2CreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2CreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionExperimentV2CreateRequest** | [**AppStoreVersionExperimentV2CreateRequest**](AppStoreVersionExperimentV2CreateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **201** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsv2deleteinstance"></a>
# **AppStoreVersionExperimentsV2DeleteInstance**
> void AppStoreVersionExperimentsV2DeleteInstance (string id)



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
    public class AppStoreVersionExperimentsV2DeleteInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.AppStoreVersionExperimentsV2DeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2DeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2DeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.AppStoreVersionExperimentsV2DeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2DeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="appstoreversionexperimentsv2getinstance"></a>
# **AppStoreVersionExperimentsV2GetInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2GetInstance (string id, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAppStoreVersionExperimentTreatments = null, List<string>? include = null, int? limitAppStoreVersionExperimentTreatments = null, int? limitControlVersions = null)



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
    public class AppStoreVersionExperimentsV2GetInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAppStoreVersionExperimentTreatments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionExperimentTreatments = 56;  // int? | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) (optional) 
            var limitControlVersions = 56;  // int? | maximum number of related controlVersions returned (when they are included) (optional) 

            try
            {
                AppStoreVersionExperimentV2Response result = apiInstance.AppStoreVersionExperimentsV2GetInstance(id, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatments, include, limitAppStoreVersionExperimentTreatments, limitControlVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2GetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2GetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentV2Response> response = apiInstance.AppStoreVersionExperimentsV2GetInstanceWithHttpInfo(id, fieldsAppStoreVersionExperiments, fieldsAppStoreVersionExperimentTreatments, include, limitAppStoreVersionExperimentTreatments, limitControlVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2GetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppStoreVersionExperimentTreatments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionExperimentTreatments** | **int?** | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional]  |
| **limitControlVersions** | **int?** | maximum number of related controlVersions returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="appstoreversionexperimentsv2updateinstance"></a>
# **AppStoreVersionExperimentsV2UpdateInstance**
> AppStoreVersionExperimentV2Response AppStoreVersionExperimentsV2UpdateInstance (string id, AppStoreVersionExperimentV2UpdateRequest appStoreVersionExperimentV2UpdateRequest)



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
    public class AppStoreVersionExperimentsV2UpdateInstanceExample
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
            var apiInstance = new AppStoreVersionExperimentsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var appStoreVersionExperimentV2UpdateRequest = new AppStoreVersionExperimentV2UpdateRequest(); // AppStoreVersionExperimentV2UpdateRequest | AppStoreVersionExperiment representation

            try
            {
                AppStoreVersionExperimentV2Response result = apiInstance.AppStoreVersionExperimentsV2UpdateInstance(id, appStoreVersionExperimentV2UpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2UpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AppStoreVersionExperimentsV2UpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionExperimentV2Response> response = apiInstance.AppStoreVersionExperimentsV2UpdateInstanceWithHttpInfo(id, appStoreVersionExperimentV2UpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AppStoreVersionExperimentsApi.AppStoreVersionExperimentsV2UpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **appStoreVersionExperimentV2UpdateRequest** | [**AppStoreVersionExperimentV2UpdateRequest**](AppStoreVersionExperimentV2UpdateRequest.md) | AppStoreVersionExperiment representation |  |

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
| **200** | Single AppStoreVersionExperiment |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

