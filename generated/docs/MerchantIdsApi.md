# AppStoreConnect.Net.Api.MerchantIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MerchantIdsCertificatesGetToManyRelated**](MerchantIdsApi.md#merchantidscertificatesgettomanyrelated) | **GET** /v1/merchantIds/{id}/certificates |  |
| [**MerchantIdsCertificatesGetToManyRelationship**](MerchantIdsApi.md#merchantidscertificatesgettomanyrelationship) | **GET** /v1/merchantIds/{id}/relationships/certificates |  |
| [**MerchantIdsCreateInstance**](MerchantIdsApi.md#merchantidscreateinstance) | **POST** /v1/merchantIds |  |
| [**MerchantIdsDeleteInstance**](MerchantIdsApi.md#merchantidsdeleteinstance) | **DELETE** /v1/merchantIds/{id} |  |
| [**MerchantIdsGetCollection**](MerchantIdsApi.md#merchantidsgetcollection) | **GET** /v1/merchantIds |  |
| [**MerchantIdsGetInstance**](MerchantIdsApi.md#merchantidsgetinstance) | **GET** /v1/merchantIds/{id} |  |
| [**MerchantIdsUpdateInstance**](MerchantIdsApi.md#merchantidsupdateinstance) | **PATCH** /v1/merchantIds/{id} |  |

<a id="merchantidscertificatesgettomanyrelated"></a>
# **MerchantIdsCertificatesGetToManyRelated**
> CertificatesResponse MerchantIdsCertificatesGetToManyRelated (string id, List<string>? filterDisplayName = null, List<string>? filterCertificateType = null, List<string>? filterSerialNumber = null, List<string>? filterId = null, List<string>? sort = null, List<string>? fieldsCertificates = null, List<string>? fieldsPassTypeIds = null, int? limit = null, List<string>? include = null)



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
    public class MerchantIdsCertificatesGetToManyRelatedExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterDisplayName = new List<string>?(); // List<string>? | filter by attribute 'displayName' (optional) 
            var filterCertificateType = new List<string>?(); // List<string>? | filter by attribute 'certificateType' (optional) 
            var filterSerialNumber = new List<string>?(); // List<string>? | filter by attribute 'serialNumber' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var fieldsPassTypeIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type passTypeIds (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CertificatesResponse result = apiInstance.MerchantIdsCertificatesGetToManyRelated(id, filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCertificatesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsCertificatesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificatesResponse> response = apiInstance.MerchantIdsCertificatesGetToManyRelatedWithHttpInfo(id, filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCertificatesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterDisplayName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;displayName&#39; | [optional]  |
| **filterCertificateType** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;certificateType&#39; | [optional]  |
| **filterSerialNumber** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;serialNumber&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CertificatesResponse**](CertificatesResponse.md)

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
| **200** | List of Certificates |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="merchantidscertificatesgettomanyrelationship"></a>
# **MerchantIdsCertificatesGetToManyRelationship**
> MerchantIdCertificatesLinkagesResponse MerchantIdsCertificatesGetToManyRelationship (string id, int? limit = null)



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
    public class MerchantIdsCertificatesGetToManyRelationshipExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                MerchantIdCertificatesLinkagesResponse result = apiInstance.MerchantIdsCertificatesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCertificatesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsCertificatesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MerchantIdCertificatesLinkagesResponse> response = apiInstance.MerchantIdsCertificatesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCertificatesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**MerchantIdCertificatesLinkagesResponse**](MerchantIdCertificatesLinkagesResponse.md)

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

<a id="merchantidscreateinstance"></a>
# **MerchantIdsCreateInstance**
> MerchantIdResponse MerchantIdsCreateInstance (MerchantIdCreateRequest merchantIdCreateRequest)



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
    public class MerchantIdsCreateInstanceExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var merchantIdCreateRequest = new MerchantIdCreateRequest(); // MerchantIdCreateRequest | MerchantId representation

            try
            {
                MerchantIdResponse result = apiInstance.MerchantIdsCreateInstance(merchantIdCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MerchantIdResponse> response = apiInstance.MerchantIdsCreateInstanceWithHttpInfo(merchantIdCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **merchantIdCreateRequest** | [**MerchantIdCreateRequest**](MerchantIdCreateRequest.md) | MerchantId representation |  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **201** | Single MerchantId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="merchantidsdeleteinstance"></a>
# **MerchantIdsDeleteInstance**
> void MerchantIdsDeleteInstance (string id)



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
    public class MerchantIdsDeleteInstanceExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.MerchantIdsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.MerchantIdsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="merchantidsgetcollection"></a>
# **MerchantIdsGetCollection**
> MerchantIdsResponse MerchantIdsGetCollection (List<string>? filterName = null, List<string>? filterIdentifier = null, List<string>? sort = null, List<string>? fieldsMerchantIds = null, List<string>? fieldsCertificates = null, int? limit = null, List<string>? include = null, int? limitCertificates = null)



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
    public class MerchantIdsGetCollectionExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var filterName = new List<string>?(); // List<string>? | filter by attribute 'name' (optional) 
            var filterIdentifier = new List<string>?(); // List<string>? | filter by attribute 'identifier' (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsMerchantIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type merchantIds (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCertificates = 56;  // int? | maximum number of related certificates returned (when they are included) (optional) 

            try
            {
                MerchantIdsResponse result = apiInstance.MerchantIdsGetCollection(filterName, filterIdentifier, sort, fieldsMerchantIds, fieldsCertificates, limit, include, limitCertificates);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MerchantIdsResponse> response = apiInstance.MerchantIdsGetCollectionWithHttpInfo(filterName, filterIdentifier, sort, fieldsMerchantIds, fieldsCertificates, limit, include, limitCertificates);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIdentifier** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;identifier&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsMerchantIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type merchantIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int?** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**MerchantIdsResponse**](MerchantIdsResponse.md)

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
| **200** | List of MerchantIds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="merchantidsgetinstance"></a>
# **MerchantIdsGetInstance**
> MerchantIdResponse MerchantIdsGetInstance (string id, List<string>? fieldsMerchantIds = null, List<string>? fieldsCertificates = null, List<string>? include = null, int? limitCertificates = null)



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
    public class MerchantIdsGetInstanceExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsMerchantIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type merchantIds (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCertificates = 56;  // int? | maximum number of related certificates returned (when they are included) (optional) 

            try
            {
                MerchantIdResponse result = apiInstance.MerchantIdsGetInstance(id, fieldsMerchantIds, fieldsCertificates, include, limitCertificates);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MerchantIdResponse> response = apiInstance.MerchantIdsGetInstanceWithHttpInfo(id, fieldsMerchantIds, fieldsCertificates, include, limitCertificates);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsMerchantIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type merchantIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int?** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **200** | Single MerchantId |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="merchantidsupdateinstance"></a>
# **MerchantIdsUpdateInstance**
> MerchantIdResponse MerchantIdsUpdateInstance (string id, MerchantIdUpdateRequest merchantIdUpdateRequest)



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
    public class MerchantIdsUpdateInstanceExample
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
            var apiInstance = new MerchantIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var merchantIdUpdateRequest = new MerchantIdUpdateRequest(); // MerchantIdUpdateRequest | MerchantId representation

            try
            {
                MerchantIdResponse result = apiInstance.MerchantIdsUpdateInstance(id, merchantIdUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MerchantIdsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<MerchantIdResponse> response = apiInstance.MerchantIdsUpdateInstanceWithHttpInfo(id, merchantIdUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MerchantIdsApi.MerchantIdsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **merchantIdUpdateRequest** | [**MerchantIdUpdateRequest**](MerchantIdUpdateRequest.md) | MerchantId representation |  |

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
| **200** | Single MerchantId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

