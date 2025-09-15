# MPCMembershipsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**mpcServiceListMembershipsForDevice**](#mpcservicelistmembershipsfordevice) | **GET** /v2/mpc/device/memberships | List memberships for device|
|[**mpcServiceListMembershipsForQuorum**](#mpcservicelistmembershipsforquorum) | **GET** /v2/mpc/memberships/{quorumId} | List memberships for quorum|

# **mpcServiceListMembershipsForDevice**
> Array<V2Membership> mpcServiceListMembershipsForDevice()

List memberships for device

### Example

```typescript
import {
    MPCMembershipsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCMembershipsApi(configuration);

const { status, data } = await apiInstance.mpcServiceListMembershipsForDevice();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2Membership>**

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

# **mpcServiceListMembershipsForQuorum**
> Array<V2Membership> mpcServiceListMembershipsForQuorum()

List memberships for quorum

### Example

```typescript
import {
    MPCMembershipsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCMembershipsApi(configuration);

let quorumId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceListMembershipsForQuorum(
    quorumId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**Array<V2Membership>**

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

