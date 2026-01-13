# AppStoreConnect.Net.Api.BetaGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaGroupsAppGetToOneRelated**](BetaGroupsApi.md#betagroupsappgettoonerelated) | **GET** /v1/betaGroups/{id}/app |  |
| [**BetaGroupsAppGetToOneRelationship**](BetaGroupsApi.md#betagroupsappgettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/app |  |
| [**BetaGroupsBetaRecruitmentCriteriaGetToOneRelated**](BetaGroupsApi.md#betagroupsbetarecruitmentcriteriagettoonerelated) | **GET** /v1/betaGroups/{id}/betaRecruitmentCriteria |  |
| [**BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship**](BetaGroupsApi.md#betagroupsbetarecruitmentcriteriagettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/betaRecruitmentCriteria |  |
| [**BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated**](BetaGroupsApi.md#betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelated) | **GET** /v1/betaGroups/{id}/betaRecruitmentCriterionCompatibleBuildCheck |  |
| [**BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship**](BetaGroupsApi.md#betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelationship) | **GET** /v1/betaGroups/{id}/relationships/betaRecruitmentCriterionCompatibleBuildCheck |  |
| [**BetaGroupsBetaTesterUsagesGetMetrics**](BetaGroupsApi.md#betagroupsbetatesterusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/betaTesterUsages |  |
| [**BetaGroupsBetaTestersCreateToManyRelationship**](BetaGroupsApi.md#betagroupsbetatesterscreatetomanyrelationship) | **POST** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBetaTestersDeleteToManyRelationship**](BetaGroupsApi.md#betagroupsbetatestersdeletetomanyrelationship) | **DELETE** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBetaTestersGetToManyRelated**](BetaGroupsApi.md#betagroupsbetatestersgettomanyrelated) | **GET** /v1/betaGroups/{id}/betaTesters |  |
| [**BetaGroupsBetaTestersGetToManyRelationship**](BetaGroupsApi.md#betagroupsbetatestersgettomanyrelationship) | **GET** /v1/betaGroups/{id}/relationships/betaTesters |  |
| [**BetaGroupsBuildsCreateToManyRelationship**](BetaGroupsApi.md#betagroupsbuildscreatetomanyrelationship) | **POST** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsBuildsDeleteToManyRelationship**](BetaGroupsApi.md#betagroupsbuildsdeletetomanyrelationship) | **DELETE** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsBuildsGetToManyRelated**](BetaGroupsApi.md#betagroupsbuildsgettomanyrelated) | **GET** /v1/betaGroups/{id}/builds |  |
| [**BetaGroupsBuildsGetToManyRelationship**](BetaGroupsApi.md#betagroupsbuildsgettomanyrelationship) | **GET** /v1/betaGroups/{id}/relationships/builds |  |
| [**BetaGroupsCreateInstance**](BetaGroupsApi.md#betagroupscreateinstance) | **POST** /v1/betaGroups |  |
| [**BetaGroupsDeleteInstance**](BetaGroupsApi.md#betagroupsdeleteinstance) | **DELETE** /v1/betaGroups/{id} |  |
| [**BetaGroupsGetCollection**](BetaGroupsApi.md#betagroupsgetcollection) | **GET** /v1/betaGroups |  |
| [**BetaGroupsGetInstance**](BetaGroupsApi.md#betagroupsgetinstance) | **GET** /v1/betaGroups/{id} |  |
| [**BetaGroupsPublicLinkUsagesGetMetrics**](BetaGroupsApi.md#betagroupspubliclinkusagesgetmetrics) | **GET** /v1/betaGroups/{id}/metrics/publicLinkUsages |  |
| [**BetaGroupsUpdateInstance**](BetaGroupsApi.md#betagroupsupdateinstance) | **PATCH** /v1/betaGroups/{id} |  |

<a id="betagroupsappgettoonerelated"></a>
# **BetaGroupsAppGetToOneRelated**
> AppWithoutIncludesResponse BetaGroupsAppGetToOneRelated (string id, List<string> fieldsApps = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
| **200** | Single App with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsappgettoonerelationship"></a>
# **BetaGroupsAppGetToOneRelationship**
> BetaGroupAppLinkageResponse BetaGroupsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupAppLinkageResponse**](BetaGroupAppLinkageResponse.md)

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetarecruitmentcriteriagettoonerelated"></a>
# **BetaGroupsBetaRecruitmentCriteriaGetToOneRelated**
> BetaRecruitmentCriterionResponse BetaGroupsBetaRecruitmentCriteriaGetToOneRelated (string id, List<string> fieldsBetaRecruitmentCriteria = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **200** | Single BetaRecruitmentCriterion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetarecruitmentcriteriagettoonerelationship"></a>
# **BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship**
> BetaGroupBetaRecruitmentCriteriaLinkageResponse BetaGroupsBetaRecruitmentCriteriaGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupBetaRecruitmentCriteriaLinkageResponse**](BetaGroupBetaRecruitmentCriteriaLinkageResponse.md)

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelated"></a>
# **BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated**
> BetaRecruitmentCriterionCompatibleBuildCheckResponse BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelated (string id, List<string> fieldsBetaRecruitmentCriterionCompatibleBuildChecks = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaRecruitmentCriterionCompatibleBuildChecks** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaRecruitmentCriterionCompatibleBuildChecks | [optional]  |

### Return type

[**BetaRecruitmentCriterionCompatibleBuildCheckResponse**](BetaRecruitmentCriterionCompatibleBuildCheckResponse.md)

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
| **200** | Single BetaRecruitmentCriterionCompatibleBuildCheck |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetarecruitmentcriterioncompatiblebuildcheckgettoonerelationship"></a>
# **BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship**
> BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse BetaGroupsBetaRecruitmentCriterionCompatibleBuildCheckGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse**](BetaGroupBetaRecruitmentCriterionCompatibleBuildCheckLinkageResponse.md)

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetatesterusagesgetmetrics"></a>
# **BetaGroupsBetaTesterUsagesGetMetrics**
> AppsBetaTesterUsagesV1MetricResponse BetaGroupsBetaTesterUsagesGetMetrics (string id, string period = null, List<string> groupBy = null, string filterBetaTesters = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **period** | **string** | the duration of the reporting period | [optional]  |
| **groupBy** | [**List&lt;string&gt;**](string.md) | the dimension by which to group the results | [optional]  |
| **filterBetaTesters** | **string** | filter by &#39;betaTesters&#39; relationship dimension | [optional]  |
| **limit** | **int** | maximum number of groups to return per page | [optional]  |

### Return type

[**AppsBetaTesterUsagesV1MetricResponse**](AppsBetaTesterUsagesV1MetricResponse.md)

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

<a id="betagroupsbetatesterscreatetomanyrelationship"></a>
# **BetaGroupsBetaTestersCreateToManyRelationship**
> void BetaGroupsBetaTestersCreateToManyRelationship (string id, BetaGroupBetaTestersLinkagesRequest betaGroupBetaTestersLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBetaTestersLinkagesRequest** | [**BetaGroupBetaTestersLinkagesRequest**](BetaGroupBetaTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbetatestersdeletetomanyrelationship"></a>
# **BetaGroupsBetaTestersDeleteToManyRelationship**
> void BetaGroupsBetaTestersDeleteToManyRelationship (string id, BetaGroupBetaTestersLinkagesRequest betaGroupBetaTestersLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBetaTestersLinkagesRequest** | [**BetaGroupBetaTestersLinkagesRequest**](BetaGroupBetaTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbetatestersgettomanyrelated"></a>
# **BetaGroupsBetaTestersGetToManyRelated**
> BetaTestersWithoutIncludesResponse BetaGroupsBetaTestersGetToManyRelated (string id, List<string> fieldsBetaTesters = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaTestersWithoutIncludesResponse**](BetaTestersWithoutIncludesResponse.md)

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
| **200** | List of BetaTesters with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsbetatestersgettomanyrelationship"></a>
# **BetaGroupsBetaTestersGetToManyRelationship**
> BetaGroupBetaTestersLinkagesResponse BetaGroupsBetaTestersGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaGroupBetaTestersLinkagesResponse**](BetaGroupBetaTestersLinkagesResponse.md)

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

<a id="betagroupsbuildscreatetomanyrelationship"></a>
# **BetaGroupsBuildsCreateToManyRelationship**
> void BetaGroupsBuildsCreateToManyRelationship (string id, BetaGroupBuildsLinkagesRequest betaGroupBuildsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBuildsLinkagesRequest** | [**BetaGroupBuildsLinkagesRequest**](BetaGroupBuildsLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbuildsdeletetomanyrelationship"></a>
# **BetaGroupsBuildsDeleteToManyRelationship**
> void BetaGroupsBuildsDeleteToManyRelationship (string id, BetaGroupBuildsLinkagesRequest betaGroupBuildsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupBuildsLinkagesRequest** | [**BetaGroupBuildsLinkagesRequest**](BetaGroupBuildsLinkagesRequest.md) | List of related linkages |  |

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

<a id="betagroupsbuildsgettomanyrelated"></a>
# **BetaGroupsBuildsGetToManyRelated**
> BuildsWithoutIncludesResponse BetaGroupsBuildsGetToManyRelated (string id, List<string> fieldsBuilds = null, int limit = null)




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

<a id="betagroupsbuildsgettomanyrelationship"></a>
# **BetaGroupsBuildsGetToManyRelationship**
> BetaGroupBuildsLinkagesResponse BetaGroupsBuildsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaGroupBuildsLinkagesResponse**](BetaGroupBuildsLinkagesResponse.md)

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

<a id="betagroupscreateinstance"></a>
# **BetaGroupsCreateInstance**
> BetaGroupResponse BetaGroupsCreateInstance (BetaGroupCreateRequest betaGroupCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaGroupCreateRequest** | [**BetaGroupCreateRequest**](BetaGroupCreateRequest.md) | BetaGroup representation |  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **201** | Single BetaGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsdeleteinstance"></a>
# **BetaGroupsDeleteInstance**
> void BetaGroupsDeleteInstance (string id)




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

<a id="betagroupsgetcollection"></a>
# **BetaGroupsGetCollection**
> BetaGroupsResponse BetaGroupsGetCollection (List<string> filterName = null, List<string> filterIsInternalGroup = null, List<string> filterPublicLinkEnabled = null, List<string> filterPublicLinkLimitEnabled = null, List<string> filterPublicLink = null, List<string> filterApp = null, List<string> filterBuilds = null, List<string> filterId = null, List<string> sort = null, List<string> fieldsBetaGroups = null, List<string> fieldsApps = null, List<string> fieldsBuilds = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaRecruitmentCriteria = null, int limit = null, List<string> include = null, int limitBetaTesters = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterName** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;name&#39; | [optional]  |
| **filterIsInternalGroup** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;isInternalGroup&#39; | [optional]  |
| **filterPublicLinkEnabled** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;publicLinkEnabled&#39; | [optional]  |
| **filterPublicLinkLimitEnabled** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;publicLinkLimitEnabled&#39; | [optional]  |
| **filterPublicLink** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;publicLink&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBuilds** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;builds&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaTesters** | **int** | maximum number of related betaTesters returned (when they are included) | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaGroupsResponse**](BetaGroupsResponse.md)

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
| **200** | List of BetaGroups |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupsgetinstance"></a>
# **BetaGroupsGetInstance**
> BetaGroupResponse BetaGroupsGetInstance (string id, List<string> fieldsBetaGroups = null, List<string> fieldsApps = null, List<string> fieldsBuilds = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaRecruitmentCriteria = null, List<string> include = null, int limitBetaTesters = null, int limitBuilds = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaRecruitmentCriteria** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaRecruitmentCriteria | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaTesters** | **int** | maximum number of related betaTesters returned (when they are included) | [optional]  |
| **limitBuilds** | **int** | maximum number of related builds returned (when they are included) | [optional]  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **200** | Single BetaGroup |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betagroupspubliclinkusagesgetmetrics"></a>
# **BetaGroupsPublicLinkUsagesGetMetrics**
> BetaPublicLinkUsagesV1MetricResponse BetaGroupsPublicLinkUsagesGetMetrics (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaPublicLinkUsagesV1MetricResponse**](BetaPublicLinkUsagesV1MetricResponse.md)

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

<a id="betagroupsupdateinstance"></a>
# **BetaGroupsUpdateInstance**
> BetaGroupResponse BetaGroupsUpdateInstance (string id, BetaGroupUpdateRequest betaGroupUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaGroupUpdateRequest** | [**BetaGroupUpdateRequest**](BetaGroupUpdateRequest.md) | BetaGroup representation |  |

### Return type

[**BetaGroupResponse**](BetaGroupResponse.md)

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
| **200** | Single BetaGroup |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

