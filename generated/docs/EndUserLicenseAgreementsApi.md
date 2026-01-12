# AppStoreConnect.Net.Api.EndUserLicenseAgreementsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**EndUserLicenseAgreementsCreateInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementscreateinstance) | **POST** /v1/endUserLicenseAgreements |  |
| [**EndUserLicenseAgreementsDeleteInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsdeleteinstance) | **DELETE** /v1/endUserLicenseAgreements/{id} |  |
| [**EndUserLicenseAgreementsGetInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsgetinstance) | **GET** /v1/endUserLicenseAgreements/{id} |  |
| [**EndUserLicenseAgreementsTerritoriesGetToManyRelated**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsterritoriesgettomanyrelated) | **GET** /v1/endUserLicenseAgreements/{id}/territories |  |
| [**EndUserLicenseAgreementsTerritoriesGetToManyRelationship**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsterritoriesgettomanyrelationship) | **GET** /v1/endUserLicenseAgreements/{id}/relationships/territories |  |
| [**EndUserLicenseAgreementsUpdateInstance**](EndUserLicenseAgreementsApi.md#enduserlicenseagreementsupdateinstance) | **PATCH** /v1/endUserLicenseAgreements/{id} |  |

<a id="enduserlicenseagreementscreateinstance"></a>
# **EndUserLicenseAgreementsCreateInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsCreateInstance (EndUserLicenseAgreementCreateRequest endUserLicenseAgreementCreateRequest)



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
    public class EndUserLicenseAgreementsCreateInstanceExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var endUserLicenseAgreementCreateRequest = new EndUserLicenseAgreementCreateRequest(); // EndUserLicenseAgreementCreateRequest | EndUserLicenseAgreement representation

            try
            {
                EndUserLicenseAgreementResponse result = apiInstance.EndUserLicenseAgreementsCreateInstance(endUserLicenseAgreementCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EndUserLicenseAgreementResponse> response = apiInstance.EndUserLicenseAgreementsCreateInstanceWithHttpInfo(endUserLicenseAgreementCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **endUserLicenseAgreementCreateRequest** | [**EndUserLicenseAgreementCreateRequest**](EndUserLicenseAgreementCreateRequest.md) | EndUserLicenseAgreement representation |  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **201** | Single EndUserLicenseAgreement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="enduserlicenseagreementsdeleteinstance"></a>
# **EndUserLicenseAgreementsDeleteInstance**
> void EndUserLicenseAgreementsDeleteInstance (string id)



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
    public class EndUserLicenseAgreementsDeleteInstanceExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.EndUserLicenseAgreementsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.EndUserLicenseAgreementsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="enduserlicenseagreementsgetinstance"></a>
# **EndUserLicenseAgreementsGetInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsGetInstance (string id, List<string>? fieldsEndUserLicenseAgreements = null, List<string>? fieldsTerritories = null, List<string>? include = null, int? limitTerritories = null)



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
    public class EndUserLicenseAgreementsGetInstanceExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsEndUserLicenseAgreements = new List<string>?(); // List<string>? | the fields to include for returned resources of type endUserLicenseAgreements (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitTerritories = 56;  // int? | maximum number of related territories returned (when they are included) (optional) 

            try
            {
                EndUserLicenseAgreementResponse result = apiInstance.EndUserLicenseAgreementsGetInstance(id, fieldsEndUserLicenseAgreements, fieldsTerritories, include, limitTerritories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EndUserLicenseAgreementResponse> response = apiInstance.EndUserLicenseAgreementsGetInstanceWithHttpInfo(id, fieldsEndUserLicenseAgreements, fieldsTerritories, include, limitTerritories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsEndUserLicenseAgreements** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type endUserLicenseAgreements | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitTerritories** | **int?** | maximum number of related territories returned (when they are included) | [optional]  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **200** | Single EndUserLicenseAgreement |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="enduserlicenseagreementsterritoriesgettomanyrelated"></a>
# **EndUserLicenseAgreementsTerritoriesGetToManyRelated**
> TerritoriesWithoutIncludesResponse EndUserLicenseAgreementsTerritoriesGetToManyRelated (string id, List<string>? fieldsTerritories = null, int? limit = null)



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
    public class EndUserLicenseAgreementsTerritoriesGetToManyRelatedExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                TerritoriesWithoutIncludesResponse result = apiInstance.EndUserLicenseAgreementsTerritoriesGetToManyRelated(id, fieldsTerritories, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsTerritoriesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsTerritoriesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TerritoriesWithoutIncludesResponse> response = apiInstance.EndUserLicenseAgreementsTerritoriesGetToManyRelatedWithHttpInfo(id, fieldsTerritories, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsTerritoriesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |

### Return type

[**TerritoriesWithoutIncludesResponse**](TerritoriesWithoutIncludesResponse.md)

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
| **200** | List of Territories with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="enduserlicenseagreementsterritoriesgettomanyrelationship"></a>
# **EndUserLicenseAgreementsTerritoriesGetToManyRelationship**
> EndUserLicenseAgreementTerritoriesLinkagesResponse EndUserLicenseAgreementsTerritoriesGetToManyRelationship (string id, int? limit = null)



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
    public class EndUserLicenseAgreementsTerritoriesGetToManyRelationshipExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                EndUserLicenseAgreementTerritoriesLinkagesResponse result = apiInstance.EndUserLicenseAgreementsTerritoriesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsTerritoriesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsTerritoriesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EndUserLicenseAgreementTerritoriesLinkagesResponse> response = apiInstance.EndUserLicenseAgreementsTerritoriesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsTerritoriesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**EndUserLicenseAgreementTerritoriesLinkagesResponse**](EndUserLicenseAgreementTerritoriesLinkagesResponse.md)

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

<a id="enduserlicenseagreementsupdateinstance"></a>
# **EndUserLicenseAgreementsUpdateInstance**
> EndUserLicenseAgreementResponse EndUserLicenseAgreementsUpdateInstance (string id, EndUserLicenseAgreementUpdateRequest endUserLicenseAgreementUpdateRequest)



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
    public class EndUserLicenseAgreementsUpdateInstanceExample
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
            var apiInstance = new EndUserLicenseAgreementsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var endUserLicenseAgreementUpdateRequest = new EndUserLicenseAgreementUpdateRequest(); // EndUserLicenseAgreementUpdateRequest | EndUserLicenseAgreement representation

            try
            {
                EndUserLicenseAgreementResponse result = apiInstance.EndUserLicenseAgreementsUpdateInstance(id, endUserLicenseAgreementUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the EndUserLicenseAgreementsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EndUserLicenseAgreementResponse> response = apiInstance.EndUserLicenseAgreementsUpdateInstanceWithHttpInfo(id, endUserLicenseAgreementUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EndUserLicenseAgreementsApi.EndUserLicenseAgreementsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **endUserLicenseAgreementUpdateRequest** | [**EndUserLicenseAgreementUpdateRequest**](EndUserLicenseAgreementUpdateRequest.md) | EndUserLicenseAgreement representation |  |

### Return type

[**EndUserLicenseAgreementResponse**](EndUserLicenseAgreementResponse.md)

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
| **200** | Single EndUserLicenseAgreement |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

