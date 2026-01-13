# AppStoreConnect.Net.Api.BetaTesterInvitationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaTesterInvitationsCreateInstance**](BetaTesterInvitationsApi.md#betatesterinvitationscreateinstance) | **POST** /v1/betaTesterInvitations |  |

<a id="betatesterinvitationscreateinstance"></a>
# **BetaTesterInvitationsCreateInstance**
> BetaTesterInvitationResponse BetaTesterInvitationsCreateInstance (BetaTesterInvitationCreateRequest betaTesterInvitationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaTesterInvitationCreateRequest** | [**BetaTesterInvitationCreateRequest**](BetaTesterInvitationCreateRequest.md) | BetaTesterInvitation representation |  |

### Return type

[**BetaTesterInvitationResponse**](BetaTesterInvitationResponse.md)

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
| **201** | Single BetaTesterInvitation |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

