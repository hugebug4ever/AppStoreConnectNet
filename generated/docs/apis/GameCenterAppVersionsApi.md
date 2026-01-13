# AppStoreConnect.Net.Api.GameCenterAppVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GameCenterAppVersionsAppStoreVersionGetToOneRelated**](GameCenterAppVersionsApi.md#gamecenterappversionsappstoreversiongettoonerelated) | **GET** /v1/gameCenterAppVersions/{id}/appStoreVersion |  |
| [**GameCenterAppVersionsAppStoreVersionGetToOneRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionsappstoreversiongettoonerelationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/appStoreVersion |  |
| [**GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionscreatetomanyrelationship) | **POST** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsdeletetomanyrelationship) | **DELETE** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsGetToManyRelated**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsgettomanyrelated) | **GET** /v1/gameCenterAppVersions/{id}/compatibilityVersions |  |
| [**GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship**](GameCenterAppVersionsApi.md#gamecenterappversionscompatibilityversionsgettomanyrelationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions |  |
| [**GameCenterAppVersionsCreateInstance**](GameCenterAppVersionsApi.md#gamecenterappversionscreateinstance) | **POST** /v1/gameCenterAppVersions |  |
| [**GameCenterAppVersionsGetInstance**](GameCenterAppVersionsApi.md#gamecenterappversionsgetinstance) | **GET** /v1/gameCenterAppVersions/{id} |  |
| [**GameCenterAppVersionsUpdateInstance**](GameCenterAppVersionsApi.md#gamecenterappversionsupdateinstance) | **PATCH** /v1/gameCenterAppVersions/{id} |  |

<a id="gamecenterappversionsappstoreversiongettoonerelated"></a>
# **GameCenterAppVersionsAppStoreVersionGetToOneRelated**
> AppStoreVersionResponse GameCenterAppVersionsAppStoreVersionGetToOneRelated (string id, List<string> fieldsAppStoreVersions = null, List<string> fieldsApps = null, List<string> fieldsAgeRatingDeclarations = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsBuilds = null, List<string> fieldsAppStoreVersionPhasedReleases = null, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsRoutingAppCoverages = null, List<string> fieldsAppStoreReviewDetails = null, List<string> fieldsAppStoreVersionSubmissions = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAlternativeDistributionPackages = null, List<string> include = null, int limitAppStoreVersionLocalizations = null, int limitAppStoreVersionExperiments = null, int limitAppStoreVersionExperimentsV2 = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsAgeRatingDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type ageRatingDeclarations | [optional]  |
| **fieldsAppStoreVersionLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionLocalizations | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsAppStoreVersionPhasedReleases** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsRoutingAppCoverages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type routingAppCoverages | [optional]  |
| **fieldsAppStoreReviewDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreReviewDetails | [optional]  |
| **fieldsAppStoreVersionSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionSubmissions | [optional]  |
| **fieldsAppClipDefaultExperiences** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appClipDefaultExperiences | [optional]  |
| **fieldsAppStoreVersionExperiments** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersionExperiments | [optional]  |
| **fieldsAlternativeDistributionPackages** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type alternativeDistributionPackages | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitAppStoreVersionLocalizations** | **int** | maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperiments** | **int** | maximum number of related appStoreVersionExperiments returned (when they are included) | [optional]  |
| **limitAppStoreVersionExperimentsV2** | **int** | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional]  |

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
| **200** | Single AppStoreVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterappversionsappstoreversiongettoonerelationship"></a>
# **GameCenterAppVersionsAppStoreVersionGetToOneRelationship**
> GameCenterAppVersionAppStoreVersionLinkageResponse GameCenterAppVersionsAppStoreVersionGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**GameCenterAppVersionAppStoreVersionLinkageResponse**](GameCenterAppVersionAppStoreVersionLinkageResponse.md)

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

<a id="gamecenterappversionscompatibilityversionscreatetomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship**
> void GameCenterAppVersionsCompatibilityVersionsCreateToManyRelationship (string id, GameCenterAppVersionCompatibilityVersionsLinkagesRequest gameCenterAppVersionCompatibilityVersionsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionCompatibilityVersionsLinkagesRequest** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterappversionscompatibilityversionsdeletetomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship**
> void GameCenterAppVersionsCompatibilityVersionsDeleteToManyRelationship (string id, GameCenterAppVersionCompatibilityVersionsLinkagesRequest gameCenterAppVersionCompatibilityVersionsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionCompatibilityVersionsLinkagesRequest** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md) | List of related linkages |  |

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

<a id="gamecenterappversionscompatibilityversionsgettomanyrelated"></a>
# **GameCenterAppVersionsCompatibilityVersionsGetToManyRelated**
> GameCenterAppVersionsResponse GameCenterAppVersionsCompatibilityVersionsGetToManyRelated (string id, List<string> filterEnabled = null, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsAppStoreVersions = null, int limit = null, List<string> include = null, int limitCompatibilityVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterEnabled** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;enabled&#39; | [optional]  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCompatibilityVersions** | **int** | maximum number of related compatibilityVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAppVersionsResponse**](GameCenterAppVersionsResponse.md)

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
| **200** | List of GameCenterAppVersions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterappversionscompatibilityversionsgettomanyrelationship"></a>
# **GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship**
> GameCenterAppVersionCompatibilityVersionsLinkagesResponse GameCenterAppVersionsCompatibilityVersionsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**GameCenterAppVersionCompatibilityVersionsLinkagesResponse**](GameCenterAppVersionCompatibilityVersionsLinkagesResponse.md)

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

<a id="gamecenterappversionscreateinstance"></a>
# **GameCenterAppVersionsCreateInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsCreateInstance (GameCenterAppVersionCreateRequest gameCenterAppVersionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameCenterAppVersionCreateRequest** | [**GameCenterAppVersionCreateRequest**](GameCenterAppVersionCreateRequest.md) | GameCenterAppVersion representation |  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **201** | Single GameCenterAppVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterappversionsgetinstance"></a>
# **GameCenterAppVersionsGetInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsGetInstance (string id, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsAppStoreVersions = null, List<string> include = null, int limitCompatibilityVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsGameCenterAppVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type gameCenterAppVersions | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitCompatibilityVersions** | **int** | maximum number of related compatibilityVersions returned (when they are included) | [optional]  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **200** | Single GameCenterAppVersion |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="gamecenterappversionsupdateinstance"></a>
# **GameCenterAppVersionsUpdateInstance**
> GameCenterAppVersionResponse GameCenterAppVersionsUpdateInstance (string id, GameCenterAppVersionUpdateRequest gameCenterAppVersionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **gameCenterAppVersionUpdateRequest** | [**GameCenterAppVersionUpdateRequest**](GameCenterAppVersionUpdateRequest.md) | GameCenterAppVersion representation |  |

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
| **200** | Single GameCenterAppVersion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

