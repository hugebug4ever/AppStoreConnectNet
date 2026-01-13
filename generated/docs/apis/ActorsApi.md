# AppStoreConnect.Net.Api.ActorsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ActorsGetCollection**](ActorsApi.md#actorsgetcollection) | **GET** /v1/actors |  |
| [**ActorsGetInstance**](ActorsApi.md#actorsgetinstance) | **GET** /v1/actors/{id} |  |

<a id="actorsgetcollection"></a>
# **ActorsGetCollection**
> ActorsResponse ActorsGetCollection (List<string> filterId, List<string> fieldsActors = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) |  |
| **fieldsActors** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type actors | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ActorsResponse**](ActorsResponse.md)

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
| **200** | List of Actors |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="actorsgetinstance"></a>
# **ActorsGetInstance**
> ActorResponse ActorsGetInstance (string id, List<string> fieldsActors = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsActors** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type actors | [optional]  |

### Return type

[**ActorResponse**](ActorResponse.md)

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
| **200** | Single Actor |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

