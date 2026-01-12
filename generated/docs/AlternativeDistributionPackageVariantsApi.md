# AppStoreConnect.Net.Api.AlternativeDistributionPackageVariantsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackageVariantsGetInstance**](AlternativeDistributionPackageVariantsApi.md#alternativedistributionpackagevariantsgetinstance) | **GET** /v1/alternativeDistributionPackageVariants/{id} |  |

<a id="alternativedistributionpackagevariantsgetinstance"></a>
# **AlternativeDistributionPackageVariantsGetInstance**
> AlternativeDistributionPackageVariantResponse AlternativeDistributionPackageVariantsGetInstance (string id, List<string>? fieldsAlternativeDistributionPackageVariants = null)



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
    public class AlternativeDistributionPackageVariantsGetInstanceExample
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
            var apiInstance = new AlternativeDistributionPackageVariantsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsAlternativeDistributionPackageVariants = new List<string>?(); // List<string>? | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional) 

            try
            {
                AlternativeDistributionPackageVariantResponse result = apiInstance.AlternativeDistributionPackageVariantsGetInstance(id, fieldsAlternativeDistributionPackageVariants);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AlternativeDistributionPackageVariantsApi.AlternativeDistributionPackageVariantsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the AlternativeDistributionPackageVariantsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AlternativeDistributionPackageVariantResponse> response = apiInstance.AlternativeDistributionPackageVariantsGetInstanceWithHttpInfo(id, fieldsAlternativeDistributionPackageVariants);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AlternativeDistributionPackageVariantsApi.AlternativeDistributionPackageVariantsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |

### Return type

[**AlternativeDistributionPackageVariantResponse**](AlternativeDistributionPackageVariantResponse.md)

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
| **200** | Single AlternativeDistributionPackageVariant |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

