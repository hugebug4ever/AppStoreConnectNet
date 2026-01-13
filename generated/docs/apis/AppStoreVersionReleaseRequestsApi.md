# AppStoreConnect.Net.Api.AppStoreVersionReleaseRequestsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AppStoreVersionReleaseRequestsCreateInstance**](AppStoreVersionReleaseRequestsApi.md#appstoreversionreleaserequestscreateinstance) | **POST** /v1/appStoreVersionReleaseRequests |  |

<a id="appstoreversionreleaserequestscreateinstance"></a>
# **AppStoreVersionReleaseRequestsCreateInstance**
> AppStoreVersionReleaseRequestResponse AppStoreVersionReleaseRequestsCreateInstance (AppStoreVersionReleaseRequestCreateRequest appStoreVersionReleaseRequestCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **appStoreVersionReleaseRequestCreateRequest** | [**AppStoreVersionReleaseRequestCreateRequest**](AppStoreVersionReleaseRequestCreateRequest.md) | AppStoreVersionReleaseRequest representation |  |

### Return type

[**AppStoreVersionReleaseRequestResponse**](AppStoreVersionReleaseRequestResponse.md)

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
| **201** | Single AppStoreVersionReleaseRequest |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

