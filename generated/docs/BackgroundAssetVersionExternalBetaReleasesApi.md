# AppStoreConnect.Net.Api.BackgroundAssetVersionExternalBetaReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BackgroundAssetVersionExternalBetaReleasesGetInstance**](BackgroundAssetVersionExternalBetaReleasesApi.md#backgroundassetversionexternalbetareleasesgetinstance) | **GET** /v1/backgroundAssetVersionExternalBetaReleases/{id} |  |

<a id="backgroundassetversionexternalbetareleasesgetinstance"></a>
# **BackgroundAssetVersionExternalBetaReleasesGetInstance**
> BackgroundAssetVersionExternalBetaReleaseResponse BackgroundAssetVersionExternalBetaReleasesGetInstance (string id, List<string>? fieldsBackgroundAssetVersionExternalBetaReleases = null, List<string>? include = null)



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
    public class BackgroundAssetVersionExternalBetaReleasesGetInstanceExample
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
            var apiInstance = new BackgroundAssetVersionExternalBetaReleasesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsBackgroundAssetVersionExternalBetaReleases = new List<string>?(); // List<string>? | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                BackgroundAssetVersionExternalBetaReleaseResponse result = apiInstance.BackgroundAssetVersionExternalBetaReleasesGetInstance(id, fieldsBackgroundAssetVersionExternalBetaReleases, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BackgroundAssetVersionExternalBetaReleasesApi.BackgroundAssetVersionExternalBetaReleasesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BackgroundAssetVersionExternalBetaReleasesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<BackgroundAssetVersionExternalBetaReleaseResponse> response = apiInstance.BackgroundAssetVersionExternalBetaReleasesGetInstanceWithHttpInfo(id, fieldsBackgroundAssetVersionExternalBetaReleases, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BackgroundAssetVersionExternalBetaReleasesApi.BackgroundAssetVersionExternalBetaReleasesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBackgroundAssetVersionExternalBetaReleases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type backgroundAssetVersionExternalBetaReleases | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BackgroundAssetVersionExternalBetaReleaseResponse**](BackgroundAssetVersionExternalBetaReleaseResponse.md)

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
| **200** | Single BackgroundAssetVersionExternalBetaRelease |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

