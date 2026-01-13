# AppStoreConnect.Net.Api.BetaRecruitmentCriterionOptionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BetaRecruitmentCriterionOptionsGetCollection**](BetaRecruitmentCriterionOptionsApi.md#betarecruitmentcriterionoptionsgetcollection) | **GET** /v1/betaRecruitmentCriterionOptions |  |

<a id="betarecruitmentcriterionoptionsgetcollection"></a>
# **BetaRecruitmentCriterionOptionsGetCollection**
> BetaRecruitmentCriterionOptionsResponse BetaRecruitmentCriterionOptionsGetCollection (List<string> fieldsBetaRecruitmentCriterionOptions = null, int limit = null)




### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **fieldsBetaRecruitmentCriterionOptions** | [**List&lt;string&gt;**](string.md) | the fields to include for returned resources of type betaRecruitmentCriterionOptions | [optional]  |
| **limit** | **int** | maximum resources per page | [optional]  |

### Return type

[**BetaRecruitmentCriterionOptionsResponse**](BetaRecruitmentCriterionOptionsResponse.md)

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
| **200** | List of BetaRecruitmentCriterionOptions |  -  |
| **429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

