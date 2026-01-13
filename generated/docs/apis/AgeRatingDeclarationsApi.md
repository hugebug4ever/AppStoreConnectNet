# AppStoreConnect.Net.Api.AgeRatingDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AgeRatingDeclarationsUpdateInstance**](AgeRatingDeclarationsApi.md#ageratingdeclarationsupdateinstance) | **PATCH** /v1/ageRatingDeclarations/{id} |  |

<a id="ageratingdeclarationsupdateinstance"></a>
# **AgeRatingDeclarationsUpdateInstance**
> AgeRatingDeclarationResponse AgeRatingDeclarationsUpdateInstance (string id, AgeRatingDeclarationUpdateRequest ageRatingDeclarationUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **ageRatingDeclarationUpdateRequest** | [**AgeRatingDeclarationUpdateRequest**](AgeRatingDeclarationUpdateRequest.md) | AgeRatingDeclaration representation |  |

### Return type

[**AgeRatingDeclarationResponse**](AgeRatingDeclarationResponse.md)

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
| **200** | Single AgeRatingDeclaration |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

