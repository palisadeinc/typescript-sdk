# DevicesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deviceServiceAddDeviceMetadata**](#deviceserviceadddevicemetadata) | **POST** /v2/devices/metadata | Add device metadata|
|[**deviceServiceCreateDevice**](#deviceservicecreatedevice) | **POST** /v2/devices | Create a new device|
|[**deviceServiceDeleteDevice**](#deviceservicedeletedevice) | **DELETE** /v2/devices/{id} | Delete a device|
|[**deviceServiceGetDevice**](#deviceservicegetdevice) | **GET** /v2/devices/{id} | Get a device|
|[**deviceServiceGetDeviceCredentials**](#deviceservicegetdevicecredentials) | **GET** /v2/devices/credentials | Get device credentials|
|[**deviceServiceGetDevicePairingCredentials**](#deviceservicegetdevicepairingcredentials) | **GET** /v2/devices/{id}/pairing-credentials | Get device pairing credentials|
|[**deviceServiceGetPushToken**](#deviceservicegetpushtoken) | **GET** /v2/devices/push-token | Get push notification token|
|[**deviceServiceGetSelf**](#deviceservicegetself) | **GET** /v2/devices/self | Get device|
|[**deviceServiceListDevices**](#deviceservicelistdevices) | **GET** /v2/devices | List all devices|
|[**deviceServicePairDeviceWithCredential**](#deviceservicepairdevicewithcredential) | **POST** /v2/devices/pair-with-credential | Pair a device with an organization|
|[**deviceServiceSetDeviceVersion**](#deviceservicesetdeviceversion) | **POST** /v2/devices/version | Set device version|
|[**deviceServiceTrustOrganization**](#deviceservicetrustorganization) | **POST** /v2/devices/{id}/trust-organization | Trust organization|
|[**deviceServiceUpdateDeviceApprovalStatus**](#deviceserviceupdatedeviceapprovalstatus) | **PUT** /v2/devices/{id}/approval-status | Update device approval status|
|[**deviceServiceUpdateDeviceDisplayName**](#deviceserviceupdatedevicedisplayname) | **PUT** /v2/devices/{id}/display-name | Update device display name|
|[**deviceServiceUpdateDeviceEnabledStatus**](#deviceserviceupdatedeviceenabledstatus) | **PUT** /v2/devices/{id}/enabled-status | Update device enabled status|

# **deviceServiceAddDeviceMetadata**
> object deviceServiceAddDeviceMetadata(v2AddDeviceMetadataRequest)

Add key/value metadata to the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    V2AddDeviceMetadataRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let v2AddDeviceMetadataRequest: V2AddDeviceMetadataRequest; //

const { status, data } = await apiInstance.deviceServiceAddDeviceMetadata(
    v2AddDeviceMetadataRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2AddDeviceMetadataRequest** | **V2AddDeviceMetadataRequest**|  | |


### Return type

**object**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **deviceServiceCreateDevice**
> V2Device deviceServiceCreateDevice(v2CreateDeviceRequest)

Create a new device in your organization ready to pair with a physical device

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    V2CreateDeviceRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let v2CreateDeviceRequest: V2CreateDeviceRequest; //

const { status, data } = await apiInstance.deviceServiceCreateDevice(
    v2CreateDeviceRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateDeviceRequest** | **V2CreateDeviceRequest**|  | |


### Return type

**V2Device**

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

# **deviceServiceDeleteDevice**
> V2Device deviceServiceDeleteDevice()

Delete a specific device by ID. This action can only be performed for unapproved devices at this time.

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)

const { status, data } = await apiInstance.deviceServiceDeleteDevice(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2Device**

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

# **deviceServiceGetDevice**
> V2Device deviceServiceGetDevice()

Get a specific device by ID

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)

const { status, data } = await apiInstance.deviceServiceGetDevice(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2Device**

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

# **deviceServiceGetDeviceCredentials**
> V2GetDeviceCredentialsResponse deviceServiceGetDeviceCredentials()

Get device credentials for the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

const { status, data } = await apiInstance.deviceServiceGetDeviceCredentials();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2GetDeviceCredentialsResponse**

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

# **deviceServiceGetDevicePairingCredentials**
> V2PairingCredentials deviceServiceGetDevicePairingCredentials()

Get a new set of pairing credentials for a device by ID

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)

const { status, data } = await apiInstance.deviceServiceGetDevicePairingCredentials(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2PairingCredentials**

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

# **deviceServiceGetPushToken**
> V2GetPushTokenResponse deviceServiceGetPushToken()

Get a new push notification token for the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

const { status, data } = await apiInstance.deviceServiceGetPushToken();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2GetPushTokenResponse**

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

# **deviceServiceGetSelf**
> V2Device deviceServiceGetSelf()

Get the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

const { status, data } = await apiInstance.deviceServiceGetSelf();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2Device**

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

# **deviceServiceListDevices**
> Array<V2Device> deviceServiceListDevices()

List all devices associated with a user or organization

### Example

```typescript
import {
    DevicesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let deviceType: 'MOBILE' | 'CLOUD'; //The device type (default to undefined)
let deviceOwner: 'THIS_ORGANIZATION' | 'TRUSTED_ORGANIZATION'; //The device owner (optional) (default to undefined)

const { status, data } = await apiInstance.deviceServiceListDevices(
    deviceType,
    deviceOwner
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceType** | [**&#39;MOBILE&#39; | &#39;CLOUD&#39;**]**Array<&#39;MOBILE&#39; &#124; &#39;CLOUD&#39;>** | The device type | defaults to undefined|
| **deviceOwner** | [**&#39;THIS_ORGANIZATION&#39; | &#39;TRUSTED_ORGANIZATION&#39;**]**Array<&#39;THIS_ORGANIZATION&#39; &#124; &#39;TRUSTED_ORGANIZATION&#39;>** | The device owner | (optional) defaults to undefined|


### Return type

**Array<V2Device>**

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

# **deviceServicePairDeviceWithCredential**
> V2Device deviceServicePairDeviceWithCredential(v2PairDeviceWithCredentialRequest)

Pair the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    V2PairDeviceWithCredentialRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let v2PairDeviceWithCredentialRequest: V2PairDeviceWithCredentialRequest; //

const { status, data } = await apiInstance.deviceServicePairDeviceWithCredential(
    v2PairDeviceWithCredentialRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2PairDeviceWithCredentialRequest** | **V2PairDeviceWithCredentialRequest**|  | |


### Return type

**V2Device**

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

# **deviceServiceSetDeviceVersion**
> object deviceServiceSetDeviceVersion(v2SetDeviceVersionRequest)

Set the version of the device specified in the JWT

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    V2SetDeviceVersionRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let v2SetDeviceVersionRequest: V2SetDeviceVersionRequest; //

const { status, data } = await apiInstance.deviceServiceSetDeviceVersion(
    v2SetDeviceVersionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2SetDeviceVersionRequest** | **V2SetDeviceVersionRequest**|  | |


### Return type

**object**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **deviceServiceTrustOrganization**
> V2TrustedOrganization deviceServiceTrustOrganization(deviceServiceTrustOrganizationRequest)

Trust a new organization to use this device in it\'s controls

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    DeviceServiceTrustOrganizationRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)
let deviceServiceTrustOrganizationRequest: DeviceServiceTrustOrganizationRequest; //

const { status, data } = await apiInstance.deviceServiceTrustOrganization(
    id,
    deviceServiceTrustOrganizationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceServiceTrustOrganizationRequest** | **DeviceServiceTrustOrganizationRequest**|  | |
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2TrustedOrganization**

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

# **deviceServiceUpdateDeviceApprovalStatus**
> V2Device deviceServiceUpdateDeviceApprovalStatus(deviceServiceUpdateDeviceApprovalStatusRequest)

Update the approval status of a device by ID

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    DeviceServiceUpdateDeviceApprovalStatusRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)
let deviceServiceUpdateDeviceApprovalStatusRequest: DeviceServiceUpdateDeviceApprovalStatusRequest; //

const { status, data } = await apiInstance.deviceServiceUpdateDeviceApprovalStatus(
    id,
    deviceServiceUpdateDeviceApprovalStatusRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceServiceUpdateDeviceApprovalStatusRequest** | **DeviceServiceUpdateDeviceApprovalStatusRequest**|  | |
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2Device**

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

# **deviceServiceUpdateDeviceDisplayName**
> V2Device deviceServiceUpdateDeviceDisplayName(deviceServiceUpdateDeviceDisplayNameRequest)

Update the display name of a device by ID

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    DeviceServiceUpdateDeviceDisplayNameRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)
let deviceServiceUpdateDeviceDisplayNameRequest: DeviceServiceUpdateDeviceDisplayNameRequest; //

const { status, data } = await apiInstance.deviceServiceUpdateDeviceDisplayName(
    id,
    deviceServiceUpdateDeviceDisplayNameRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceServiceUpdateDeviceDisplayNameRequest** | **DeviceServiceUpdateDeviceDisplayNameRequest**|  | |
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2Device**

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

# **deviceServiceUpdateDeviceEnabledStatus**
> V2Device deviceServiceUpdateDeviceEnabledStatus(deviceServiceUpdateDeviceEnabledStatusRequest)

Update the enabled status of a device by ID

### Example

```typescript
import {
    DevicesApi,
    Configuration,
    DeviceServiceUpdateDeviceEnabledStatusRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new DevicesApi(configuration);

let id: string; //The device ID (default to undefined)
let deviceServiceUpdateDeviceEnabledStatusRequest: DeviceServiceUpdateDeviceEnabledStatusRequest; //

const { status, data } = await apiInstance.deviceServiceUpdateDeviceEnabledStatus(
    id,
    deviceServiceUpdateDeviceEnabledStatusRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceServiceUpdateDeviceEnabledStatusRequest** | **DeviceServiceUpdateDeviceEnabledStatusRequest**|  | |
| **id** | [**string**] | The device ID | defaults to undefined|


### Return type

**V2Device**

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

