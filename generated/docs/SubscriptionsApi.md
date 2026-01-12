# AppStoreConnect.Net.Api.SubscriptionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SubscriptionsAppStoreReviewScreenshotGetToOneRelated**](SubscriptionsApi.md#subscriptionsappstorereviewscreenshotgettoonerelated) | **GET** /v1/subscriptions/{id}/appStoreReviewScreenshot |  |
| [**SubscriptionsAppStoreReviewScreenshotGetToOneRelationship**](SubscriptionsApi.md#subscriptionsappstorereviewscreenshotgettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/appStoreReviewScreenshot |  |
| [**SubscriptionsCreateInstance**](SubscriptionsApi.md#subscriptionscreateinstance) | **POST** /v1/subscriptions |  |
| [**SubscriptionsDeleteInstance**](SubscriptionsApi.md#subscriptionsdeleteinstance) | **DELETE** /v1/subscriptions/{id} |  |
| [**SubscriptionsGetInstance**](SubscriptionsApi.md#subscriptionsgetinstance) | **GET** /v1/subscriptions/{id} |  |
| [**SubscriptionsImagesGetToManyRelated**](SubscriptionsApi.md#subscriptionsimagesgettomanyrelated) | **GET** /v1/subscriptions/{id}/images |  |
| [**SubscriptionsImagesGetToManyRelationship**](SubscriptionsApi.md#subscriptionsimagesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/images |  |
| [**SubscriptionsIntroductoryOffersDeleteToManyRelationship**](SubscriptionsApi.md#subscriptionsintroductoryoffersdeletetomanyrelationship) | **DELETE** /v1/subscriptions/{id}/relationships/introductoryOffers |  |
| [**SubscriptionsIntroductoryOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionsintroductoryoffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/introductoryOffers |  |
| [**SubscriptionsIntroductoryOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionsintroductoryoffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/introductoryOffers |  |
| [**SubscriptionsOfferCodesGetToManyRelated**](SubscriptionsApi.md#subscriptionsoffercodesgettomanyrelated) | **GET** /v1/subscriptions/{id}/offerCodes |  |
| [**SubscriptionsOfferCodesGetToManyRelationship**](SubscriptionsApi.md#subscriptionsoffercodesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/offerCodes |  |
| [**SubscriptionsPricePointsGetToManyRelated**](SubscriptionsApi.md#subscriptionspricepointsgettomanyrelated) | **GET** /v1/subscriptions/{id}/pricePoints |  |
| [**SubscriptionsPricePointsGetToManyRelationship**](SubscriptionsApi.md#subscriptionspricepointsgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/pricePoints |  |
| [**SubscriptionsPricesDeleteToManyRelationship**](SubscriptionsApi.md#subscriptionspricesdeletetomanyrelationship) | **DELETE** /v1/subscriptions/{id}/relationships/prices |  |
| [**SubscriptionsPricesGetToManyRelated**](SubscriptionsApi.md#subscriptionspricesgettomanyrelated) | **GET** /v1/subscriptions/{id}/prices |  |
| [**SubscriptionsPricesGetToManyRelationship**](SubscriptionsApi.md#subscriptionspricesgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/prices |  |
| [**SubscriptionsPromotedPurchaseGetToOneRelated**](SubscriptionsApi.md#subscriptionspromotedpurchasegettoonerelated) | **GET** /v1/subscriptions/{id}/promotedPurchase |  |
| [**SubscriptionsPromotedPurchaseGetToOneRelationship**](SubscriptionsApi.md#subscriptionspromotedpurchasegettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/promotedPurchase |  |
| [**SubscriptionsPromotionalOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionspromotionaloffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/promotionalOffers |  |
| [**SubscriptionsPromotionalOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionspromotionaloffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/promotionalOffers |  |
| [**SubscriptionsSubscriptionAvailabilityGetToOneRelated**](SubscriptionsApi.md#subscriptionssubscriptionavailabilitygettoonerelated) | **GET** /v1/subscriptions/{id}/subscriptionAvailability |  |
| [**SubscriptionsSubscriptionAvailabilityGetToOneRelationship**](SubscriptionsApi.md#subscriptionssubscriptionavailabilitygettoonerelationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionAvailability |  |
| [**SubscriptionsSubscriptionLocalizationsGetToManyRelated**](SubscriptionsApi.md#subscriptionssubscriptionlocalizationsgettomanyrelated) | **GET** /v1/subscriptions/{id}/subscriptionLocalizations |  |
| [**SubscriptionsSubscriptionLocalizationsGetToManyRelationship**](SubscriptionsApi.md#subscriptionssubscriptionlocalizationsgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionLocalizations |  |
| [**SubscriptionsUpdateInstance**](SubscriptionsApi.md#subscriptionsupdateinstance) | **PATCH** /v1/subscriptions/{id} |  |
| [**SubscriptionsWinBackOffersGetToManyRelated**](SubscriptionsApi.md#subscriptionswinbackoffersgettomanyrelated) | **GET** /v1/subscriptions/{id}/winBackOffers |  |
| [**SubscriptionsWinBackOffersGetToManyRelationship**](SubscriptionsApi.md#subscriptionswinbackoffersgettomanyrelationship) | **GET** /v1/subscriptions/{id}/relationships/winBackOffers |  |

<a id="subscriptionsappstorereviewscreenshotgettoonerelated"></a>
# **SubscriptionsAppStoreReviewScreenshotGetToOneRelated**
> SubscriptionAppStoreReviewScreenshotResponse SubscriptionsAppStoreReviewScreenshotGetToOneRelated (string id, List<string>? fieldsSubscriptionAppStoreReviewScreenshots = null, List<string>? fieldsSubscriptions = null, List<string>? include = null)



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
    public class SubscriptionsAppStoreReviewScreenshotGetToOneRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionAppStoreReviewScreenshots = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionAppStoreReviewScreenshotResponse result = apiInstance.SubscriptionsAppStoreReviewScreenshotGetToOneRelated(id, fieldsSubscriptionAppStoreReviewScreenshots, fieldsSubscriptions, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsAppStoreReviewScreenshotGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsAppStoreReviewScreenshotGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAppStoreReviewScreenshotResponse> response = apiInstance.SubscriptionsAppStoreReviewScreenshotGetToOneRelatedWithHttpInfo(id, fieldsSubscriptionAppStoreReviewScreenshots, fieldsSubscriptions, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsAppStoreReviewScreenshotGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionAppStoreReviewScreenshots** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionAppStoreReviewScreenshotResponse**](SubscriptionAppStoreReviewScreenshotResponse.md)

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
| **200** | Single SubscriptionAppStoreReviewScreenshot |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsappstorereviewscreenshotgettoonerelationship"></a>
# **SubscriptionsAppStoreReviewScreenshotGetToOneRelationship**
> SubscriptionAppStoreReviewScreenshotLinkageResponse SubscriptionsAppStoreReviewScreenshotGetToOneRelationship (string id)



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
    public class SubscriptionsAppStoreReviewScreenshotGetToOneRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                SubscriptionAppStoreReviewScreenshotLinkageResponse result = apiInstance.SubscriptionsAppStoreReviewScreenshotGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsAppStoreReviewScreenshotGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsAppStoreReviewScreenshotGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAppStoreReviewScreenshotLinkageResponse> response = apiInstance.SubscriptionsAppStoreReviewScreenshotGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsAppStoreReviewScreenshotGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionAppStoreReviewScreenshotLinkageResponse**](SubscriptionAppStoreReviewScreenshotLinkageResponse.md)

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

<a id="subscriptionscreateinstance"></a>
# **SubscriptionsCreateInstance**
> SubscriptionResponse SubscriptionsCreateInstance (SubscriptionCreateRequest subscriptionCreateRequest)



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
    public class SubscriptionsCreateInstanceExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var subscriptionCreateRequest = new SubscriptionCreateRequest(); // SubscriptionCreateRequest | Subscription representation

            try
            {
                SubscriptionResponse result = apiInstance.SubscriptionsCreateInstance(subscriptionCreateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsCreateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsCreateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionResponse> response = apiInstance.SubscriptionsCreateInstanceWithHttpInfo(subscriptionCreateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsCreateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **subscriptionCreateRequest** | [**SubscriptionCreateRequest**](SubscriptionCreateRequest.md) | Subscription representation |  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **201** | Single Subscription |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsdeleteinstance"></a>
# **SubscriptionsDeleteInstance**
> void SubscriptionsDeleteInstance (string id)



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
    public class SubscriptionsDeleteInstanceExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                apiInstance.SubscriptionsDeleteInstance(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsDeleteInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsDeleteInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.SubscriptionsDeleteInstanceWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsDeleteInstanceWithHttpInfo: " + e.Message);
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

<a id="subscriptionsgetinstance"></a>
# **SubscriptionsGetInstance**
> SubscriptionResponse SubscriptionsGetInstance (string id, List<string>? fieldsSubscriptions = null, List<string>? fieldsSubscriptionLocalizations = null, List<string>? fieldsSubscriptionAppStoreReviewScreenshots = null, List<string>? fieldsSubscriptionIntroductoryOffers = null, List<string>? fieldsSubscriptionPromotionalOffers = null, List<string>? fieldsSubscriptionOfferCodes = null, List<string>? fieldsSubscriptionPrices = null, List<string>? fieldsPromotedPurchases = null, List<string>? fieldsSubscriptionAvailabilities = null, List<string>? fieldsWinBackOffers = null, List<string>? fieldsSubscriptionImages = null, List<string>? include = null, int? limitImages = null, int? limitIntroductoryOffers = null, int? limitOfferCodes = null, int? limitPrices = null, int? limitPromotionalOffers = null, int? limitSubscriptionLocalizations = null, int? limitWinBackOffers = null)



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
    public class SubscriptionsGetInstanceExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var fieldsSubscriptionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionLocalizations (optional) 
            var fieldsSubscriptionAppStoreReviewScreenshots = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots (optional) 
            var fieldsSubscriptionIntroductoryOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionIntroductoryOffers (optional) 
            var fieldsSubscriptionPromotionalOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOffers (optional) 
            var fieldsSubscriptionOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodes (optional) 
            var fieldsSubscriptionPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPrices (optional) 
            var fieldsPromotedPurchases = new List<string>?(); // List<string>? | the fields to include for returned resources of type promotedPurchases (optional) 
            var fieldsSubscriptionAvailabilities = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionAvailabilities (optional) 
            var fieldsWinBackOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOffers (optional) 
            var fieldsSubscriptionImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionImages (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitImages = 56;  // int? | maximum number of related images returned (when they are included) (optional) 
            var limitIntroductoryOffers = 56;  // int? | maximum number of related introductoryOffers returned (when they are included) (optional) 
            var limitOfferCodes = 56;  // int? | maximum number of related offerCodes returned (when they are included) (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 
            var limitPromotionalOffers = 56;  // int? | maximum number of related promotionalOffers returned (when they are included) (optional) 
            var limitSubscriptionLocalizations = 56;  // int? | maximum number of related subscriptionLocalizations returned (when they are included) (optional) 
            var limitWinBackOffers = 56;  // int? | maximum number of related winBackOffers returned (when they are included) (optional) 

            try
            {
                SubscriptionResponse result = apiInstance.SubscriptionsGetInstance(id, fieldsSubscriptions, fieldsSubscriptionLocalizations, fieldsSubscriptionAppStoreReviewScreenshots, fieldsSubscriptionIntroductoryOffers, fieldsSubscriptionPromotionalOffers, fieldsSubscriptionOfferCodes, fieldsSubscriptionPrices, fieldsPromotedPurchases, fieldsSubscriptionAvailabilities, fieldsWinBackOffers, fieldsSubscriptionImages, include, limitImages, limitIntroductoryOffers, limitOfferCodes, limitPrices, limitPromotionalOffers, limitSubscriptionLocalizations, limitWinBackOffers);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsGetInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsGetInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionResponse> response = apiInstance.SubscriptionsGetInstanceWithHttpInfo(id, fieldsSubscriptions, fieldsSubscriptionLocalizations, fieldsSubscriptionAppStoreReviewScreenshots, fieldsSubscriptionIntroductoryOffers, fieldsSubscriptionPromotionalOffers, fieldsSubscriptionOfferCodes, fieldsSubscriptionPrices, fieldsPromotedPurchases, fieldsSubscriptionAvailabilities, fieldsWinBackOffers, fieldsSubscriptionImages, include, limitImages, limitIntroductoryOffers, limitOfferCodes, limitPrices, limitPromotionalOffers, limitSubscriptionLocalizations, limitWinBackOffers);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsGetInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionLocalizations | [optional]  |
| **fieldsSubscriptionAppStoreReviewScreenshots** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional]  |
| **fieldsSubscriptionIntroductoryOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional]  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptionPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPrices | [optional]  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsSubscriptionAvailabilities** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionAvailabilities | [optional]  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitImages** | **int?** | maximum number of related images returned (when they are included) | [optional]  |
| **limitIntroductoryOffers** | **int?** | maximum number of related introductoryOffers returned (when they are included) | [optional]  |
| **limitOfferCodes** | **int?** | maximum number of related offerCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |
| **limitPromotionalOffers** | **int?** | maximum number of related promotionalOffers returned (when they are included) | [optional]  |
| **limitSubscriptionLocalizations** | **int?** | maximum number of related subscriptionLocalizations returned (when they are included) | [optional]  |
| **limitWinBackOffers** | **int?** | maximum number of related winBackOffers returned (when they are included) | [optional]  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **200** | Single Subscription |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsimagesgettomanyrelated"></a>
# **SubscriptionsImagesGetToManyRelated**
> SubscriptionImagesResponse SubscriptionsImagesGetToManyRelated (string id, List<string>? fieldsSubscriptionImages = null, List<string>? fieldsSubscriptions = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionsImagesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionImages = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionImages (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionImagesResponse result = apiInstance.SubscriptionsImagesGetToManyRelated(id, fieldsSubscriptionImages, fieldsSubscriptions, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsImagesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsImagesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionImagesResponse> response = apiInstance.SubscriptionsImagesGetToManyRelatedWithHttpInfo(id, fieldsSubscriptionImages, fieldsSubscriptions, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsImagesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionImages** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionImages | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionImagesResponse**](SubscriptionImagesResponse.md)

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
| **200** | List of SubscriptionImages |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsimagesgettomanyrelationship"></a>
# **SubscriptionsImagesGetToManyRelationship**
> SubscriptionImagesLinkagesResponse SubscriptionsImagesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsImagesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionImagesLinkagesResponse result = apiInstance.SubscriptionsImagesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsImagesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsImagesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionImagesLinkagesResponse> response = apiInstance.SubscriptionsImagesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsImagesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionImagesLinkagesResponse**](SubscriptionImagesLinkagesResponse.md)

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

<a id="subscriptionsintroductoryoffersdeletetomanyrelationship"></a>
# **SubscriptionsIntroductoryOffersDeleteToManyRelationship**
> void SubscriptionsIntroductoryOffersDeleteToManyRelationship (string id, SubscriptionIntroductoryOffersLinkagesRequest subscriptionIntroductoryOffersLinkagesRequest)



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
    public class SubscriptionsIntroductoryOffersDeleteToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var subscriptionIntroductoryOffersLinkagesRequest = new SubscriptionIntroductoryOffersLinkagesRequest(); // SubscriptionIntroductoryOffersLinkagesRequest | List of related linkages

            try
            {
                apiInstance.SubscriptionsIntroductoryOffersDeleteToManyRelationship(id, subscriptionIntroductoryOffersLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsIntroductoryOffersDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.SubscriptionsIntroductoryOffersDeleteToManyRelationshipWithHttpInfo(id, subscriptionIntroductoryOffersLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionIntroductoryOffersLinkagesRequest** | [**SubscriptionIntroductoryOffersLinkagesRequest**](SubscriptionIntroductoryOffersLinkagesRequest.md) | List of related linkages |  |

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

<a id="subscriptionsintroductoryoffersgettomanyrelated"></a>
# **SubscriptionsIntroductoryOffersGetToManyRelated**
> SubscriptionIntroductoryOffersResponse SubscriptionsIntroductoryOffersGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionIntroductoryOffers = null, List<string>? fieldsSubscriptions = null, List<string>? fieldsTerritories = null, List<string>? fieldsSubscriptionPricePoints = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionsIntroductoryOffersGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsSubscriptionIntroductoryOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionIntroductoryOffers (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionIntroductoryOffersResponse result = apiInstance.SubscriptionsIntroductoryOffersGetToManyRelated(id, filterTerritory, fieldsSubscriptionIntroductoryOffers, fieldsSubscriptions, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsIntroductoryOffersGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionIntroductoryOffersResponse> response = apiInstance.SubscriptionsIntroductoryOffersGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionIntroductoryOffers, fieldsSubscriptions, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionIntroductoryOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionIntroductoryOffersResponse**](SubscriptionIntroductoryOffersResponse.md)

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
| **200** | List of SubscriptionIntroductoryOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsintroductoryoffersgettomanyrelationship"></a>
# **SubscriptionsIntroductoryOffersGetToManyRelationship**
> SubscriptionIntroductoryOffersLinkagesResponse SubscriptionsIntroductoryOffersGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsIntroductoryOffersGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionIntroductoryOffersLinkagesResponse result = apiInstance.SubscriptionsIntroductoryOffersGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsIntroductoryOffersGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionIntroductoryOffersLinkagesResponse> response = apiInstance.SubscriptionsIntroductoryOffersGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsIntroductoryOffersGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionIntroductoryOffersLinkagesResponse**](SubscriptionIntroductoryOffersLinkagesResponse.md)

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

<a id="subscriptionsoffercodesgettomanyrelated"></a>
# **SubscriptionsOfferCodesGetToManyRelated**
> SubscriptionOfferCodesResponse SubscriptionsOfferCodesGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionOfferCodes = null, List<string>? fieldsSubscriptions = null, List<string>? fieldsSubscriptionOfferCodeOneTimeUseCodes = null, List<string>? fieldsSubscriptionOfferCodeCustomCodes = null, List<string>? fieldsSubscriptionOfferCodePrices = null, int? limit = null, List<string>? include = null, int? limitOneTimeUseCodes = null, int? limitCustomCodes = null, int? limitPrices = null)



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
    public class SubscriptionsOfferCodesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by territory (optional) 
            var fieldsSubscriptionOfferCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodes (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var fieldsSubscriptionOfferCodeOneTimeUseCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional) 
            var fieldsSubscriptionOfferCodeCustomCodes = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional) 
            var fieldsSubscriptionOfferCodePrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionOfferCodePrices (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitOneTimeUseCodes = 56;  // int? | maximum number of related oneTimeUseCodes returned (when they are included) (optional) 
            var limitCustomCodes = 56;  // int? | maximum number of related customCodes returned (when they are included) (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                SubscriptionOfferCodesResponse result = apiInstance.SubscriptionsOfferCodesGetToManyRelated(id, filterTerritory, fieldsSubscriptionOfferCodes, fieldsSubscriptions, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodePrices, limit, include, limitOneTimeUseCodes, limitCustomCodes, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsOfferCodesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsOfferCodesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodesResponse> response = apiInstance.SubscriptionsOfferCodesGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionOfferCodes, fieldsSubscriptions, fieldsSubscriptionOfferCodeOneTimeUseCodes, fieldsSubscriptionOfferCodeCustomCodes, fieldsSubscriptionOfferCodePrices, limit, include, limitOneTimeUseCodes, limitCustomCodes, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsOfferCodesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by territory | [optional]  |
| **fieldsSubscriptionOfferCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodes | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionOfferCodeOneTimeUseCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional]  |
| **fieldsSubscriptionOfferCodeCustomCodes** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional]  |
| **fieldsSubscriptionOfferCodePrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionOfferCodePrices | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitOneTimeUseCodes** | **int?** | maximum number of related oneTimeUseCodes returned (when they are included) | [optional]  |
| **limitCustomCodes** | **int?** | maximum number of related customCodes returned (when they are included) | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionOfferCodesResponse**](SubscriptionOfferCodesResponse.md)

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
| **200** | List of SubscriptionOfferCodes |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionsoffercodesgettomanyrelationship"></a>
# **SubscriptionsOfferCodesGetToManyRelationship**
> SubscriptionOfferCodesLinkagesResponse SubscriptionsOfferCodesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsOfferCodesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionOfferCodesLinkagesResponse result = apiInstance.SubscriptionsOfferCodesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsOfferCodesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsOfferCodesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionOfferCodesLinkagesResponse> response = apiInstance.SubscriptionsOfferCodesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsOfferCodesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionOfferCodesLinkagesResponse**](SubscriptionOfferCodesLinkagesResponse.md)

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

<a id="subscriptionspricepointsgettomanyrelated"></a>
# **SubscriptionsPricePointsGetToManyRelated**
> SubscriptionPricePointsResponse SubscriptionsPricePointsGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionPricePoints = null, List<string>? fieldsTerritories = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionsPricePointsGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionPricePointsResponse result = apiInstance.SubscriptionsPricePointsGetToManyRelated(id, filterTerritory, fieldsSubscriptionPricePoints, fieldsTerritories, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricePointsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPricePointsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPricePointsResponse> response = apiInstance.SubscriptionsPricePointsGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionPricePoints, fieldsTerritories, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricePointsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricePointsResponse**](SubscriptionPricePointsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of SubscriptionPricePoints |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionspricepointsgettomanyrelationship"></a>
# **SubscriptionsPricePointsGetToManyRelationship**
> SubscriptionPricePointsLinkagesResponse SubscriptionsPricePointsGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsPricePointsGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionPricePointsLinkagesResponse result = apiInstance.SubscriptionsPricePointsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricePointsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPricePointsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPricePointsLinkagesResponse> response = apiInstance.SubscriptionsPricePointsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricePointsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionPricePointsLinkagesResponse**](SubscriptionPricePointsLinkagesResponse.md)

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

<a id="subscriptionspricesdeletetomanyrelationship"></a>
# **SubscriptionsPricesDeleteToManyRelationship**
> void SubscriptionsPricesDeleteToManyRelationship (string id, SubscriptionPricesLinkagesRequest subscriptionPricesLinkagesRequest)



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
    public class SubscriptionsPricesDeleteToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var subscriptionPricesLinkagesRequest = new SubscriptionPricesLinkagesRequest(); // SubscriptionPricesLinkagesRequest | List of related linkages

            try
            {
                apiInstance.SubscriptionsPricesDeleteToManyRelationship(id, subscriptionPricesLinkagesRequest);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesDeleteToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPricesDeleteToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.SubscriptionsPricesDeleteToManyRelationshipWithHttpInfo(id, subscriptionPricesLinkagesRequest);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesDeleteToManyRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionPricesLinkagesRequest** | [**SubscriptionPricesLinkagesRequest**](SubscriptionPricesLinkagesRequest.md) | List of related linkages |  |

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

<a id="subscriptionspricesgettomanyrelated"></a>
# **SubscriptionsPricesGetToManyRelated**
> SubscriptionPricesResponse SubscriptionsPricesGetToManyRelated (string id, List<string>? filterSubscriptionPricePoint = null, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionPrices = null, List<string>? fieldsTerritories = null, List<string>? fieldsSubscriptionPricePoints = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionsPricesGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterSubscriptionPricePoint = new List<string>?(); // List<string>? | filter by id(s) of related 'subscriptionPricePoint' (optional) 
            var filterTerritory = new List<string>?(); // List<string>? | filter by id(s) of related 'territory' (optional) 
            var fieldsSubscriptionPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPrices (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var fieldsSubscriptionPricePoints = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPricePoints (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionPricesResponse result = apiInstance.SubscriptionsPricesGetToManyRelated(id, filterSubscriptionPricePoint, filterTerritory, fieldsSubscriptionPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPricesGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPricesResponse> response = apiInstance.SubscriptionsPricesGetToManyRelatedWithHttpInfo(id, filterSubscriptionPricePoint, filterTerritory, fieldsSubscriptionPrices, fieldsTerritories, fieldsSubscriptionPricePoints, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterSubscriptionPricePoint** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;subscriptionPricePoint&#39; | [optional]  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by id(s) of related &#39;territory&#39; | [optional]  |
| **fieldsSubscriptionPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPrices | [optional]  |
| **fieldsTerritories** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type territories | [optional]  |
| **fieldsSubscriptionPricePoints** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPricePoints | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionPricesResponse**](SubscriptionPricesResponse.md)

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
| **200** | List of SubscriptionPrices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionspricesgettomanyrelationship"></a>
# **SubscriptionsPricesGetToManyRelationship**
> SubscriptionPricesLinkagesResponse SubscriptionsPricesGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsPricesGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionPricesLinkagesResponse result = apiInstance.SubscriptionsPricesGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPricesGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPricesLinkagesResponse> response = apiInstance.SubscriptionsPricesGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPricesGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionPricesLinkagesResponse**](SubscriptionPricesLinkagesResponse.md)

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

<a id="subscriptionspromotedpurchasegettoonerelated"></a>
# **SubscriptionsPromotedPurchaseGetToOneRelated**
> PromotedPurchaseResponse SubscriptionsPromotedPurchaseGetToOneRelated (string id, List<string>? fieldsPromotedPurchases = null, List<string>? fieldsInAppPurchases = null, List<string>? fieldsSubscriptions = null, List<string>? include = null)



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
    public class SubscriptionsPromotedPurchaseGetToOneRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsPromotedPurchases = new List<string>?(); // List<string>? | the fields to include for returned resources of type promotedPurchases (optional) 
            var fieldsInAppPurchases = new List<string>?(); // List<string>? | the fields to include for returned resources of type inAppPurchases (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                PromotedPurchaseResponse result = apiInstance.SubscriptionsPromotedPurchaseGetToOneRelated(id, fieldsPromotedPurchases, fieldsInAppPurchases, fieldsSubscriptions, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotedPurchaseGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPromotedPurchaseGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<PromotedPurchaseResponse> response = apiInstance.SubscriptionsPromotedPurchaseGetToOneRelatedWithHttpInfo(id, fieldsPromotedPurchases, fieldsInAppPurchases, fieldsSubscriptions, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotedPurchaseGetToOneRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPromotedPurchases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type promotedPurchases | [optional]  |
| **fieldsInAppPurchases** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type inAppPurchases | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**PromotedPurchaseResponse**](PromotedPurchaseResponse.md)

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
| **200** | Single PromotedPurchase |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionspromotedpurchasegettoonerelationship"></a>
# **SubscriptionsPromotedPurchaseGetToOneRelationship**
> SubscriptionPromotedPurchaseLinkageResponse SubscriptionsPromotedPurchaseGetToOneRelationship (string id)



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
    public class SubscriptionsPromotedPurchaseGetToOneRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                SubscriptionPromotedPurchaseLinkageResponse result = apiInstance.SubscriptionsPromotedPurchaseGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotedPurchaseGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPromotedPurchaseGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotedPurchaseLinkageResponse> response = apiInstance.SubscriptionsPromotedPurchaseGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotedPurchaseGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionPromotedPurchaseLinkageResponse**](SubscriptionPromotedPurchaseLinkageResponse.md)

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

<a id="subscriptionspromotionaloffersgettomanyrelated"></a>
# **SubscriptionsPromotionalOffersGetToManyRelated**
> SubscriptionPromotionalOffersResponse SubscriptionsPromotionalOffersGetToManyRelated (string id, List<string>? filterTerritory = null, List<string>? fieldsSubscriptionPromotionalOffers = null, List<string>? fieldsSubscriptions = null, List<string>? fieldsSubscriptionPromotionalOfferPrices = null, int? limit = null, List<string>? include = null, int? limitPrices = null)



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
    public class SubscriptionsPromotionalOffersGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var filterTerritory = new List<string>?(); // List<string>? | filter by territory (optional) 
            var fieldsSubscriptionPromotionalOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOffers (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var fieldsSubscriptionPromotionalOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionPromotionalOfferPrices (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                SubscriptionPromotionalOffersResponse result = apiInstance.SubscriptionsPromotionalOffersGetToManyRelated(id, filterTerritory, fieldsSubscriptionPromotionalOffers, fieldsSubscriptions, fieldsSubscriptionPromotionalOfferPrices, limit, include, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotionalOffersGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPromotionalOffersGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOffersResponse> response = apiInstance.SubscriptionsPromotionalOffersGetToManyRelatedWithHttpInfo(id, filterTerritory, fieldsSubscriptionPromotionalOffers, fieldsSubscriptions, fieldsSubscriptionPromotionalOfferPrices, limit, include, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotionalOffersGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterTerritory** | [**List&lt;string&gt;?**](string.md) | filter by territory | [optional]  |
| **fieldsSubscriptionPromotionalOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOffers | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **fieldsSubscriptionPromotionalOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**SubscriptionPromotionalOffersResponse**](SubscriptionPromotionalOffersResponse.md)

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
| **200** | List of SubscriptionPromotionalOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionspromotionaloffersgettomanyrelationship"></a>
# **SubscriptionsPromotionalOffersGetToManyRelationship**
> SubscriptionPromotionalOffersLinkagesResponse SubscriptionsPromotionalOffersGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsPromotionalOffersGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionPromotionalOffersLinkagesResponse result = apiInstance.SubscriptionsPromotionalOffersGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotionalOffersGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsPromotionalOffersGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionPromotionalOffersLinkagesResponse> response = apiInstance.SubscriptionsPromotionalOffersGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsPromotionalOffersGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionPromotionalOffersLinkagesResponse**](SubscriptionPromotionalOffersLinkagesResponse.md)

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

<a id="subscriptionssubscriptionavailabilitygettoonerelated"></a>
# **SubscriptionsSubscriptionAvailabilityGetToOneRelated**
> SubscriptionAvailabilityResponse SubscriptionsSubscriptionAvailabilityGetToOneRelated (string id, List<string>? fieldsSubscriptionAvailabilities = null, List<string>? fieldsTerritories = null, List<string>? include = null, int? limitAvailableTerritories = null)



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
    public class SubscriptionsSubscriptionAvailabilityGetToOneRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionAvailabilities = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionAvailabilities (optional) 
            var fieldsTerritories = new List<string>?(); // List<string>? | the fields to include for returned resources of type territories (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitAvailableTerritories = 56;  // int? | maximum number of related availableTerritories returned (when they are included) (optional) 

            try
            {
                SubscriptionAvailabilityResponse result = apiInstance.SubscriptionsSubscriptionAvailabilityGetToOneRelated(id, fieldsSubscriptionAvailabilities, fieldsTerritories, include, limitAvailableTerritories);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionAvailabilityGetToOneRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsSubscriptionAvailabilityGetToOneRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionAvailabilityResponse> response = apiInstance.SubscriptionsSubscriptionAvailabilityGetToOneRelatedWithHttpInfo(id, fieldsSubscriptionAvailabilities, fieldsTerritories, include, limitAvailableTerritories);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionAvailabilityGetToOneRelatedWithHttpInfo: " + e.Message);
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

<a id="subscriptionssubscriptionavailabilitygettoonerelationship"></a>
# **SubscriptionsSubscriptionAvailabilityGetToOneRelationship**
> SubscriptionSubscriptionAvailabilityLinkageResponse SubscriptionsSubscriptionAvailabilityGetToOneRelationship (string id)



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
    public class SubscriptionsSubscriptionAvailabilityGetToOneRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource

            try
            {
                SubscriptionSubscriptionAvailabilityLinkageResponse result = apiInstance.SubscriptionsSubscriptionAvailabilityGetToOneRelationship(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionAvailabilityGetToOneRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsSubscriptionAvailabilityGetToOneRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionSubscriptionAvailabilityLinkageResponse> response = apiInstance.SubscriptionsSubscriptionAvailabilityGetToOneRelationshipWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionAvailabilityGetToOneRelationshipWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**SubscriptionSubscriptionAvailabilityLinkageResponse**](SubscriptionSubscriptionAvailabilityLinkageResponse.md)

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

<a id="subscriptionssubscriptionlocalizationsgettomanyrelated"></a>
# **SubscriptionsSubscriptionLocalizationsGetToManyRelated**
> SubscriptionLocalizationsResponse SubscriptionsSubscriptionLocalizationsGetToManyRelated (string id, List<string>? fieldsSubscriptionLocalizations = null, List<string>? fieldsSubscriptions = null, int? limit = null, List<string>? include = null)



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
    public class SubscriptionsSubscriptionLocalizationsGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsSubscriptionLocalizations = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptionLocalizations (optional) 
            var fieldsSubscriptions = new List<string>?(); // List<string>? | the fields to include for returned resources of type subscriptions (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 

            try
            {
                SubscriptionLocalizationsResponse result = apiInstance.SubscriptionsSubscriptionLocalizationsGetToManyRelated(id, fieldsSubscriptionLocalizations, fieldsSubscriptions, limit, include);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionLocalizationsGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsSubscriptionLocalizationsGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionLocalizationsResponse> response = apiInstance.SubscriptionsSubscriptionLocalizationsGetToManyRelatedWithHttpInfo(id, fieldsSubscriptionLocalizations, fieldsSubscriptions, limit, include);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionLocalizationsGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsSubscriptionLocalizations** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptionLocalizations | [optional]  |
| **fieldsSubscriptions** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type subscriptions | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**SubscriptionLocalizationsResponse**](SubscriptionLocalizationsResponse.md)

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
| **200** | List of SubscriptionLocalizations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionssubscriptionlocalizationsgettomanyrelationship"></a>
# **SubscriptionsSubscriptionLocalizationsGetToManyRelationship**
> SubscriptionSubscriptionLocalizationsLinkagesResponse SubscriptionsSubscriptionLocalizationsGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsSubscriptionLocalizationsGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionSubscriptionLocalizationsLinkagesResponse result = apiInstance.SubscriptionsSubscriptionLocalizationsGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionLocalizationsGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsSubscriptionLocalizationsGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionSubscriptionLocalizationsLinkagesResponse> response = apiInstance.SubscriptionsSubscriptionLocalizationsGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsSubscriptionLocalizationsGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionSubscriptionLocalizationsLinkagesResponse**](SubscriptionSubscriptionLocalizationsLinkagesResponse.md)

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

<a id="subscriptionsupdateinstance"></a>
# **SubscriptionsUpdateInstance**
> SubscriptionResponse SubscriptionsUpdateInstance (string id, SubscriptionUpdateRequest subscriptionUpdateRequest)



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
    public class SubscriptionsUpdateInstanceExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var subscriptionUpdateRequest = new SubscriptionUpdateRequest(); // SubscriptionUpdateRequest | Subscription representation

            try
            {
                SubscriptionResponse result = apiInstance.SubscriptionsUpdateInstance(id, subscriptionUpdateRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsUpdateInstance: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsUpdateInstanceWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionResponse> response = apiInstance.SubscriptionsUpdateInstanceWithHttpInfo(id, subscriptionUpdateRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsUpdateInstanceWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **subscriptionUpdateRequest** | [**SubscriptionUpdateRequest**](SubscriptionUpdateRequest.md) | Subscription representation |  |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

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
| **200** | Single Subscription |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionswinbackoffersgettomanyrelated"></a>
# **SubscriptionsWinBackOffersGetToManyRelated**
> WinBackOffersResponse SubscriptionsWinBackOffersGetToManyRelated (string id, List<string>? fieldsWinBackOffers = null, List<string>? fieldsWinBackOfferPrices = null, int? limit = null, List<string>? include = null, int? limitPrices = null)



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
    public class SubscriptionsWinBackOffersGetToManyRelatedExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var fieldsWinBackOffers = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOffers (optional) 
            var fieldsWinBackOfferPrices = new List<string>?(); // List<string>? | the fields to include for returned resources of type winBackOfferPrices (optional) 
            var limit = 56;  // int? | maximum resources per page (optional) 
            var include = new List<string>?(); // List<string>? | comma-separated list of relationships to include (optional) 
            var limitPrices = 56;  // int? | maximum number of related prices returned (when they are included) (optional) 

            try
            {
                WinBackOffersResponse result = apiInstance.SubscriptionsWinBackOffersGetToManyRelated(id, fieldsWinBackOffers, fieldsWinBackOfferPrices, limit, include, limitPrices);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsWinBackOffersGetToManyRelated: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsWinBackOffersGetToManyRelatedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<WinBackOffersResponse> response = apiInstance.SubscriptionsWinBackOffersGetToManyRelatedWithHttpInfo(id, fieldsWinBackOffers, fieldsWinBackOfferPrices, limit, include, limitPrices);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsWinBackOffersGetToManyRelatedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsWinBackOffers** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOffers | [optional]  |
| **fieldsWinBackOfferPrices** | [**List&lt;string&gt;?**](string.md) | the fields to include for returned resources of type winBackOfferPrices | [optional]  |
| **limit** | **int?** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;?**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitPrices** | **int?** | maximum number of related prices returned (when they are included) | [optional]  |

### Return type

[**WinBackOffersResponse**](WinBackOffersResponse.md)

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
| **200** | List of WinBackOffers |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="subscriptionswinbackoffersgettomanyrelationship"></a>
# **SubscriptionsWinBackOffersGetToManyRelationship**
> SubscriptionWinBackOffersLinkagesResponse SubscriptionsWinBackOffersGetToManyRelationship (string id, int? limit = null)



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
    public class SubscriptionsWinBackOffersGetToManyRelationshipExample
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
            var apiInstance = new SubscriptionsApi(httpClient, config, httpClientHandler);
            var id = "id_example";  // string | the id of the requested resource
            var limit = 56;  // int? | maximum resources per page (optional) 

            try
            {
                SubscriptionWinBackOffersLinkagesResponse result = apiInstance.SubscriptionsWinBackOffersGetToManyRelationship(id, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsWinBackOffersGetToManyRelationship: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SubscriptionsWinBackOffersGetToManyRelationshipWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SubscriptionWinBackOffersLinkagesResponse> response = apiInstance.SubscriptionsWinBackOffersGetToManyRelationshipWithHttpInfo(id, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SubscriptionsApi.SubscriptionsWinBackOffersGetToManyRelationshipWithHttpInfo: " + e.Message);
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

[**SubscriptionWinBackOffersLinkagesResponse**](SubscriptionWinBackOffersLinkagesResponse.md)

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

