# AppStoreConnect.Net.Api.CertificatesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CertificatesCreateInstance**](CertificatesApi.md#certificatescreateinstance) | **POST** /v1/certificates |  |
| [**CertificatesDeleteInstance**](CertificatesApi.md#certificatesdeleteinstance) | **DELETE** /v1/certificates/{id} |  |
| [**CertificatesGetCollection**](CertificatesApi.md#certificatesgetcollection) | **GET** /v1/certificates |  |
| [**CertificatesGetInstance**](CertificatesApi.md#certificatesgetinstance) | **GET** /v1/certificates/{id} |  |
| [**CertificatesPassTypeIdGetToOneRelated**](CertificatesApi.md#certificatespasstypeidgettoonerelated) | **GET** /v1/certificates/{id}/passTypeId |  |
| [**CertificatesPassTypeIdGetToOneRelationship**](CertificatesApi.md#certificatespasstypeidgettoonerelationship) | **GET** /v1/certificates/{id}/relationships/passTypeId |  |
| [**CertificatesUpdateInstance**](CertificatesApi.md#certificatesupdateinstance) | **PATCH** /v1/certificates/{id} |  |

<a id="certificatescreateinstance"></a>
# **CertificatesCreateInstance**
> CertificateResponse CertificatesCreateInstance (CertificateCreateRequest certificateCreateRequest)



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
    public class CertificatesCreateInstanceExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var certificateCreateRequest = new CertificateCreateRequest(); // CertificateCreateRequest | Certificate representation

            try
            {
                CertificateResponse result = apiInstance.CertificatesCreateInstance(certificateCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificateResponse> response = apiInstance.CertificatesCreateInstanceWithHttpInfo(certificateCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **certificateCreateRequest** | [**CertificateCreateRequest**](CertificateCreateRequest.md) | Certificate representation |  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **201** | Single Certificate |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="certificatesdeleteinstance"></a>
# **CertificatesDeleteInstance**
> void CertificatesDeleteInstance (string id)



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
    public class CertificatesDeleteInstanceExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.CertificatesDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.CertificatesDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="certificatesgetcollection"></a>
# **CertificatesGetCollection**
> CertificatesResponse CertificatesGetCollection (List<string>? filterDisplayName = null, List<string>? filterCertificateType = null, List<string>? filterSerialNumber = null, List<string>? filterId = null, List<string>? sort = null, List<string>? fieldsCertificates = null, List<string>? fieldsPassTypeIds = null, int? limit = null, List<string>? include = null)



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
    public class CertificatesGetCollectionExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
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
                CertificatesResponse result = apiInstance.CertificatesGetCollection(filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificatesResponse> response = apiInstance.CertificatesGetCollectionWithHttpInfo(filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
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
| **200** | List of Certificates |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="certificatesgetinstance"></a>
# **CertificatesGetInstance**
> CertificateResponse CertificatesGetInstance (string id, List<string>? fieldsCertificates = null, List<string>? fieldsPassTypeIds = null, List<string>? include = null)



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
    public class CertificatesGetInstanceExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var fieldsPassTypeIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type passTypeIds (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                CertificateResponse result = apiInstance.CertificatesGetInstance(id, fieldsCertificates, fieldsPassTypeIds, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificateResponse> response = apiInstance.CertificatesGetInstanceWithHttpInfo(id, fieldsCertificates, fieldsPassTypeIds, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **200** | Single Certificate |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="certificatespasstypeidgettoonerelated"></a>
# **CertificatesPassTypeIdGetToOneRelated**
> PassTypeIdResponse CertificatesPassTypeIdGetToOneRelated (string id, List<string>? fieldsPassTypeIds = null, List<string>? fieldsCertificates = null, List<string>? include = null, int? limitCertificates = null)



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
    public class CertificatesPassTypeIdGetToOneRelatedExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsPassTypeIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type passTypeIds (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCertificates = 56;  // int? | maximum number of related certificates returned (when they are included) (optional) 

            try
            {
                PassTypeIdResponse result = apiInstance.CertificatesPassTypeIdGetToOneRelated(id, fieldsPassTypeIds, fieldsCertificates, include, limitCertificates);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesPassTypeIdGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesPassTypeIdGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdResponse> response = apiInstance.CertificatesPassTypeIdGetToOneRelatedWithHttpInfo(id, fieldsPassTypeIds, fieldsCertificates, include, limitCertificates);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesPassTypeIdGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int?** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **200** | Single PassTypeId |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="certificatespasstypeidgettoonerelationship"></a>
# **CertificatesPassTypeIdGetToOneRelationship**
> CertificatePassTypeIdLinkageResponse CertificatesPassTypeIdGetToOneRelationship (string id)



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
    public class CertificatesPassTypeIdGetToOneRelationshipExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                CertificatePassTypeIdLinkageResponse result = apiInstance.CertificatesPassTypeIdGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesPassTypeIdGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesPassTypeIdGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificatePassTypeIdLinkageResponse> response = apiInstance.CertificatesPassTypeIdGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesPassTypeIdGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**CertificatePassTypeIdLinkageResponse**](CertificatePassTypeIdLinkageResponse.md)

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

<a id="certificatesupdateinstance"></a>
# **CertificatesUpdateInstance**
> CertificateResponse CertificatesUpdateInstance (string id, CertificateUpdateRequest certificateUpdateRequest)



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
    public class CertificatesUpdateInstanceExample
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
            var apiInstance = new CertificatesApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var certificateUpdateRequest = new CertificateUpdateRequest(); // CertificateUpdateRequest | Certificate representation

            try
            {
                CertificateResponse result = apiInstance.CertificatesUpdateInstance(id, certificateUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CertificatesApi.CertificatesUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CertificatesUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificateResponse> response = apiInstance.CertificatesUpdateInstanceWithHttpInfo(id, certificateUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CertificatesApi.CertificatesUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **certificateUpdateRequest** | [**CertificateUpdateRequest**](CertificateUpdateRequest.md) | Certificate representation |  |

### Return type

[**CertificateResponse**](CertificateResponse.md)

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
| **200** | Single Certificate |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

