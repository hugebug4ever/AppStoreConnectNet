# AppStoreConnect.Net.Api.BetaTestersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaTestersAppsDeleteToManyRelationship**](BetaTestersApi.md#betatestersappsdeletetomanyrelationship) | **DELETE** /v1/betaTesters/{id}/relationships/apps |  |
| [**BetaTestersAppsGetToManyRelated**](BetaTestersApi.md#betatestersappsgettomanyrelated) | **GET** /v1/betaTesters/{id}/apps |  |
| [**BetaTestersAppsGetToManyRelationship**](BetaTestersApi.md#betatestersappsgettomanyrelationship) | **GET** /v1/betaTesters/{id}/relationships/apps |  |
| [**BetaTestersBetaGroupsCreateToManyRelationship**](BetaTestersApi.md#betatestersbetagroupscreatetomanyrelationship) | **POST** /v1/betaTesters/{id}/relationships/betaGroups |  |
| [**BetaTestersBetaGroupsDeleteToManyRelationship**](BetaTestersApi.md#betatestersbetagroupsdeletetomanyrelationship) | **DELETE** /v1/betaTesters/{id}/relationships/betaGroups |  |
| [**BetaTestersBetaGroupsGetToManyRelated**](BetaTestersApi.md#betatestersbetagroupsgettomanyrelated) | **GET** /v1/betaTesters/{id}/betaGroups |  |
| [**BetaTestersBetaGroupsGetToManyRelationship**](BetaTestersApi.md#betatestersbetagroupsgettomanyrelationship) | **GET** /v1/betaTesters/{id}/relationships/betaGroups |  |
| [**BetaTestersBetaTesterUsagesGetMetrics**](BetaTestersApi.md#betatestersbetatesterusagesgetmetrics) | **GET** /v1/betaTesters/{id}/metrics/betaTesterUsages |  |
| [**BetaTestersBuildsCreateToManyRelationship**](BetaTestersApi.md#betatestersbuildscreatetomanyrelationship) | **POST** /v1/betaTesters/{id}/relationships/builds |  |
| [**BetaTestersBuildsDeleteToManyRelationship**](BetaTestersApi.md#betatestersbuildsdeletetomanyrelationship) | **DELETE** /v1/betaTesters/{id}/relationships/builds |  |
| [**BetaTestersBuildsGetToManyRelated**](BetaTestersApi.md#betatestersbuildsgettomanyrelated) | **GET** /v1/betaTesters/{id}/builds |  |
| [**BetaTestersBuildsGetToManyRelationship**](BetaTestersApi.md#betatestersbuildsgettomanyrelationship) | **GET** /v1/betaTesters/{id}/relationships/builds |  |
| [**BetaTestersCreateInstance**](BetaTestersApi.md#betatesterscreateinstance) | **POST** /v1/betaTesters |  |
| [**BetaTestersDeleteInstance**](BetaTestersApi.md#betatestersdeleteinstance) | **DELETE** /v1/betaTesters/{id} |  |
| [**BetaTestersGetCollection**](BetaTestersApi.md#betatestersgetcollection) | **GET** /v1/betaTesters |  |
| [**BetaTestersGetInstance**](BetaTestersApi.md#betatestersgetinstance) | **GET** /v1/betaTesters/{id} |  |

<a id="betatestersappsdeletetomanyrelationship"></a>
# **BetaTestersAppsDeleteToManyRelationship**
> void BetaTestersAppsDeleteToManyRelationship (string id, BetaTesterAppsLinkagesRequest betaTesterAppsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaTesterAppsLinkagesRequest** | [**BetaTesterAppsLinkagesRequest**](BetaTesterAppsLinkagesRequest.md) | List of related linkages |  |

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
| **202** | Accepted for future completion |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersappsgettomanyrelated"></a>
# **BetaTestersAppsGetToManyRelated**
> AppsWithoutIncludesResponse BetaTestersAppsGetToManyRelated (string id, List<string> fieldsApps = null, int limit = null)




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

<a id="betatestersappsgettomanyrelationship"></a>
# **BetaTestersAppsGetToManyRelationship**
> BetaTesterAppsLinkagesResponse BetaTestersAppsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaTesterAppsLinkagesResponse**](BetaTesterAppsLinkagesResponse.md)

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

<a id="betatestersbetagroupscreatetomanyrelationship"></a>
# **BetaTestersBetaGroupsCreateToManyRelationship**
> void BetaTestersBetaGroupsCreateToManyRelationship (string id, BetaTesterBetaGroupsLinkagesRequest betaTesterBetaGroupsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaTesterBetaGroupsLinkagesRequest** | [**BetaTesterBetaGroupsLinkagesRequest**](BetaTesterBetaGroupsLinkagesRequest.md) | List of related linkages |  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbetagroupsdeletetomanyrelationship"></a>
# **BetaTestersBetaGroupsDeleteToManyRelationship**
> void BetaTestersBetaGroupsDeleteToManyRelationship (string id, BetaTesterBetaGroupsLinkagesRequest betaTesterBetaGroupsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaTesterBetaGroupsLinkagesRequest** | [**BetaTesterBetaGroupsLinkagesRequest**](BetaTesterBetaGroupsLinkagesRequest.md) | List of related linkages |  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbetagroupsgettomanyrelated"></a>
# **BetaTestersBetaGroupsGetToManyRelated**
> BetaGroupsWithoutIncludesResponse BetaTestersBetaGroupsGetToManyRelated (string id, List<string> fieldsBetaGroups = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaGroupsWithoutIncludesResponse**](BetaGroupsWithoutIncludesResponse.md)

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
| **200** | List of BetaGroups with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbetagroupsgettomanyrelationship"></a>
# **BetaTestersBetaGroupsGetToManyRelationship**
> BetaTesterBetaGroupsLinkagesResponse BetaTestersBetaGroupsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaTesterBetaGroupsLinkagesResponse**](BetaTesterBetaGroupsLinkagesResponse.md)

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

<a id="betatestersbetatesterusagesgetmetrics"></a>
# **BetaTestersBetaTesterUsagesGetMetrics**
> BetaTesterUsagesV1MetricResponse BetaTestersBetaTesterUsagesGetMetrics (string id, string filterApps, string period = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterApps** | **string** | filter by &#39;apps&#39; relationship dimension |  |
| **period** | **string** | the duration of the reporting period | [optional]  |
| **limit** | **int** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaTesterUsagesV1MetricResponse**](BetaTesterUsagesV1MetricResponse.md)

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
| **200** | Metrics data response |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbuildscreatetomanyrelationship"></a>
# **BetaTestersBuildsCreateToManyRelationship**
> void BetaTestersBuildsCreateToManyRelationship (string id, BetaTesterBuildsLinkagesRequest betaTesterBuildsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaTesterBuildsLinkagesRequest** | [**BetaTesterBuildsLinkagesRequest**](BetaTesterBuildsLinkagesRequest.md) | List of related linkages |  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbuildsdeletetomanyrelationship"></a>
# **BetaTestersBuildsDeleteToManyRelationship**
> void BetaTestersBuildsDeleteToManyRelationship (string id, BetaTesterBuildsLinkagesRequest betaTesterBuildsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaTesterBuildsLinkagesRequest** | [**BetaTesterBuildsLinkagesRequest**](BetaTesterBuildsLinkagesRequest.md) | List of related linkages |  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbuildsgettomanyrelated"></a>
# **BetaTestersBuildsGetToManyRelated**
> BuildsWithoutIncludesResponse BetaTestersBuildsGetToManyRelated (string id, List<string> fieldsBuilds = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildsWithoutIncludesResponse**](BuildsWithoutIncludesResponse.md)

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
| **200** | List of Builds with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersbuildsgettomanyrelationship"></a>
# **BetaTestersBuildsGetToManyRelationship**
> BetaTesterBuildsLinkagesResponse BetaTestersBuildsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaTesterBuildsLinkagesResponse**](BetaTesterBuildsLinkagesResponse.md)

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

<a id="betatesterscreateinstance"></a>
# **BetaTestersCreateInstance**
> BetaTesterResponse BetaTestersCreateInstance (BetaTesterCreateRequest betaTesterCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaTesterCreateRequest** | [**BetaTesterCreateRequest**](BetaTesterCreateRequest.md) | BetaTester representation |  |

### Return type

[**BetaTesterResponse**](BetaTesterResponse.md)

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
| **201** | Single BetaTester |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersdeleteinstance"></a>
# **BetaTestersDeleteInstance**
> void BetaTestersDeleteInstance (string id)




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
| **202** | Accepted for future completion |  -  |
| **204** | Success (no content) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersgetcollection"></a>
# **BetaTestersGetCollection**
> BetaTestersResponse BetaTestersGetCollection (List<string> filterFirstName = null, List<string> filterLastName = null, List<string> filterEmail = null, List<string> filterInviteType = null, List<string> filterApps = null, List<string> filterBetaGroups = null, List<string> filterBuilds = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsBetaTesters = null, List<string> fieldsApps = null, List<string> fieldsBetaGroups = null, List<string> fieldsBuilds = null, int limit = null, List<string> include = null, int limitApps = null, int limitBetaGroups = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterFirstName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;firstName&#39; | [optional]  |
| **filterLastName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;lastName&#39; | [optional]  |
| **filterEmail** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;email&#39; | [optional]  |
| **filterInviteType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;inviteType&#39; | [optional]  |
| **filterApps** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;apps&#39; | [optional]  |
| **filterBetaGroups** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;betaGroups&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitApps** | **int** | maximum number of related apps returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaTestersResponse**](BetaTestersResponse.md)

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
| **200** | List of BetaTesters |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betatestersgetinstance"></a>
# **BetaTestersGetInstance**
> BetaTesterResponse BetaTestersGetInstance (string id, List<string> fieldsBetaTesters = null, List<string> fieldsApps = null, List<string> fieldsBetaGroups = null, List<string> fieldsBuilds = null, List<string> include = null, int limitApps = null, int limitBetaGroups = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitApps** | **int** | maximum number of related apps returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaTesterResponse**](BetaTesterResponse.md)

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
| **200** | Single BetaTester |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

