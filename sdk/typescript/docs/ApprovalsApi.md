# ApprovalsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**approvalServiceGetApprovalSummary**](#approvalservicegetapprovalsummary) | **GET** /v2/approvals/{id} | Get approval summary|
|[**approvalServiceListApprovalSummaries**](#approvalservicelistapprovalsummaries) | **GET** /v2/approvals | List approval summaries|
|[**approvalServiceUpdateApproval**](#approvalserviceupdateapproval) | **PUT** /v2/approvals/{id} | Update approval summary|

# **approvalServiceGetApprovalSummary**
> Approvalv2ApprovalSummary approvalServiceGetApprovalSummary()

Returns a specific approval summary for the current user

### Example

```typescript
import {
    ApprovalsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApprovalsApi(configuration);

let id: string; //The approval summary ID (default to undefined)

const { status, data } = await apiInstance.approvalServiceGetApprovalSummary(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The approval summary ID | defaults to undefined|


### Return type

**Approvalv2ApprovalSummary**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approvalServiceListApprovalSummaries**
> Array<Approvalv2ApprovalSummary> approvalServiceListApprovalSummaries()

Returns the list of approval summaries for the current user

### Example

```typescript
import {
    ApprovalsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApprovalsApi(configuration);

let status: 'PROCESSING' | 'APPROVED' | 'REJECTED'; //The approval status (optional) (default to undefined)

const { status, data } = await apiInstance.approvalServiceListApprovalSummaries(
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **status** | [**&#39;PROCESSING&#39; | &#39;APPROVED&#39; | &#39;REJECTED&#39;**]**Array<&#39;PROCESSING&#39; &#124; &#39;APPROVED&#39; &#124; &#39;REJECTED&#39;>** | The approval status | (optional) defaults to undefined|


### Return type

**Array<Approvalv2ApprovalSummary>**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approvalServiceUpdateApproval**
> Approvalv2ApprovalSummary approvalServiceUpdateApproval(approvalServiceUpdateApprovalRequest)

Update the approval summary to either approve or reject the request

### Example

```typescript
import {
    ApprovalsApi,
    Configuration,
    ApprovalServiceUpdateApprovalRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApprovalsApi(configuration);

let id: string; //The approval ID (default to undefined)
let approvalServiceUpdateApprovalRequest: ApprovalServiceUpdateApprovalRequest; //

const { status, data } = await apiInstance.approvalServiceUpdateApproval(
    id,
    approvalServiceUpdateApprovalRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **approvalServiceUpdateApprovalRequest** | **ApprovalServiceUpdateApprovalRequest**|  | |
| **id** | [**string**] | The approval ID | defaults to undefined|


### Return type

**Approvalv2ApprovalSummary**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

