# AppStoreConnect.Net.Api.TerritoryAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**TerritoryAvailabilitiesUpdateInstance**](TerritoryAvailabilitiesApi.md#territoryavailabilitiesupdateinstance) | **PATCH** /v1/territoryAvailabilities/{id} |  |

<a id="territoryavailabilitiesupdateinstance"></a>
# **TerritoryAvailabilitiesUpdateInstance**
> TerritoryAvailabilityResponse TerritoryAvailabilitiesUpdateInstance (string id, TerritoryAvailabilityUpdateRequest territoryAvailabilityUpdateRequest)



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
    public class TerritoryAvailabilitiesUpdateInstanceExample
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
            var apiInstance = new TerritoryAvailabilitiesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var territoryAvailabilityUpdateRequest = new TerritoryAvailabilityUpdateRequest(); // TerritoryAvailabilityUpdateRequest | TerritoryAvailability representation

            try
            {
                TerritoryAvailabilityResponse result = apiInstance.TerritoryAvailabilitiesUpdateInstance(id, territoryAvailabilityUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TerritoryAvailabilitiesApi.TerritoryAvailabilitiesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TerritoryAvailabilitiesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TerritoryAvailabilityResponse> response = apiInstance.TerritoryAvailabilitiesUpdateInstanceWithHttpInfo(id, territoryAvailabilityUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TerritoryAvailabilitiesApi.TerritoryAvailabilitiesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **territoryAvailabilityUpdateRequest** | [**TerritoryAvailabilityUpdateRequest**](TerritoryAvailabilityUpdateRequest.md) | TerritoryAvailability representation |  |

### Return type

[**TerritoryAvailabilityResponse**](TerritoryAvailabilityResponse.md)

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
| **200** | Single TerritoryAvailability |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

