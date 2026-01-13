# AppStoreConnect.Net.Api.BetaRecruitmentCriteriaApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaRecruitmentCriteriaCreateInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriacreateinstance) | **POST** /v1/betaRecruitmentCriteria |  |
| [**BetaRecruitmentCriteriaDeleteInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriadeleteinstance) | **DELETE** /v1/betaRecruitmentCriteria/{id} |  |
| [**BetaRecruitmentCriteriaUpdateInstance**](BetaRecruitmentCriteriaApi.md#betarecruitmentcriteriaupdateinstance) | **PATCH** /v1/betaRecruitmentCriteria/{id} |  |

<a id="betarecruitmentcriteriacreateinstance"></a>
# **BetaRecruitmentCriteriaCreateInstance**
> BetaRecruitmentCriterionResponse BetaRecruitmentCriteriaCreateInstance (BetaRecruitmentCriterionCreateRequest betaRecruitmentCriterionCreateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **betaRecruitmentCriterionCreateRequest** | [**BetaRecruitmentCriterionCreateRequest**](BetaRecruitmentCriterionCreateRequest.md) | BetaRecruitmentCriterion representation |  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **201** | Single BetaRecruitmentCriterion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="betarecruitmentcriteriadeleteinstance"></a>
# **BetaRecruitmentCriteriaDeleteInstance**
> void BetaRecruitmentCriteriaDeleteInstance (string id)




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

<a id="betarecruitmentcriteriaupdateinstance"></a>
# **BetaRecruitmentCriteriaUpdateInstance**
> BetaRecruitmentCriterionResponse BetaRecruitmentCriteriaUpdateInstance (string id, BetaRecruitmentCriterionUpdateRequest betaRecruitmentCriterionUpdateRequest)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | the id of the requested resource |  |
| **betaRecruitmentCriterionUpdateRequest** | [**BetaRecruitmentCriterionUpdateRequest**](BetaRecruitmentCriterionUpdateRequest.md) | BetaRecruitmentCriterion representation |  |

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

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
| **200** | Single BetaRecruitmentCriterion |  -  |
| **409** | Request entity error(s) |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

