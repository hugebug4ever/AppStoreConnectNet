# AppStoreConnect.Net.Api.AlternativeDistributionPackageVariantsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AlternativeDistributionPackageVariantsGetInstance**](AlternativeDistributionPackageVariantsApi.md#alternativedistributionpackagevariantsgetinstance) | **GET** /v1/alternativeDistributionPackageVariants/{id} |  |

<a id="alternativedistributionpackagevariantsgetinstance"></a>
# **AlternativeDistributionPackageVariantsGetInstance**
> AlternativeDistributionPackageVariantResponse AlternativeDistributionPackageVariantsGetInstance (string id, List<string> fieldsAlternativeDistributionPackageVariants = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAlternativeDistributionPackageVariants** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional]  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

