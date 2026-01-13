# AppStoreConnect.Net.Api.BuildsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BuildsAppEncryptionDeclarationGetToOneRelated**](BuildsApi.md#buildsappencryptiondeclarationgettoonerelated) | **GET** /v1/builds/{id}/appEncryptionDeclaration |  |
| [**BuildsAppEncryptionDeclarationGetToOneRelationship**](BuildsApi.md#buildsappencryptiondeclarationgettoonerelationship) | **GET** /v1/builds/{id}/relationships/appEncryptionDeclaration |  |
| [**BuildsAppEncryptionDeclarationUpdateToOneRelationship**](BuildsApi.md#buildsappencryptiondeclarationupdatetoonerelationship) | **PATCH** /v1/builds/{id}/relationships/appEncryptionDeclaration |  |
| [**BuildsAppGetToOneRelated**](BuildsApi.md#buildsappgettoonerelated) | **GET** /v1/builds/{id}/app |  |
| [**BuildsAppGetToOneRelationship**](BuildsApi.md#buildsappgettoonerelationship) | **GET** /v1/builds/{id}/relationships/app |  |
| [**BuildsAppStoreVersionGetToOneRelated**](BuildsApi.md#buildsappstoreversiongettoonerelated) | **GET** /v1/builds/{id}/appStoreVersion |  |
| [**BuildsAppStoreVersionGetToOneRelationship**](BuildsApi.md#buildsappstoreversiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/appStoreVersion |  |
| [**BuildsBetaAppReviewSubmissionGetToOneRelated**](BuildsApi.md#buildsbetaappreviewsubmissiongettoonerelated) | **GET** /v1/builds/{id}/betaAppReviewSubmission |  |
| [**BuildsBetaAppReviewSubmissionGetToOneRelationship**](BuildsApi.md#buildsbetaappreviewsubmissiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/betaAppReviewSubmission |  |
| [**BuildsBetaBuildLocalizationsGetToManyRelated**](BuildsApi.md#buildsbetabuildlocalizationsgettomanyrelated) | **GET** /v1/builds/{id}/betaBuildLocalizations |  |
| [**BuildsBetaBuildLocalizationsGetToManyRelationship**](BuildsApi.md#buildsbetabuildlocalizationsgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/betaBuildLocalizations |  |
| [**BuildsBetaBuildUsagesGetMetrics**](BuildsApi.md#buildsbetabuildusagesgetmetrics) | **GET** /v1/builds/{id}/metrics/betaBuildUsages |  |
| [**BuildsBetaGroupsCreateToManyRelationship**](BuildsApi.md#buildsbetagroupscreatetomanyrelationship) | **POST** /v1/builds/{id}/relationships/betaGroups |  |
| [**BuildsBetaGroupsDeleteToManyRelationship**](BuildsApi.md#buildsbetagroupsdeletetomanyrelationship) | **DELETE** /v1/builds/{id}/relationships/betaGroups |  |
| [**BuildsBuildBetaDetailGetToOneRelated**](BuildsApi.md#buildsbuildbetadetailgettoonerelated) | **GET** /v1/builds/{id}/buildBetaDetail |  |
| [**BuildsBuildBetaDetailGetToOneRelationship**](BuildsApi.md#buildsbuildbetadetailgettoonerelationship) | **GET** /v1/builds/{id}/relationships/buildBetaDetail |  |
| [**BuildsDiagnosticSignaturesGetToManyRelated**](BuildsApi.md#buildsdiagnosticsignaturesgettomanyrelated) | **GET** /v1/builds/{id}/diagnosticSignatures |  |
| [**BuildsDiagnosticSignaturesGetToManyRelationship**](BuildsApi.md#buildsdiagnosticsignaturesgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/diagnosticSignatures |  |
| [**BuildsGetCollection**](BuildsApi.md#buildsgetcollection) | **GET** /v1/builds |  |
| [**BuildsGetInstance**](BuildsApi.md#buildsgetinstance) | **GET** /v1/builds/{id} |  |
| [**BuildsIconsGetToManyRelated**](BuildsApi.md#buildsiconsgettomanyrelated) | **GET** /v1/builds/{id}/icons |  |
| [**BuildsIconsGetToManyRelationship**](BuildsApi.md#buildsiconsgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/icons |  |
| [**BuildsIndividualTestersCreateToManyRelationship**](BuildsApi.md#buildsindividualtesterscreatetomanyrelationship) | **POST** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsIndividualTestersDeleteToManyRelationship**](BuildsApi.md#buildsindividualtestersdeletetomanyrelationship) | **DELETE** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsIndividualTestersGetToManyRelated**](BuildsApi.md#buildsindividualtestersgettomanyrelated) | **GET** /v1/builds/{id}/individualTesters |  |
| [**BuildsIndividualTestersGetToManyRelationship**](BuildsApi.md#buildsindividualtestersgettomanyrelationship) | **GET** /v1/builds/{id}/relationships/individualTesters |  |
| [**BuildsPerfPowerMetricsGetToManyRelated**](BuildsApi.md#buildsperfpowermetricsgettomanyrelated) | **GET** /v1/builds/{id}/perfPowerMetrics |  |
| [**BuildsPreReleaseVersionGetToOneRelated**](BuildsApi.md#buildsprereleaseversiongettoonerelated) | **GET** /v1/builds/{id}/preReleaseVersion |  |
| [**BuildsPreReleaseVersionGetToOneRelationship**](BuildsApi.md#buildsprereleaseversiongettoonerelationship) | **GET** /v1/builds/{id}/relationships/preReleaseVersion |  |
| [**BuildsUpdateInstance**](BuildsApi.md#buildsupdateinstance) | **PATCH** /v1/builds/{id} |  |

<a id="buildsappencryptiondeclarationgettoonerelated"></a>
# **BuildsAppEncryptionDeclarationGetToOneRelated**
> AppEncryptionDeclarationWithoutIncludesResponse BuildsAppEncryptionDeclarationGetToOneRelated (string id, List<string> fieldsAppEncryptionDeclarations = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |

### Return type

[**AppEncryptionDeclarationWithoutIncludesResponse**](AppEncryptionDeclarationWithoutIncludesResponse.md)

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
| **200** | Single AppEncryptionDeclaration with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsappencryptiondeclarationgettoonerelationship"></a>
# **BuildsAppEncryptionDeclarationGetToOneRelationship**
> BuildAppEncryptionDeclarationLinkageResponse BuildsAppEncryptionDeclarationGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppEncryptionDeclarationLinkageResponse**](BuildAppEncryptionDeclarationLinkageResponse.md)

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

<a id="buildsappencryptiondeclarationupdatetoonerelationship"></a>
# **BuildsAppEncryptionDeclarationUpdateToOneRelationship**
> void BuildsAppEncryptionDeclarationUpdateToOneRelationship (string id, BuildAppEncryptionDeclarationLinkageRequest buildAppEncryptionDeclarationLinkageRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildAppEncryptionDeclarationLinkageRequest** | [**BuildAppEncryptionDeclarationLinkageRequest**](BuildAppEncryptionDeclarationLinkageRequest.md) | Related linkage |  |

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

<a id="buildsappgettoonerelated"></a>
# **BuildsAppGetToOneRelated**
> AppWithoutIncludesResponse BuildsAppGetToOneRelated (string id, List<string> fieldsApps = null)




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

<a id="buildsappgettoonerelationship"></a>
# **BuildsAppGetToOneRelationship**
> BuildAppLinkageResponse BuildsAppGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppLinkageResponse**](BuildAppLinkageResponse.md)

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

<a id="buildsappstoreversiongettoonerelated"></a>
# **BuildsAppStoreVersionGetToOneRelated**
> AppStoreVersionResponse BuildsAppStoreVersionGetToOneRelated (string id, List<string> fieldsAppStoreVersions = null, List<string> fieldsApps = null, List<string> fieldsAgeRatingDeclarations = null, List<string> fieldsAppStoreVersionLocalizations = null, List<string> fieldsBuilds = null, List<string> fieldsAppStoreVersionPhasedReleases = null, List<string> fieldsGameCenterAppVersions = null, List<string> fieldsRoutingAppCoverages = null, List<string> fieldsAppStoreReviewDetails = null, List<string> fieldsAppStoreVersionSubmissions = null, List<string> fieldsAppClipDefaultExperiences = null, List<string> fieldsAppStoreVersionExperiments = null, List<string> fieldsAlternativeDistributionPackages = null, List<string> include = null, int limitAppStoreVersionLocalizations = null, int limitAppStoreVersionExperiments = null, int limitAppStoreVersionExperimentsV2 = null)




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

<a id="buildsappstoreversiongettoonerelationship"></a>
# **BuildsAppStoreVersionGetToOneRelationship**
> BuildAppStoreVersionLinkageResponse BuildsAppStoreVersionGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildAppStoreVersionLinkageResponse**](BuildAppStoreVersionLinkageResponse.md)

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

<a id="buildsbetaappreviewsubmissiongettoonerelated"></a>
# **BuildsBetaAppReviewSubmissionGetToOneRelated**
> BetaAppReviewSubmissionWithoutIncludesResponse BuildsBetaAppReviewSubmissionGetToOneRelated (string id, List<string> fieldsBetaAppReviewSubmissions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |

### Return type

[**BetaAppReviewSubmissionWithoutIncludesResponse**](BetaAppReviewSubmissionWithoutIncludesResponse.md)

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
| **200** | Single BetaAppReviewSubmission with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsbetaappreviewsubmissiongettoonerelationship"></a>
# **BuildsBetaAppReviewSubmissionGetToOneRelationship**
> BuildBetaAppReviewSubmissionLinkageResponse BuildsBetaAppReviewSubmissionGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBetaAppReviewSubmissionLinkageResponse**](BuildBetaAppReviewSubmissionLinkageResponse.md)

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

<a id="buildsbetabuildlocalizationsgettomanyrelated"></a>
# **BuildsBetaBuildLocalizationsGetToManyRelated**
> BetaBuildLocalizationsWithoutIncludesResponse BuildsBetaBuildLocalizationsGetToManyRelated (string id, List<string> fieldsBetaBuildLocalizations = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaBuildLocalizationsWithoutIncludesResponse**](BetaBuildLocalizationsWithoutIncludesResponse.md)

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
| **200** | List of BetaBuildLocalizations with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsbetabuildlocalizationsgettomanyrelationship"></a>
# **BuildsBetaBuildLocalizationsGetToManyRelationship**
> BuildBetaBuildLocalizationsLinkagesResponse BuildsBetaBuildLocalizationsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildBetaBuildLocalizationsLinkagesResponse**](BuildBetaBuildLocalizationsLinkagesResponse.md)

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

<a id="buildsbetabuildusagesgetmetrics"></a>
# **BuildsBetaBuildUsagesGetMetrics**
> BetaBuildUsagesV1MetricResponse BuildsBetaBuildUsagesGetMetrics (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum number of groups to return per page | [optional]  |

### Return type

[**BetaBuildUsagesV1MetricResponse**](BetaBuildUsagesV1MetricResponse.md)

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

<a id="buildsbetagroupscreatetomanyrelationship"></a>
# **BuildsBetaGroupsCreateToManyRelationship**
> void BuildsBetaGroupsCreateToManyRelationship (string id, BuildBetaGroupsLinkagesRequest buildBetaGroupsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaGroupsLinkagesRequest** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md) | List of related linkages |  |

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

<a id="buildsbetagroupsdeletetomanyrelationship"></a>
# **BuildsBetaGroupsDeleteToManyRelationship**
> void BuildsBetaGroupsDeleteToManyRelationship (string id, BuildBetaGroupsLinkagesRequest buildBetaGroupsLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildBetaGroupsLinkagesRequest** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md) | List of related linkages |  |

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

<a id="buildsbuildbetadetailgettoonerelated"></a>
# **BuildsBuildBetaDetailGetToOneRelated**
> BuildBetaDetailResponse BuildsBuildBetaDetailGetToOneRelated (string id, List<string> fieldsBuildBetaDetails = null, List<string> fieldsBuilds = null, List<string> include = null)




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

<a id="buildsbuildbetadetailgettoonerelationship"></a>
# **BuildsBuildBetaDetailGetToOneRelationship**
> BuildBuildBetaDetailLinkageResponse BuildsBuildBetaDetailGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildBuildBetaDetailLinkageResponse**](BuildBuildBetaDetailLinkageResponse.md)

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

<a id="buildsdiagnosticsignaturesgettomanyrelated"></a>
# **BuildsDiagnosticSignaturesGetToManyRelated**
> DiagnosticSignaturesResponse BuildsDiagnosticSignaturesGetToManyRelated (string id, List<string> filterDiagnosticType = null, List<string> fieldsDiagnosticSignatures = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterDiagnosticType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;diagnosticType&#39; | [optional]  |
| **fieldsDiagnosticSignatures** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type diagnosticSignatures | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**DiagnosticSignaturesResponse**](DiagnosticSignaturesResponse.md)

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
| **200** | List of DiagnosticSignatures |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsdiagnosticsignaturesgettomanyrelationship"></a>
# **BuildsDiagnosticSignaturesGetToManyRelationship**
> BuildDiagnosticSignaturesLinkagesResponse BuildsDiagnosticSignaturesGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildDiagnosticSignaturesLinkagesResponse**](BuildDiagnosticSignaturesLinkagesResponse.md)

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

<a id="buildsgetcollection"></a>
# **BuildsGetCollection**
> BuildsResponse BuildsGetCollection (List<string> filterVersion = null, List<string> filterExpired = null, List<string> filterProcessingState = null, List<string> filterBetaAppReviewSubmissionBetaReviewState = null, List<string> filterUsesNonExemptEncryption = null, List<string> filterPreReleaseVersionVersion = null, List<string> filterPreReleaseVersionPlatform = null, List<string> filterBuildAudienceType = null, List<string> filterPreReleaseVersion = null, List<string> filterApp = null, List<string> filterBetaGroups = null, List<string> filterAppStoreVersion = null, List<string> filterId = null, bool existsUsesNonExemptEncryption = null, List<string> sort = null, List<string> fieldsBuilds = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsApps = null, List<string> fieldsBuildBetaDetails = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsBuildIcons = null, int limit = null, List<string> include = null, int limitBetaBuildLocalizations = null, int limitBetaGroups = null, int limitBuildBundles = null, int limitIcons = null, int limitIndividualTesters = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **filterVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;version&#39; | [optional]  |
| **filterExpired** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;expired&#39; | [optional]  |
| **filterProcessingState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;processingState&#39; | [optional]  |
| **filterBetaAppReviewSubmissionBetaReviewState** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;betaAppReviewSubmission.betaReviewState&#39; | [optional]  |
| **filterUsesNonExemptEncryption** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **filterPreReleaseVersionVersion** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;preReleaseVersion.version&#39; | [optional]  |
| **filterPreReleaseVersionPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;preReleaseVersion.platform&#39; | [optional]  |
| **filterBuildAudienceType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;buildAudienceType&#39; | [optional]  |
| **filterPreReleaseVersion** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;preReleaseVersion&#39; | [optional]  |
| **filterApp** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;app&#39; | [optional]  |
| **filterBetaGroups** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;betaGroups&#39; | [optional]  |
| **filterAppStoreVersion** | [**List&lt;string&gt;**](string.md) | filter by id(s) of related &#39;appStoreVersion&#39; | [optional]  |
| **filterId** | [**List&lt;string&gt;**](string.md) | filter by id(s) | [optional]  |
| **existsUsesNonExemptEncryption** | **bool** | filter by attribute &#39;usesNonExemptEncryption&#39; | [optional]  |
| **sort** | [**List&lt;string&gt;**](string.md) | comma-separated list of sort expressions; resources will be sorted as specified | [optional]  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaBuildLocalizations** | **int** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int** | maximum number of related buildBundles returned (when they are included) | [optional]  |
| **limitIcons** | **int** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitIndividualTesters** | **int** | maximum number of related individualTesters returned (when they are included) | [optional]  |

### Return type

[**BuildsResponse**](BuildsResponse.md)

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
| **200** | List of Builds |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsgetinstance"></a>
# **BuildsGetInstance**
> BuildResponse BuildsGetInstance (string id, List<string> fieldsBuilds = null, List<string> fieldsPreReleaseVersions = null, List<string> fieldsBetaTesters = null, List<string> fieldsBetaBuildLocalizations = null, List<string> fieldsAppEncryptionDeclarations = null, List<string> fieldsBetaAppReviewSubmissions = null, List<string> fieldsApps = null, List<string> fieldsBuildBetaDetails = null, List<string> fieldsAppStoreVersions = null, List<string> fieldsBuildIcons = null, List<string> include = null, int limitBetaBuildLocalizations = null, int limitBetaGroups = null, int limitBuildBundles = null, int limitIcons = null, int limitIndividualTesters = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuilds** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type builds | [optional]  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |
| **fieldsBetaTesters** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaTesters | [optional]  |
| **fieldsBetaBuildLocalizations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaBuildLocalizations | [optional]  |
| **fieldsAppEncryptionDeclarations** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appEncryptionDeclarations | [optional]  |
| **fieldsBetaAppReviewSubmissions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaAppReviewSubmissions | [optional]  |
| **fieldsApps** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type apps | [optional]  |
| **fieldsBuildBetaDetails** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildBetaDetails | [optional]  |
| **fieldsAppStoreVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type appStoreVersions | [optional]  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **include** | [**List&lt;string&gt;**](string.md) | comma-separated list of relationships to include | [optional]  |
| **limitBetaBuildLocalizations** | **int** | maximum number of related betaBuildLocalizations returned (when they are included) | [optional]  |
| **limitBetaGroups** | **int** | maximum number of related betaGroups returned (when they are included) | [optional]  |
| **limitBuildBundles** | **int** | maximum number of related buildBundles returned (when they are included) | [optional]  |
| **limitIcons** | **int** | maximum number of related icons returned (when they are included) | [optional]  |
| **limitIndividualTesters** | **int** | maximum number of related individualTesters returned (when they are included) | [optional]  |

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

<a id="buildsiconsgettomanyrelated"></a>
# **BuildsIconsGetToManyRelated**
> BuildIconsWithoutIncludesResponse BuildsIconsGetToManyRelated (string id, List<string> fieldsBuildIcons = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsBuildIcons** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type buildIcons | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildIconsWithoutIncludesResponse**](BuildIconsWithoutIncludesResponse.md)

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
| **200** | List of BuildIcons with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsiconsgettomanyrelationship"></a>
# **BuildsIconsGetToManyRelationship**
> BuildIconsLinkagesResponse BuildsIconsGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildIconsLinkagesResponse**](BuildIconsLinkagesResponse.md)

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

<a id="buildsindividualtesterscreatetomanyrelationship"></a>
# **BuildsIndividualTestersCreateToManyRelationship**
> void BuildsIndividualTestersCreateToManyRelationship (string id, BuildIndividualTestersLinkagesRequest buildIndividualTestersLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildIndividualTestersLinkagesRequest** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="buildsindividualtestersdeletetomanyrelationship"></a>
# **BuildsIndividualTestersDeleteToManyRelationship**
> void BuildsIndividualTestersDeleteToManyRelationship (string id, BuildIndividualTestersLinkagesRequest buildIndividualTestersLinkagesRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildIndividualTestersLinkagesRequest** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md) | List of related linkages |  |

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

<a id="buildsindividualtestersgettomanyrelated"></a>
# **BuildsIndividualTestersGetToManyRelated**
> BetaTestersWithoutIncludesResponse BuildsIndividualTestersGetToManyRelated (string id, List<string> fieldsBetaTesters = null, int limit = null)




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

<a id="buildsindividualtestersgettomanyrelationship"></a>
# **BuildsIndividualTestersGetToManyRelationship**
> BuildIndividualTestersLinkagesResponse BuildsIndividualTestersGetToManyRelationship (string id, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BuildIndividualTestersLinkagesResponse**](BuildIndividualTestersLinkagesResponse.md)

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

<a id="buildsperfpowermetricsgettomanyrelated"></a>
# **BuildsPerfPowerMetricsGetToManyRelated**
> XcodeMetrics BuildsPerfPowerMetricsGetToManyRelated (string id, List<string> filterPlatform = null, List<string> filterMetricType = null, List<string> filterDeviceType = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **filterPlatform** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;platform&#39; | [optional]  |
| **filterMetricType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;metricType&#39; | [optional]  |
| **filterDeviceType** | [**List&lt;string&gt;**](string.md) | filter by attribute &#39;deviceType&#39; | [optional]  |

### Return type

[**XcodeMetrics**](XcodeMetrics.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/vnd.apple.xcode-metrics+json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **400** | Parameter error(s) |  -  |
| **401** | Unauthorized error(s) |  -  |
| **403** | Forbidden error |  -  |
| **404** | Not found error |  -  |
| **200** | List of PerfPowerMetrics |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsprereleaseversiongettoonerelated"></a>
# **BuildsPreReleaseVersionGetToOneRelated**
> PrereleaseVersionWithoutIncludesResponse BuildsPreReleaseVersionGetToOneRelated (string id, List<string> fieldsPreReleaseVersions = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **fieldsPreReleaseVersions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type preReleaseVersions | [optional]  |

### Return type

[**PrereleaseVersionWithoutIncludesResponse**](PrereleaseVersionWithoutIncludesResponse.md)

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
| **200** | Single PrereleaseVersion with get |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="buildsprereleaseversiongettoonerelationship"></a>
# **BuildsPreReleaseVersionGetToOneRelationship**
> BuildPreReleaseVersionLinkageResponse BuildsPreReleaseVersionGetToOneRelationship (string id)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |

### Return type

[**BuildPreReleaseVersionLinkageResponse**](BuildPreReleaseVersionLinkageResponse.md)

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

<a id="buildsupdateinstance"></a>
# **BuildsUpdateInstance**
> BuildResponse BuildsUpdateInstance (string id, BuildUpdateRequest buildUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **buildUpdateRequest** | [**BuildUpdateRequest**](BuildUpdateRequest.md) | Build representation |  |

### Return type

[**BuildResponse**](BuildResponse.md)

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
| **200** | Single Build |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

