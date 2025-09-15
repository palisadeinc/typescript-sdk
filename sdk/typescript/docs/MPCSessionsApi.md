# MPCSessionsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**mpcServiceGetDeviceSessionData**](#mpcservicegetdevicesessiondata) | **GET** /v2/mpc/device/sessions/{sessionId}/data | Get device session data|
|[**mpcServiceGetSession**](#mpcservicegetsession) | **GET** /v2/mpc/device/sessions/{sessionId} | Get session|
|[**mpcServiceListSessionSets**](#mpcservicelistsessionsets) | **GET** /v2/mpc/sessions/{quorumId} | List session sets|
|[**mpcServiceListSessionsForDevice**](#mpcservicelistsessionsfordevice) | **GET** /v2/mpc/device/sessions | List sessions for device|
|[**mpcServicePollSessionSetStatus**](#mpcservicepollsessionsetstatus) | **GET** /v2/mpc/sessions/{sessionSetId}/status | Poll session set status|
|[**mpcServiceSubmitSession**](#mpcservicesubmitsession) | **PATCH** /v2/mpc/device/{sessionId} | Submit session|

# **mpcServiceGetDeviceSessionData**
> V2GetDeviceSessionDataResponse mpcServiceGetDeviceSessionData()

Get device session data

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let sessionId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceGetDeviceSessionData(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**V2GetDeviceSessionDataResponse**

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

# **mpcServiceGetSession**
> V2Session mpcServiceGetSession()

Get session

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let sessionId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceGetSession(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**V2Session**

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

# **mpcServiceListSessionSets**
> Array<V2SessionSet> mpcServiceListSessionSets()

List session sets

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let quorumId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceListSessionSets(
    quorumId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**Array<V2SessionSet>**

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

# **mpcServiceListSessionsForDevice**
> Array<V2Session> mpcServiceListSessionsForDevice()

List sessions for device

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let stateFilter: 'SESSION_STATE_CREATED' | 'SESSION_STATE_PENDING' | 'SESSION_STATE_SUBMITTED' | 'SESSION_STATE_COMPLETED' | 'SESSION_STATE_TIMED_OUT' | 'SESSION_STATE_FAILED' | 'SESSION_STATE_PROCESSED' | 'SESSION_STATE_SUPER' | 'SESSION_STATE_INITIAL'; // - SESSION_STATE_SUBMITTED: Session has completed & submitted data from this device  - SESSION_STATE_COMPLETED: Session has completed but this device did not submit data  - SESSION_STATE_SUPER: FSM USE ONLY: Super state  - SESSION_STATE_INITIAL: FSM USE ONLY: Initial state (default to undefined)

const { status, data } = await apiInstance.mpcServiceListSessionsForDevice(
    stateFilter
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **stateFilter** | [**&#39;SESSION_STATE_CREATED&#39; | &#39;SESSION_STATE_PENDING&#39; | &#39;SESSION_STATE_SUBMITTED&#39; | &#39;SESSION_STATE_COMPLETED&#39; | &#39;SESSION_STATE_TIMED_OUT&#39; | &#39;SESSION_STATE_FAILED&#39; | &#39;SESSION_STATE_PROCESSED&#39; | &#39;SESSION_STATE_SUPER&#39; | &#39;SESSION_STATE_INITIAL&#39;**]**Array<&#39;SESSION_STATE_CREATED&#39; &#124; &#39;SESSION_STATE_PENDING&#39; &#124; &#39;SESSION_STATE_SUBMITTED&#39; &#124; &#39;SESSION_STATE_COMPLETED&#39; &#124; &#39;SESSION_STATE_TIMED_OUT&#39; &#124; &#39;SESSION_STATE_FAILED&#39; &#124; &#39;SESSION_STATE_PROCESSED&#39; &#124; &#39;SESSION_STATE_SUPER&#39; &#124; &#39;SESSION_STATE_INITIAL&#39;>** |  - SESSION_STATE_SUBMITTED: Session has completed &amp; submitted data from this device  - SESSION_STATE_COMPLETED: Session has completed but this device did not submit data  - SESSION_STATE_SUPER: FSM USE ONLY: Super state  - SESSION_STATE_INITIAL: FSM USE ONLY: Initial state | defaults to undefined|


### Return type

**Array<V2Session>**

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

# **mpcServicePollSessionSetStatus**
> V2SessionSetStatus mpcServicePollSessionSetStatus()

Poll session set status

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let sessionSetId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServicePollSessionSetStatus(
    sessionSetId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionSetId** | [**string**] |  | defaults to undefined|


### Return type

**V2SessionSetStatus**

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

# **mpcServiceSubmitSession**
> V2Session mpcServiceSubmitSession(sESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018)

Submit session

### Example

```typescript
import {
    MPCSessionsApi,
    Configuration,
    SESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCSessionsApi(configuration);

let sessionId: string; // (default to undefined)
let sESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018: SESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018; //

const { status, data } = await apiInstance.mpcServiceSubmitSession(
    sessionId,
    sESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018** | **SESSIONSubmitSessionTODOWeShouldCheckTheDeviceIDFromTheJWTToEnsureUserASDeviceXDoesnTAccidentallySubmitOnBehalfOfDeviceYForTheSameUserHttpsPalisadeIncAtlassianNetBrowseENG1018**|  | |
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**V2Session**

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

