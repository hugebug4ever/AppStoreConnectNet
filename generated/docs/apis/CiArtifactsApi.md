# AppStoreConnect.Net.Api.CiArtifactsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CiArtifactsGetInstance**](CiArtifactsApi.md#ciartifactsgetinstance) | **GET** /v1/ciArtifacts/{id} |  |

<a id="ciartifactsgetinstance"></a>
# **CiArtifactsGetInstance**
> CiArtifactResponse CiArtifactsGetInstance (string id, List<string> fieldsCiArtifacts = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsCiArtifacts** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ciArtifacts | [optional]  |

### Return type

[**CiArtifactResponse**](CiArtifactResponse.md)

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
| **200** | Single CiArtifact |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

