# AppStoreConnect.Net.Api.AlternativeDistributionPackageDeltasApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackageDeltasGetInstance**](AlternativeDistributionPackageDeltasApi.md#alternativedistributionpackagedeltasgetinstance) | **GET** /v1/alternativeDistributionPackageDeltas/{id} |  |

<a id="alternativedistributionpackagedeltasgetinstance"></a>
# **AlternativeDistributionPackageDeltasGetInstance**
> AlternativeDistributionPackageDeltaResponse AlternativeDistributionPackageDeltasGetInstance (string id, List<string>? fieldsAlternativeDistributionPackageDeltas = null)



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
    public class AlternativeDistributionPackageDeltasGetInstanceExample
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
            var apiInstance = new AlternativeDistributionPackageDeltasApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackageDeltas = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional) 

            try
            {
                AlternativeDistributionPackageDeltaResponse result = apiInstance.AlternativeDistributionPackageDeltasGetInstance(id, fieldsAlternativeDistributionPackageDeltas);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageDeltasApi.AlternativeDistributionPackageDeltasGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageDeltasGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageDeltaResponse> response = apiInstance.AlternativeDistributionPackageDeltasGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionPackageDeltas);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageDeltasApi.AlternativeDistributionPackageDeltasGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageDeltas** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional]  |

### Return type

[**AlternativeDistributionPackageDeltaResponse**](AlternativeDistributionPackageDeltaResponse.md)

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
| **200** | Single AlternativeDistributionPackageDelta |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

