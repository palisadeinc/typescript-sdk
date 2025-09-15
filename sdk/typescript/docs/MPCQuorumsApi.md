# MPCQuorumsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**mpcServiceCreateQuorum**](#mpcservicecreatequorum) | **POST** /v2/mpc/quorums | Create a new quorum|
|[**mpcServiceDeleteQuorum**](#mpcservicedeletequorum) | **DELETE** /v2/mpc/quorums/{quorumId} | Delete a quorum|
|[**mpcServiceGetQuorum**](#mpcservicegetquorum) | **GET** /v2/mpc/quorums/{quorumId} | Get a quorum|
|[**mpcServiceListEligibleDevices**](#mpcservicelisteligibledevices) | **GET** /v2/mpc/eligible | List eligible devices|
|[**mpcServiceListQuorums**](#mpcservicelistquorums) | **GET** /v2/mpc/quorums | List quorums|
|[**mpcServiceListQuorumsByDevice**](#mpcservicelistquorumsbydevice) | **GET** /v2/mpc/quorums/self | List quorums|
|[**mpcServiceModifyQuorum**](#mpcservicemodifyquorum) | **PATCH** /v2/mpc/quorums/{quorumId} | Modify an existing quorum|
|[**mpcServicePollQuorumStatus**](#mpcservicepollquorumstatus) | **GET** /v2/mpc/quorums/{quorumId}/status | Poll quorum status|

# **mpcServiceCreateQuorum**
> V2Quorum mpcServiceCreateQuorum(v2CreateQuorumRequest)

Create a new quorum

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration,
    V2CreateQuorumRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let v2CreateQuorumRequest: V2CreateQuorumRequest; //

const { status, data } = await apiInstance.mpcServiceCreateQuorum(
    v2CreateQuorumRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateQuorumRequest** | **V2CreateQuorumRequest**|  | |


### Return type

**V2Quorum**

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

# **mpcServiceDeleteQuorum**
> V2Quorum mpcServiceDeleteQuorum()

Delete a quorum

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let quorumId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceDeleteQuorum(
    quorumId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**V2Quorum**

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

# **mpcServiceGetQuorum**
> V2Quorum mpcServiceGetQuorum()

Get a quorum

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let quorumId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceGetQuorum(
    quorumId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**V2Quorum**

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

# **mpcServiceListEligibleDevices**
> Array<V2EligibleDevice> mpcServiceListEligibleDevices()

List eligible devices

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let deviceType: 'MOBILE' | 'CLOUD'; // (default to undefined)

const { status, data } = await apiInstance.mpcServiceListEligibleDevices(
    deviceType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceType** | [**&#39;MOBILE&#39; | &#39;CLOUD&#39;**]**Array<&#39;MOBILE&#39; &#124; &#39;CLOUD&#39;>** |  | defaults to undefined|


### Return type

**Array<V2EligibleDevice>**

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

# **mpcServiceListQuorums**
> Array<V2Quorum> mpcServiceListQuorums()

List quorums with the client JWT

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

const { status, data } = await apiInstance.mpcServiceListQuorums();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2Quorum>**

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

# **mpcServiceListQuorumsByDevice**
> Array<V2Quorum> mpcServiceListQuorumsByDevice()

List quorums with the device JWT

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

const { status, data } = await apiInstance.mpcServiceListQuorumsByDevice();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2Quorum>**

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

# **mpcServiceModifyQuorum**
> V2Quorum mpcServiceModifyQuorum(mpcServiceModifyQuorumRequest)

Modify an existing quorum

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration,
    MpcServiceModifyQuorumRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let quorumId: string; // (default to undefined)
let mpcServiceModifyQuorumRequest: MpcServiceModifyQuorumRequest; //

const { status, data } = await apiInstance.mpcServiceModifyQuorum(
    quorumId,
    mpcServiceModifyQuorumRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mpcServiceModifyQuorumRequest** | **MpcServiceModifyQuorumRequest**|  | |
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**V2Quorum**

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

# **mpcServicePollQuorumStatus**
> V2QuorumStatus mpcServicePollQuorumStatus()

Poll quorum status

### Example

```typescript
import {
    MPCQuorumsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new MPCQuorumsApi(configuration);

let quorumId: string; // (default to undefined)

const { status, data } = await apiInstance.mpcServicePollQuorumStatus(
    quorumId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **quorumId** | [**string**] |  | defaults to undefined|


### Return type

**V2QuorumStatus**

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

