# AppStoreConnect.Net.Api.UserInvitationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**UserInvitationsCreateInstance**](UserInvitationsApi.md#userinvitationscreateinstance) | **POST** /v1/userInvitations |  |
| [**UserInvitationsDeleteInstance**](UserInvitationsApi.md#userinvitationsdeleteinstance) | **DELETE** /v1/userInvitations/{id} |  |
| [**UserInvitationsGetCollection**](UserInvitationsApi.md#userinvitationsgetcollection) | **GET** /v1/userInvitations |  |
| [**UserInvitationsGetInstance**](UserInvitationsApi.md#userinvitationsgetinstance) | **GET** /v1/userInvitations/{id} |  |
| [**UserInvitationsVisibleAppsGetToManyRelated**](UserInvitationsApi.md#userinvitationsvisibleappsgettomanyrelated) | **GET** /v1/userInvitations/{id}/visibleApps |  |
| [**UserInvitationsVisibleAppsGetToManyRelationship**](UserInvitationsApi.md#userinvitationsvisibleappsgettomanyrelationship) | **GET** /v1/userInvitations/{id}/relationships/visibleApps |  |

<a id="userinvitationscreateinstance"></a>
# **UserInvitationsCreateInstance**
> UserInvitationResponse UserInvitationsCreateInstance (UserInvitationCreateRequest userInvitationCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **userInvitationCreateRequest** | [**UserInvitationCreateRequest**](UserInvitationCreateRequest.md) | UserInvitation representation |  |

### Return type

[**UserInvitationResponse**](UserInvitationResponse.md)

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
| **201** | Single UserInvitation |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="userinvitationsdeleteinstance"></a>
# **UserInvitationsDeleteInstance**
> void UserInvitationsDeleteInstance (string id)




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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="userinvitationsgetcollection"></a>
# **UserInvitationsGetCollection**
> UserInvitationsResponse UserInvitationsGetCollection (List<string> filterEmail = null, List<string> filterRoles = null, List<string> filterVisibleApps = null, List<string> sort = null, List<string> fieldsUserInvitations = null, List<string> fieldsApps = null, int limit = null, List<string> include = null, int limitVisibleApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterEmail** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;email&#39; | [optional]  |
| **filterRoles** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;roles&#39; | [optional]  |
| **filterVisibleApps** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;visibleApps&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsUserInvitations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type userInvitations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVisibleApps** | **int** | maximum number of related visibleApps returned (when they are included) | [optional]  |

### Return type

[**UserInvitationsResponse**](UserInvitationsResponse.md)

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
| **200** | List of UserInvitations |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="userinvitationsgetinstance"></a>
# **UserInvitationsGetInstance**
> UserInvitationResponse UserInvitationsGetInstance (string id, List<string> fieldsUserInvitations = null, List<string> fieldsApps = null, List<string> include = null, int limitVisibleApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsUserInvitations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type userInvitations | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitVisibleApps** | **int** | maximum number of related visibleApps returned (when they are included) | [optional]  |

### Return type

[**UserInvitationResponse**](UserInvitationResponse.md)

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
| **200** | Single UserInvitation |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="userinvitationsvisibleappsgettomanyrelated"></a>
# **UserInvitationsVisibleAppsGetToManyRelated**
> AppsWithoutIncludesResponse UserInvitationsVisibleAppsGetToManyRelated (string id, List<string> fieldsApps = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**AppsWithoutIncludesResponse**](AppsWithoutIncludesResponse.md)

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
| **200** | List of Apps with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="userinvitationsvisibleappsgettomanyrelationship"></a>
# **UserInvitationsVisibleAppsGetToManyRelationship**
> UserInvitationVisibleAppsLinkagesResponse UserInvitationsVisibleAppsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**UserInvitationVisibleAppsLinkagesResponse**](UserInvitationVisibleAppsLinkagesResponse.md)

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

