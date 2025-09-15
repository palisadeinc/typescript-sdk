# SweepInstancesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sweepServiceListSweepInstances**](#sweepservicelistsweepinstances) | **GET** /v2/workflows/sweep/{sweepConfigurationId}/instances | List sweep instances|
|[**sweepServiceSweepInstanceByID**](#sweepservicesweepinstancebyid) | **GET** /v2/workflows/sweep/instances/{id} | Get sweep instance by ID|

# **sweepServiceListSweepInstances**
> V2ListSweepInstancesResponse sweepServiceListSweepInstances()

List sweep instances for a sweep configuration

### Example

```typescript
import {
    SweepInstancesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepInstancesApi(configuration);

let sweepConfigurationId: string; //The ID of the sweep configuration to list instances for (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 100) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.sweepServiceListSweepInstances(
    sweepConfigurationId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sweepConfigurationId** | [**string**] | The ID of the sweep configuration to list instances for | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 100) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListSweepInstancesResponse**

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

# **sweepServiceSweepInstanceByID**
> V2SweepInstance sweepServiceSweepInstanceByID()

Get a single sweep instance by its ID

### Example

```typescript
import {
    SweepInstancesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepInstancesApi(configuration);

let id: string; //The ID of the sweep instance (default to undefined)

const { status, data } = await apiInstance.sweepServiceSweepInstanceByID(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep instance | defaults to undefined|


### Return type

**V2SweepInstance**

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

