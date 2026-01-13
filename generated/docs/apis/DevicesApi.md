# AppStoreConnect.Net.Api.DevicesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**DevicesCreateInstance**](DevicesApi.md#devicescreateinstance) | **POST** /v1/devices |  |
| [**DevicesGetCollection**](DevicesApi.md#devicesgetcollection) | **GET** /v1/devices |  |
| [**DevicesGetInstance**](DevicesApi.md#devicesgetinstance) | **GET** /v1/devices/{id} |  |
| [**DevicesUpdateInstance**](DevicesApi.md#devicesupdateinstance) | **PATCH** /v1/devices/{id} |  |

<a id="devicescreateinstance"></a>
# **DevicesCreateInstance**
> DeviceResponse DevicesCreateInstance (DeviceCreateRequest deviceCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **deviceCreateRequest** | [**DeviceCreateRequest**](DeviceCreateRequest.md) | Device representation |  |

### Return type

[**DeviceResponse**](DeviceResponse.md)

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
| **201** | Single Device |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="devicesgetcollection"></a>
# **DevicesGetCollection**
> DevicesResponse DevicesGetCollection (List<string> filterName = null, List<string> filterPlatform = null, List<string> filterUdid = null, List<string> filterStatus = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsDevices = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterUdid** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;udid&#39; | [optional]  |
| **filterStatus** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;status&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsDevices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type devices | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**DevicesResponse**](DevicesResponse.md)

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
| **200** | List of Devices |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="devicesgetinstance"></a>
# **DevicesGetInstance**
> DeviceResponse DevicesGetInstance (string id, List<string> fieldsDevices = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsDevices** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type devices | [optional]  |

### Return type

[**DeviceResponse**](DeviceResponse.md)

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
| **200** | Single Device |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="devicesupdateinstance"></a>
# **DevicesUpdateInstance**
> DeviceResponse DevicesUpdateInstance (string id, DeviceUpdateRequest deviceUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **deviceUpdateRequest** | [**DeviceUpdateRequest**](DeviceUpdateRequest.md) | Device representation |  |

### Return type

[**DeviceResponse**](DeviceResponse.md)

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
| **200** | Single Device |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

