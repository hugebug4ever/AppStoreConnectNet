# AppStoreConnect.Net.Api.ReviewSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ReviewSubmissionsCreateInstance**](ReviewSubmissionsApi.md#reviewsubmissionscreateinstance) | **POST** /v1/reviewSubmissions |  |
| [**ReviewSubmissionsGetCollection**](ReviewSubmissionsApi.md#reviewsubmissionsgetcollection) | **GET** /v1/reviewSubmissions |  |
| [**ReviewSubmissionsGetInstance**](ReviewSubmissionsApi.md#reviewsubmissionsgetinstance) | **GET** /v1/reviewSubmissions/{id} |  |
| [**ReviewSubmissionsItemsGetToManyRelated**](ReviewSubmissionsApi.md#reviewsubmissionsitemsgettomanyrelated) | **GET** /v1/reviewSubmissions/{id}/items |  |
| [**ReviewSubmissionsItemsGetToManyRelationship**](ReviewSubmissionsApi.md#reviewsubmissionsitemsgettomanyrelationship) | **GET** /v1/reviewSubmissions/{id}/relationships/items |  |
| [**ReviewSubmissionsUpdateInstance**](ReviewSubmissionsApi.md#reviewsubmissionsupdateinstance) | **PATCH** /v1/reviewSubmissions/{id} |  |

<a id="reviewsubmissionscreateinstance"></a>
# **ReviewSubmissionsCreateInstance**
> ReviewSubmissionResponse ReviewSubmissionsCreateInstance (ReviewSubmissionCreateRequest reviewSubmissionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **reviewSubmissionCreateRequest** | [**ReviewSubmissionCreateRequest**](ReviewSubmissionCreateRequest.md) | ReviewSubmission representation |  |

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
| **201** | Single ReviewSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reviewsubmissionsgetcollection"></a>
# **ReviewSubmissionsGetCollection**
> ReviewSubmissionsResponse ReviewSubmissionsGetCollection (List<string> filterApp, List<string> filterPlatform = null, List<string> filterState = null, List<string> fieldsReviewSubmissions = null, List<string> fieldsReviewSubmissionItems = null, int limit = null, List<string> include = null, int limitItems = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; |  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;state&#39; | [optional]  |
| **fieldsReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissions | [optional]  |
| **fieldsReviewSubmissionItems** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissionItems | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitItems** | **int** | maximum number of related items returned (when they are included) | [optional]  |

### Return type

[**ReviewSubmissionsResponse**](ReviewSubmissionsResponse.md)

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
| **200** | List of ReviewSubmissions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reviewsubmissionsgetinstance"></a>
# **ReviewSubmissionsGetInstance**
> ReviewSubmissionResponse ReviewSubmissionsGetInstance (string id, List<string> fieldsReviewSubmissions = null, List<string> fieldsReviewSubmissionItems = null, List<string> include = null, int limitItems = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissions | [optional]  |
| **fieldsReviewSubmissionItems** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissionItems | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitItems** | **int** | maximum number of related items returned (when they are included) | [optional]  |

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
| **200** | Single ReviewSubmission |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reviewsubmissionsitemsgettomanyrelated"></a>
# **ReviewSubmissionsItemsGetToManyRelated**
> ReviewSubmissionItemsResponse ReviewSubmissionsItemsGetToManyRelated (string id, List<string> fieldsReviewSubmissionItems = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsAppCustomProductPageVersions = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAppEvents = null, List<string> fieldsBackgroundAssetVersions = null, List<string> fieldsGameCenterAchievementVersions = null, List<string> fieldsGameCenterActivityVersions = null, List<string> fieldsGameCenterChallengeVersions = null, List<string> fieldsGameCenterLeaderboardSetVersions = null, List<string> fieldsGameCenterLeaderboardVersions = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsReviewSubmissionItems** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type reviewSubmissionItems | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsAppCustomProductPageVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appCustomProductPageVersions | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAppEvents** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEvents | [optional]  |
| **fieldsBackgroundAssetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type backgroundAssetVersions | [optional]  |
| **fieldsGameCenterAchievementVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAchievementVersions | [optional]  |
| **fieldsGameCenterActivityVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterActivityVersions | [optional]  |
| **fieldsGameCenterChallengeVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterChallengeVersions | [optional]  |
| **fieldsGameCenterLeaderboardSetVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardSetVersions | [optional]  |
| **fieldsGameCenterLeaderboardVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterLeaderboardVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**ReviewSubmissionItemsResponse**](ReviewSubmissionItemsResponse.md)

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
| **200** | List of ReviewSubmissionItems |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reviewsubmissionsitemsgettomanyrelationship"></a>
# **ReviewSubmissionsItemsGetToManyRelationship**
> ReviewSubmissionItemsLinkagesResponse ReviewSubmissionsItemsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**ReviewSubmissionItemsLinkagesResponse**](ReviewSubmissionItemsLinkagesResponse.md)

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

<a id="reviewsubmissionsupdateinstance"></a>
# **ReviewSubmissionsUpdateInstance**
> ReviewSubmissionResponse ReviewSubmissionsUpdateInstance (string id, ReviewSubmissionUpdateRequest reviewSubmissionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **reviewSubmissionUpdateRequest** | [**ReviewSubmissionUpdateRequest**](ReviewSubmissionUpdateRequest.md) | ReviewSubmission representation |  |

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
| **200** | Single ReviewSubmission |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

