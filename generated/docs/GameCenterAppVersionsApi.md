# AppStoreConnect.Net.Api.GameCenterAppVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAppVersionsAppStoreVersionGetToOneRelated**](GameCenterAppVersionsApi.md#gamecenterappversionsappstoreversiongettoonerelated) | **GET** /v1/gameCenterAppVersions/{id}/appStoreVersion |  |
| [**GameCenterAppVersionsAppStoreVersionGetToOneRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionsappstoreversiongettoonerelationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/appStoreVersion |  |
| [**GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionscreatetomanyrelationship) | **POST** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsdeletetomanyrelationship) | **DELETE** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsGetToManyRelated**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsgettomanyrelated) | **GET** /v1/gameCenterAppVersions/{id}/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsgettomanyrelationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCreateInstance**](GameCenterAppVersionsApi.md#gamecenterappversionscreateinstance) | **POST** /v1/gameCenterAppVersions |  |
| [**GameCenterAppVersionsGetInstance**](GameCenterAppVersionsApi.md#gamecenterappversionsgetinstance) | **GET** /v1/gameCenterAppVersions/{id} |  |
| [**GameCenterAppVersionsUpdateInstance**](GameCenterAppVersionsApi.md#gamecenterappversionsupdateinstance) | **PATCH** /v1/gameCenterAppVersions/{id} |  |

<a id="gamecenterappversionsappstoreversiongettoonerelated"></a>
# **GameCenterAppVersionsAppStoreVersionGetToOneRelated**
> AppStoreVersionResponse GameCenterAppVersionsAppStoreVersionGetToOneRelated (string id, List<string>? fieldsAppStoreVersions = null, List<string>? fieldsApps = null, List<string>? fieldsAgeRatingDeclarations = null, List<string>? fieldsAppStoreVersionLocalizations = null, List<string>? fieldsBuilds = null, List<string>? fieldsAppStoreVersionPhasedReleases = null, List<string>? fieldsGameCenterAppVersions = null, List<string>? fieldsRoutingAppCoverages = null, List<string>? fieldsAppStoreReviewDetails = null, List<string>? fieldsAppStoreVersionSubmissions = null, List<string>? fieldsAppClipDefaultExperiences = null, List<string>? fieldsAppStoreVersionExperiments = null, List<string>? fieldsAlternativeDistributionPackages = null, List<string>? include = null, int? limitAppStoreVersionLocalizations = null, int? limitAppStoreVersionExperiments = null, int? limitAppStoreVersionExperimentsV2 = null)



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
    public class GameCenterAppVersionsAppStoreVersionGetToOneRelatedExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var fieldsApps = new List<string>?(); // List<string>? | the fields to include for returned resources of type apps (optional) 
            var fieldsAgeRatingDeclarations = new List<string>?(); // List<string>? | the fields to include for returned resources of type ageRatingDeclarations (optional) 
            var fieldsAppStoreVersionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionLocalizations (optional) 
            var fieldsBuilds = new List<string>?(); // List<string>? | the fields to include for returned resources of type builds (optional) 
            var fieldsAppStoreVersionPhasedReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionPhasedReleases (optional) 
            var fieldsGameCenterAppVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAppVersions (optional) 
            var fieldsRoutingAppCoverages = new List<string>?(); // List<string>? | the fields to include for returned resources of type routingAppCoverages (optional) 
            var fieldsAppStoreReviewDetails = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreReviewDetails (optional) 
            var fieldsAppStoreVersionSubmissions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionSubmissions (optional) 
            var fieldsAppClipDefaultExperiences = new List<string>?(); // List<string>? | the fields to include for returned resources of type appClipDefaultExperiences (optional) 
            var fieldsAppStoreVersionExperiments = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersionExperiments (optional) 
            var fieldsAlternativeDistributionPackages = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAppStoreVersionLocalizations = 56;  // int? | maximum number of related appStoreVersionLocalizations returned (when they are included) (optional) 
            var limitAppStoreVersionExperiments = 56;  // int? | maximum number of related appStoreVersionExperiments returned (when they are included) (optional) 
            var limitAppStoreVersionExperimentsV2 = 56;  // int? | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional) 

            try
            {
                AppStoreVersionResponse result = apiInstance.GameCenterAppVersionsAppStoreVersionGetToOneRelated(id, fieldsAppStoreVersions, fieldsApps, fieldsAgeRatingDeclarations, fieldsAppStoreVersionLocalizations, fieldsBuilds, fieldsAppStoreVersionPhasedReleases, fieldsGameCenterAppVersions, fieldsRoutingAppCoverages, fieldsAppStoreReviewDetails, fieldsAppStoreVersionSubmissions, fieldsAppClipDefaultExperiences, fieldsAppStoreVersionExperiments, fieldsAlternativeDistributionPackages, include, limitAppStoreVersionLocalizations, limitAppStoreVersionExperiments, limitAppStoreVersionExperimentsV2);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsAppStoreVersionGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsAppStoreVersionGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AppStoreVersionResponse> response = apiInstance.GameCenterAppVersionsAppStoreVersionGetToOneRelatedWithHttpInfo(id, fieldsAppStoreVersions, fieldsApps, fieldsAgeRatingDeclarations, fieldsAppStoreVersionLocalizations, fieldsBuilds, fieldsAppStoreVersionPhasedReleases, fieldsGameCenterAppVersions, fieldsRoutingAppCoverages, fieldsAppStoreReviewDetails, fieldsAppStoreVersionSubmissions, fieldsAppClipDefaultExperiences, fieldsAppStoreVersionExperiments, fieldsAlternativeDistributionPackages, include, limitAppStoreVersionLocalizations, limitAppStoreVersionExperiments, limitAppStoreVersionExperimentsV2);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsAppStoreVersionGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsAppStoreVersionPhasedReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsRoutingAppCoverages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type routingAppCoverages | [optional]  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **fieldsAppStoreVersionSubmissions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionSubmissions | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionLocalizations** | **int?** | maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperiments** | **int?** | maximum number of related appStoreVersionExperiments returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int?** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
| **200** | Single AppStoreVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterappversionsappstoreversiongettoonerelationship"></a>
# **GameCenterAppVersionsAppStoreVersionGetToOneRelationship**
> GameCenterAppVersionAppStoreVersionLinkageResponse GameCenterAppVersionsAppStoreVersionGetToOneRelationship (string id)



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
    public class GameCenterAppVersionsAppStoreVersionGetToOneRelationshipExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                GameCenterAppVersionAppStoreVersionLinkageResponse result = apiInstance.GameCenterAppVersionsAppStoreVersionGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsAppStoreVersionGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsAppStoreVersionGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionAppStoreVersionLinkageResponse> response = apiInstance.GameCenterAppVersionsAppStoreVersionGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsAppStoreVersionGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAppVersionAppStoreVersionLinkageResponse**](GameCenterAppVersionAppStoreVersionLinkageResponse.md)

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

<a id="gamecenterappversionscompatibilityversionscreatetomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship**
> void GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship (string id, GameCenterAppVersionCompatibilityVersionsLinkagesRequest gameCenterAppVersionCompatibilityVersionsLinkagesRequest)



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
    public class GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationshipExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterAppVersionCompatibilityVersionsLinkagesRequest = new GameCenterAppVersionCompatibilityVersionsLinkagesRequest(); // GameCenterAppVersionCompatibilityVersionsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship(id, gameCenterAppVersionCompatibilityVersionsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationshipWithHttpInfo(id, gameCenterAppVersionCompatibilityVersionsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionCompatibilityVersionsLinkagesRequest** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterappversionscompatibilityversionsdeletetomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship**
> void GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship (string id, GameCenterAppVersionCompatibilityVersionsLinkagesRequest gameCenterAppVersionCompatibilityVersionsLinkagesRequest)



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
    public class GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationshipExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterAppVersionCompatibilityVersionsLinkagesRequest = new GameCenterAppVersionCompatibilityVersionsLinkagesRequest(); // GameCenterAppVersionCompatibilityVersionsLinkagesRequest | List of related linkages

            try
            {
                apiInstance.GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship(id, gameCenterAppVersionCompatibilityVersionsLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationshipWithHttpInfo(id, gameCenterAppVersionCompatibilityVersionsLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionCompatibilityVersionsLinkagesRequest** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterappversionscompatibilityversionsgettomanyrelated"></a>
# **GameCenterAppVersionsCompatibilityVersionsGetToManyRelated**
> GameCenterAppVersionsResponse GameCenterAppVersionsCompatibilityVersionsGetToManyRelated (string id, List<string>? filterEnabled = null, List<string>? fieldsGameCenterAppVersions = null, List<string>? fieldsAppStoreVersions = null, int? limit = null, List<string>? include = null, int? limitCompatibilityVersions = null)



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
    public class GameCenterAppVersionsCompatibilityVersionsGetToManyRelatedExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterEnabled = new List<string>?(); // List<string>? | filter by attribute 'enabled' (optional) 
            var fieldsGameCenterAppVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAppVersions (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCompatibilityVersions = 56;  // int? | maximum number of related compatibilityVersions returned (when they are included) (optional) 

            try
            {
                GameCenterAppVersionsResponse result = apiInstance.GameCenterAppVersionsCompatibilityVersionsGetToManyRelated(id, filterEnabled, fieldsGameCenterAppVersions, fieldsAppStoreVersions, limit, include, limitCompatibilityVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsCompatibilityVersionsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionsResponse> response = apiInstance.GameCenterAppVersionsCompatibilityVersionsGetToManyRelatedWithHttpInfo(id, filterEnabled, fieldsGameCenterAppVersions, fieldsAppStoreVersions, limit, include, limitCompatibilityVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterEnabled** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;enabled&#39; | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCompatibilityVersions** | **int?** | maximum number of related compatibilityVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAppVersionsResponse**](GameCenterAppVersionsResponse.md)

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
| **200** | List of GameCenterAppVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterappversionscompatibilityversionsgettomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship**
> GameCenterAppVersionCompatibilityVersionsLinkagesResponse GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship (string id, int? limit = null)



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
    public class GameCenterAppVersionsCompatibilityVersionsGetToManyRelationshipExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                GameCenterAppVersionCompatibilityVersionsLinkagesResponse result = apiInstance.GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsCompatibilityVersionsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionCompatibilityVersionsLinkagesResponse> response = apiInstance.GameCenterAppVersionsCompatibilityVersionsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCompatibilityVersionsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**GameCenterAppVersionCompatibilityVersionsLinkagesResponse**](GameCenterAppVersionCompatibilityVersionsLinkagesResponse.md)

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

<a id="gamecenterappversionscreateinstance"></a>
# **GameCenterAppVersionsCreateInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsCreateInstance (GameCenterAppVersionCreateRequest gameCenterAppVersionCreateRequest)



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
    public class GameCenterAppVersionsCreateInstanceExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var gameCenterAppVersionCreateRequest = new GameCenterAppVersionCreateRequest(); // GameCenterAppVersionCreateRequest | GameCenterAppVersion representation

            try
            {
                GameCenterAppVersionResponse result = apiInstance.GameCenterAppVersionsCreateInstance(gameCenterAppVersionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionResponse> response = apiInstance.GameCenterAppVersionsCreateInstanceWithHttpInfo(gameCenterAppVersionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAppVersionCreateRequest** | [**GameCenterAppVersionCreateRequest**](GameCenterAppVersionCreateRequest.md) | GameCenterAppVersion representation |  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **201** | Single GameCenterAppVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterappversionsgetinstance"></a>
# **GameCenterAppVersionsGetInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsGetInstance (string id, List<string>? fieldsGameCenterAppVersions = null, List<string>? fieldsAppStoreVersions = null, List<string>? include = null, int? limitCompatibilityVersions = null)



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
    public class GameCenterAppVersionsGetInstanceExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsGameCenterAppVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type gameCenterAppVersions (optional) 
            var fieldsAppStoreVersions = new List<string>?(); // List<string>? | the fields to include for returned resources of type appStoreVersions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCompatibilityVersions = 56;  // int? | maximum number of related compatibilityVersions returned (when they are included) (optional) 

            try
            {
                GameCenterAppVersionResponse result = apiInstance.GameCenterAppVersionsGetInstance(id, fieldsGameCenterAppVersions, fieldsAppStoreVersions, include, limitCompatibilityVersions);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionResponse> response = apiInstance.GameCenterAppVersionsGetInstanceWithHttpInfo(id, fieldsGameCenterAppVersions, fieldsAppStoreVersions, include, limitCompatibilityVersions);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCompatibilityVersions** | **int?** | maximum number of related compatibilityVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **200** | Single GameCenterAppVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="gamecenterappversionsupdateinstance"></a>
# **GameCenterAppVersionsUpdateInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsUpdateInstance (string id, GameCenterAppVersionUpdateRequest gameCenterAppVersionUpdateRequest)



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
    public class GameCenterAppVersionsUpdateInstanceExample
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
            var apiInstance = new GameCenterAppVersionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var gameCenterAppVersionUpdateRequest = new GameCenterAppVersionUpdateRequest(); // GameCenterAppVersionUpdateRequest | GameCenterAppVersion representation

            try
            {
                GameCenterAppVersionResponse result = apiInstance.GameCenterAppVersionsUpdateInstance(id, gameCenterAppVersionUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GameCenterAppVersionsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<GameCenterAppVersionResponse> response = apiInstance.GameCenterAppVersionsUpdateInstanceWithHttpInfo(id, gameCenterAppVersionUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GameCenterAppVersionsApi.GameCenterAppVersionsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionUpdateRequest** | [**GameCenterAppVersionUpdateRequest**](GameCenterAppVersionUpdateRequest.md) | GameCenterAppVersion representation |  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **200** | Single GameCenterAppVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

