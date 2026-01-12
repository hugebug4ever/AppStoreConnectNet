# AppStoreConnect.Net.Api.PassTypeIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**PassTypeIdsCertificatesGetToManyRelated**](PassTypeIdsApi.md#passtypeidscertificatesgettomanyrelated) | **GET** /v1/passTypeIds/{id}/certificates |  |
| [**PassTypeIdsCertificatesGetToManyRelationship**](PassTypeIdsApi.md#passtypeidscertificatesgettomanyrelationship) | **GET** /v1/passTypeIds/{id}/relationships/certificates |  |
| [**PassTypeIdsCreateInstance**](PassTypeIdsApi.md#passtypeidscreateinstance) | **POST** /v1/passTypeIds |  |
| [**PassTypeIdsDeleteInstance**](PassTypeIdsApi.md#passtypeidsdeleteinstance) | **DELETE** /v1/passTypeIds/{id} |  |
| [**PassTypeIdsGetCollection**](PassTypeIdsApi.md#passtypeidsgetcollection) | **GET** /v1/passTypeIds |  |
| [**PassTypeIdsGetInstance**](PassTypeIdsApi.md#passtypeidsgetinstance) | **GET** /v1/passTypeIds/{id} |  |
| [**PassTypeIdsUpdateInstance**](PassTypeIdsApi.md#passtypeidsupdateinstance) | **PATCH** /v1/passTypeIds/{id} |  |

<a id="passtypeidscertificatesgettomanyrelated"></a>
# **PassTypeIdsCertificatesGetToManyRelated**
> CertificatesResponse PassTypeIdsCertificatesGetToManyRelated (string id, List<string>? filterDisplayName = null, List<string>? filterCertificateType = null, List<string>? filterSerialNumber = null, List<string>? filterId = null, List<string>? sort = null, List<string>? fieldsCertificates = null, List<string>? fieldsPassTypeIds = null, int? limit = null, List<string>? include = null)



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
    public class PassTypeIdsCertificatesGetToManyRelatedExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
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
                CertificatesResponse result = apiInstance.PassTypeIdsCertificatesGetToManyRelated(id, filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCertificatesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsCertificatesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CertificatesResponse> response = apiInstance.PassTypeIdsCertificatesGetToManyRelatedWithHttpInfo(id, filterDisplayName, filterCertificateType, filterSerialNumber, filterId, sort, fieldsCertificates, fieldsPassTypeIds, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCertificatesGetToManyRelatedWithHttpInfo: " + e.Message);
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

<a id="passtypeidscertificatesgettomanyrelationship"></a>
# **PassTypeIdsCertificatesGetToManyRelationship**
> PassTypeIdCertificatesLinkagesResponse PassTypeIdsCertificatesGetToManyRelationship (string id, int? limit = null)



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
    public class PassTypeIdsCertificatesGetToManyRelationshipExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                PassTypeIdCertificatesLinkagesResponse result = apiInstance.PassTypeIdsCertificatesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCertificatesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsCertificatesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdCertificatesLinkagesResponse> response = apiInstance.PassTypeIdsCertificatesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCertificatesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**PassTypeIdCertificatesLinkagesResponse**](PassTypeIdCertificatesLinkagesResponse.md)

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

<a id="passtypeidscreateinstance"></a>
# **PassTypeIdsCreateInstance**
> PassTypeIdResponse PassTypeIdsCreateInstance (PassTypeIdCreateRequest passTypeIdCreateRequest)



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
    public class PassTypeIdsCreateInstanceExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var passTypeIdCreateRequest = new PassTypeIdCreateRequest(); // PassTypeIdCreateRequest | PassTypeId representation

            try
            {
                PassTypeIdResponse result = apiInstance.PassTypeIdsCreateInstance(passTypeIdCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdResponse> response = apiInstance.PassTypeIdsCreateInstanceWithHttpInfo(passTypeIdCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **passTypeIdCreateRequest** | [**PassTypeIdCreateRequest**](PassTypeIdCreateRequest.md) | PassTypeId representation |  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **201** | Single PassTypeId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="passtypeidsdeleteinstance"></a>
# **PassTypeIdsDeleteInstance**
> void PassTypeIdsDeleteInstance (string id)



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
    public class PassTypeIdsDeleteInstanceExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.PassTypeIdsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.PassTypeIdsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="passtypeidsgetcollection"></a>
# **PassTypeIdsGetCollection**
> PassTypeIdsResponse PassTypeIdsGetCollection (List<string>? filterName = null, List<string>? filterIdentifier = null, List<string>? filterId = null, List<string>? sort = null, List<string>? fieldsPassTypeIds = null, List<string>? fieldsCertificates = null, int? limit = null, List<string>? include = null, int? limitCertificates = null)



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
    public class PassTypeIdsGetCollectionExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var filterName = new List<string>?(); // List<string>? | filter by attribute 'name' (optional) 
            var filterIdentifier = new List<string>?(); // List<string>? | filter by attribute 'identifier' (optional) 
            var filterId = new List<string>?(); // List<string>? | filter by id(s) (optional) 
            var sort = new List<string>?(); // List<string>? | comma-separated list of sort expressions; resources will be sorted as specified (optional) 
            var fieldsPassTypeIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type passTypeIds (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCertificates = 56;  // int? | maximum number of related certificates returned (when they are included) (optional) 

            try
            {
                PassTypeIdsResponse result = apiInstance.PassTypeIdsGetCollection(filterName, filterIdentifier, filterId, sort, fieldsPassTypeIds, fieldsCertificates, limit, include, limitCertificates);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsGetCollection: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsGetCollectionWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdsResponse> response = apiInstance.PassTypeIdsGetCollectionWithHttpInfo(filterName, filterIdentifier, filterId, sort, fieldsPassTypeIds, fieldsCertificates, limit, include, limitCertificates);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsGetCollectionWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIdentifier** | [**List&lt;string&gt;?**](string.md) | filter by attribute &#39;identifier&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;?**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;?**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsPassTypeIds** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type passTypeIds | [optional]  |
| **fieldsCertificates** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type certificates | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCertificates** | **int?** | maximum number of related certificates returned (when they are included) | [optional]  |

### Return type

[**PassTypeIdsResponse**](PassTypeIdsResponse.md)

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
| **200** | List of PassTypeIds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="passtypeidsgetinstance"></a>
# **PassTypeIdsGetInstance**
> PassTypeIdResponse PassTypeIdsGetInstance (string id, List<string>? fieldsPassTypeIds = null, List<string>? fieldsCertificates = null, List<string>? include = null, int? limitCertificates = null)



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
    public class PassTypeIdsGetInstanceExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsPassTypeIds = new List<string>?(); // List<string>? | the fields to include for returned resources of type passTypeIds (optional) 
            var fieldsCertificates = new List<string>?(); // List<string>? | the fields to include for returned resources of type certificates (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitCertificates = 56;  // int? | maximum number of related certificates returned (when they are included) (optional) 

            try
            {
                PassTypeIdResponse result = apiInstance.PassTypeIdsGetInstance(id, fieldsPassTypeIds, fieldsCertificates, include, limitCertificates);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdResponse> response = apiInstance.PassTypeIdsGetInstanceWithHttpInfo(id, fieldsPassTypeIds, fieldsCertificates, include, limitCertificates);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsGetInstanceWithHttpInfo: " + e.Message);
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

<a id="passtypeidsupdateinstance"></a>
# **PassTypeIdsUpdateInstance**
> PassTypeIdResponse PassTypeIdsUpdateInstance (string id, PassTypeIdUpdateRequest passTypeIdUpdateRequest)



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
    public class PassTypeIdsUpdateInstanceExample
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
            var apiInstance = new PassTypeIdsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var passTypeIdUpdateRequest = new PassTypeIdUpdateRequest(); // PassTypeIdUpdateRequest | PassTypeId representation

            try
            {
                PassTypeIdResponse result = apiInstance.PassTypeIdsUpdateInstance(id, passTypeIdUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the PassTypeIdsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PassTypeIdResponse> response = apiInstance.PassTypeIdsUpdateInstanceWithHttpInfo(id, passTypeIdUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling PassTypeIdsApi.PassTypeIdsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **passTypeIdUpdateRequest** | [**PassTypeIdUpdateRequest**](PassTypeIdUpdateRequest.md) | PassTypeId representation |  |

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
| **200** | Single PassTypeId |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

