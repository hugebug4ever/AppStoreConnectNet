# AppStoreConnect.Net.Api.BuildBetaDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildBetaDetailsBuildGetToOneRelated**](BuildBetaDetailsApi.md#buildbetadetailsbuildgettoonerelated) | **GET** /v1/buildBetaDetails/{id}/build |  |
| [**BuildBetaDetailsBuildGetToOneRelationship**](BuildBetaDetailsApi.md#buildbetadetailsbuildgettoonerelationship) | **GET** /v1/buildBetaDetails/{id}/relationships/build |  |
| [**BuildBetaDetailsGetCollection**](BuildBetaDetailsApi.md#buildbetadetailsgetcollection) | **GET** /v1/buildBetaDetails |  |
| [**BuildBetaDetailsGetInstance**](BuildBetaDetailsApi.md#buildbetadetailsgetinstance) | **GET** /v1/buildBetaDetails/{id} |  |
| [**BuildBetaDetailsUpdateInstance**](BuildBetaDetailsApi.md#buildbetadetailsupdateinstance) | **PATCH** /v1/buildBetaDetails/{id} |  |

<a id="buildbetadetailsbuildgettoonerelated"></a>
# **BuildBetaDetailsBuildGetToOneRelated**
> BuildResponse BuildBetaDetailsBuildGetToOneRelated (string id, List<string> fieldsBuilds = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaGroups = null, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsApps = null, List<string> fieldsBuildBetaDetails = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsBuildIcons = null, List<string> fieldsBuildBundles = null, List<string> fieldsBuildUploads = null, List<string> include = null, int limitIndividualTesters = null, int limitBetaGroups = null, int limitBetaBuildLocalizations = null, int limitIcons = null, int limitBuildBundles = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaGroups** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaGroups | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **fieldsBuildBundles** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBundles | [optional]  |
| **fieldsBuildUploads** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildUploads | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitIndividualTesters** | **int** | maximum number of related individualTesters returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBetaBuildLocalizations** | **int** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitIcons** | **int** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int** | maximum number of related buildBundles returned (when they are included) | [optional]  |

### Return type

[**BuildResponse**](BuildResponse.md)

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
| **200** | Single Build |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbetadetailsbuildgettoonerelationship"></a>
# **BuildBetaDetailsBuildGetToOneRelationship**
> BuildBetaDetailBuildLinkageResponse BuildBetaDetailsBuildGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBetaDetailBuildLinkageResponse**](BuildBetaDetailBuildLinkageResponse.md)

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

<a id="buildbetadetailsgetcollection"></a>
# **BuildBetaDetailsGetCollection**
> BuildBetaDetailsResponse BuildBetaDetailsGetCollection (List<string> filterBuild = null, List<string> filterId = null, List<string> fieldsBuildBetaDetails = null, List<string> fieldsBuilds = null, int limit = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterBuild** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;build&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BuildBetaDetailsResponse**](BuildBetaDetailsResponse.md)

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
| **200** | List of BuildBetaDetails |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbetadetailsgetinstance"></a>
# **BuildBetaDetailsGetInstance**
> BuildBetaDetailResponse BuildBetaDetailsGetInstance (string id, List<string> fieldsBuildBetaDetails = null, List<string> fieldsBuilds = null, List<string> include = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
| **200** | Single BuildBetaDetail |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildbetadetailsupdateinstance"></a>
# **BuildBetaDetailsUpdateInstance**
> BuildBetaDetailResponse BuildBetaDetailsUpdateInstance (string id, BuildBetaDetailUpdateRequest buildBetaDetailUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaDetailUpdateRequest** | [**BuildBetaDetailUpdateRequest**](BuildBetaDetailUpdateRequest.md) | BuildBetaDetail representation |  |

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
| **200** | Single BuildBetaDetail |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

