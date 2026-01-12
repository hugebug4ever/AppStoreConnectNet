# AppStoreConnect.Net.Api.SubscriptionAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesavailableterritoriesgettomanyrelated) | **GET** /v1/subscriptionAvailabilities/{id}/availableTerritories |  |
| [**SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesavailableterritoriesgettomanyrelationship) | **GET** /v1/subscriptionAvailabilities/{id}/relationships/availableTerritories |  |
| [**SubscriptionAvailabilitiesCreateInstance**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiescreateinstance) | **POST** /v1/subscriptionAvailabilities |  |
| [**SubscriptionAvailabilitiesGetInstance**](SubscriptionAvailabilitiesApi.md#subscriptionavailabilitiesgetinstance) | **GET** /v1/subscriptionAvailabilities/{id} |  |

<a id="subscriptionavailabilitiesavailableterritoriesgettomanyrelated"></a>
# **SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated**
> TerritoriesResponse SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated (string id, List<string>? fieldsTerritories = null, int? limit = null)



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
    public class SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionAvailabilitiesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                TerritoriesResponse result = apiInstance.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated(id, fieldsTerritories, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TerritoriesResponse> response = apiInstance.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelatedWithHttpInfo(id, fieldsTerritories, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelatedWithHttpInfo: " + e.Message);
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

[**TerritoriesResponse**](TerritoriesResponse.md)

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
| **200** | List of Territories |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionavailabilitiesavailableterritoriesgettomanyrelationship"></a>
# **SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship**
> SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionAvailabilitiesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse result = apiInstance.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse> response = apiInstance.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesAvailableTerritoriesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse**](SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.md)

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

<a id="subscriptionavailabilitiescreateinstance"></a>
# **SubscriptionAvailabilitiesCreateInstance**
> SubscriptionAvailabilityResponse SubscriptionAvailabilitiesCreateInstance (SubscriptionAvailabilityCreateRequest subscriptionAvailabilityCreateRequest)



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
    public class SubscriptionAvailabilitiesCreateInstanceExample
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
            var apiInstance = new SubscriptionAvailabilitiesApi(httpClient, config, httpClientHandler);
            var subscriptionAvailabilityCreateRequest = new SubscriptionAvailabilityCreateRequest(); // SubscriptionAvailabilityCreateRequest | SubscriptionAvailability representation

            try
            {
                SubscriptionAvailabilityResponse result = apiInstance.SubscriptionAvailabilitiesCreateInstance(subscriptionAvailabilityCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionAvailabilitiesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAvailabilityResponse> response = apiInstance.SubscriptionAvailabilitiesCreateInstanceWithHttpInfo(subscriptionAvailabilityCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionAvailabilityCreateRequest** | [**SubscriptionAvailabilityCreateRequest**](SubscriptionAvailabilityCreateRequest.md) | SubscriptionAvailability representation |  |

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
| **201** | Single SubscriptionAvailability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionavailabilitiesgetinstance"></a>
# **SubscriptionAvailabilitiesGetInstance**
> SubscriptionAvailabilityResponse SubscriptionAvailabilitiesGetInstance (string id, List<string>? fieldsSubscriptionAvailabilities = null, List<string>? fieldsTerritories = null, List<string>? include = null, int? limitAvailableTerritories = null)



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
    public class SubscriptionAvailabilitiesGetInstanceExample
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
            var apiInstance = new SubscriptionAvailabilitiesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionAvailabilities = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionAvailabilities (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAvailableTerritories = 56;  // int? | maximum number of related availableTerritories returned (when they are included) (optional) 

            try
            {
                SubscriptionAvailabilityResponse result = apiInstance.SubscriptionAvailabilitiesGetInstance(id, fieldsSubscriptionAvailabilities, fieldsTerritories, include, limitAvailableTerritories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionAvailabilitiesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAvailabilityResponse> response = apiInstance.SubscriptionAvailabilitiesGetInstanceWithHttpInfo(id, fieldsSubscriptionAvailabilities, fieldsTerritories, include, limitAvailableTerritories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionAvailabilitiesApi.SubscriptionAvailabilitiesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionAvailabilities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionAvailabilities | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAvailableTerritories** | **int?** | maximum number of related availableTerritories returned (when they are included) | [optional]  |

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
| **200** | Single SubscriptionAvailability |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

