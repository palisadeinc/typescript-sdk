# ApproversApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**approvalServiceGetKeyApprovers**](#approvalservicegetkeyapprovers) | **GET** /v2/approvers/{id} | List wallet approvers|
|[**approvalServiceGetOrgApprovers**](#approvalservicegetorgapprovers) | **GET** /v2/approvers | List organization approvers|
|[**approvalServiceListEligibleApprovers**](#approvalservicelisteligibleapprovers) | **GET** /v2/approvers/eligible | List eligible approvers|
|[**approvalServiceUpdateKeyApprovers**](#approvalserviceupdatekeyapprovers) | **PUT** /v2/approvers/{id} | Update wallet approvers|
|[**approvalServiceUpdateOrgApprovers**](#approvalserviceupdateorgapprovers) | **PUT** /v2/approvers | Update organization approvers|

# **approvalServiceGetKeyApprovers**
> V2GetKeyApproversResponse approvalServiceGetKeyApprovers()

Returns the list of approvers within the approval set configured for the wallet and optionally source type

### Example

```typescript
import {
    ApproversApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApproversApi(configuration);

let id: string; //The wallet ID (default to undefined)
let sourceType: 'TRANSACTION' | 'DEVICE' | 'API_CREDENTIAL' | 'ALLOW_LIST_ENTRY' | 'POLICY' | 'USER' | 'APPROVAL_GROUP' | 'ADDRESS'; //The source type (optional) (default to undefined)

const { status, data } = await apiInstance.approvalServiceGetKeyApprovers(
    id,
    sourceType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The wallet ID | defaults to undefined|
| **sourceType** | [**&#39;TRANSACTION&#39; | &#39;DEVICE&#39; | &#39;API_CREDENTIAL&#39; | &#39;ALLOW_LIST_ENTRY&#39; | &#39;POLICY&#39; | &#39;USER&#39; | &#39;APPROVAL_GROUP&#39; | &#39;ADDRESS&#39;**]**Array<&#39;TRANSACTION&#39; &#124; &#39;DEVICE&#39; &#124; &#39;API_CREDENTIAL&#39; &#124; &#39;ALLOW_LIST_ENTRY&#39; &#124; &#39;POLICY&#39; &#124; &#39;USER&#39; &#124; &#39;APPROVAL_GROUP&#39; &#124; &#39;ADDRESS&#39;>** | The source type | (optional) defaults to undefined|


### Return type

**V2GetKeyApproversResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approvalServiceGetOrgApprovers**
> V2GetOrgApproversResponse approvalServiceGetOrgApprovers()

Returns the list of approvers within the approval set configured for the organization and optionally source type

### Example

```typescript
import {
    ApproversApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApproversApi(configuration);

let sourceType: 'TRANSACTION' | 'DEVICE' | 'API_CREDENTIAL' | 'ALLOW_LIST_ENTRY' | 'POLICY' | 'USER' | 'APPROVAL_GROUP' | 'ADDRESS'; //The source type (optional) (default to undefined)

const { status, data } = await apiInstance.approvalServiceGetOrgApprovers(
    sourceType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sourceType** | [**&#39;TRANSACTION&#39; | &#39;DEVICE&#39; | &#39;API_CREDENTIAL&#39; | &#39;ALLOW_LIST_ENTRY&#39; | &#39;POLICY&#39; | &#39;USER&#39; | &#39;APPROVAL_GROUP&#39; | &#39;ADDRESS&#39;**]**Array<&#39;TRANSACTION&#39; &#124; &#39;DEVICE&#39; &#124; &#39;API_CREDENTIAL&#39; &#124; &#39;ALLOW_LIST_ENTRY&#39; &#124; &#39;POLICY&#39; &#124; &#39;USER&#39; &#124; &#39;APPROVAL_GROUP&#39; &#124; &#39;ADDRESS&#39;>** | The source type | (optional) defaults to undefined|


### Return type

**V2GetOrgApproversResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **approvalServiceListEligibleApprovers**
> Array<V2EligibleApprover> approvalServiceListEligibleApprovers()

Returns the list of eligible approvers

### Example

```typescript
import {
    ApproversApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApproversApi(configuration);

const { status, data } = await apiInstance.approvalServiceListEligibleApprovers();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2EligibleApprover>**

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

# **approvalServiceUpdateKeyApprovers**
> V2ApprovalGroup approvalServiceUpdateKeyApprovers(v2ApprovalGroup)

Updates the list of approvers within the approval set configured for the wallet and source type

### Example

```typescript
import {
    ApproversApi,
    Configuration,
    V2ApprovalGroup
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApproversApi(configuration);

let id: string; //The wallet ID (default to undefined)
let v2ApprovalGroup: V2ApprovalGroup; //

const { status, data } = await apiInstance.approvalServiceUpdateKeyApprovers(
    id,
    v2ApprovalGroup
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ApprovalGroup** | **V2ApprovalGroup**|  | |
| **id** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**V2ApprovalGroup**

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

# **approvalServiceUpdateOrgApprovers**
> V2ApprovalGroup approvalServiceUpdateOrgApprovers(v2ApprovalGroup)

Updates the list of approvers within the approval set configured for the organization and source type

### Example

```typescript
import {
    ApproversApi,
    Configuration,
    V2ApprovalGroup
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ApproversApi(configuration);

let v2ApprovalGroup: V2ApprovalGroup; //

const { status, data } = await apiInstance.approvalServiceUpdateOrgApprovers(
    v2ApprovalGroup
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ApprovalGroup** | **V2ApprovalGroup**|  | |


### Return type

**V2ApprovalGroup**

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

