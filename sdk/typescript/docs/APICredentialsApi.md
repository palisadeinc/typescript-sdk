# APICredentialsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**credentialServiceCreateCredential**](#credentialservicecreatecredential) | **POST** /v2/credentials | Create credentials|
|[**credentialServiceDeleteCredential**](#credentialservicedeletecredential) | **DELETE** /v2/credentials/{id} | Delete credential|
|[**credentialServiceExchangeCredential**](#credentialserviceexchangecredential) | **POST** /v2/credentials/oauth/token | Client credentials exchange|
|[**credentialServiceGetCredential**](#credentialservicegetcredential) | **GET** /v2/credentials/{id} | Get credentials|
|[**credentialServiceGetCredentialInfo**](#credentialservicegetcredentialinfo) | **GET** /v2/credentials/{id}/info | Get credential info |
|[**credentialServiceListCredentialInfo**](#credentialservicelistcredentialinfo) | **GET** /v2/credentials/info | List all credential info|
|[**credentialServiceListCredentials**](#credentialservicelistcredentials) | **GET** /v2/credentials | List all credentials|
|[**credentialServiceListVariants**](#credentialservicelistvariants) | **GET** /v2/credentials/permissions | List available permissions|
|[**credentialServiceUpdateCredentialActiveStatus**](#credentialserviceupdatecredentialactivestatus) | **PUT** /v2/credentials/{id}/active | Update credential active status|
|[**credentialServiceUpdateCredentialPermissions**](#credentialserviceupdatecredentialpermissions) | **PUT** /v2/credentials/{id}/permissions | Update credential permissions|

# **credentialServiceCreateCredential**
> V2Credential credentialServiceCreateCredential(v2CreateCredentialRequest)

Create a set of API credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration,
    V2CreateCredentialRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let v2CreateCredentialRequest: V2CreateCredentialRequest; //

const { status, data } = await apiInstance.credentialServiceCreateCredential(
    v2CreateCredentialRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateCredentialRequest** | **V2CreateCredentialRequest**|  | |


### Return type

**V2Credential**

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

# **credentialServiceDeleteCredential**
> object credentialServiceDeleteCredential()

Delete a specific set of API credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let id: string; //The credential ID (default to undefined)

const { status, data } = await apiInstance.credentialServiceDeleteCredential(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The credential ID | defaults to undefined|


### Return type

**object**

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

# **credentialServiceExchangeCredential**
> V2ExchangeCredentialResponse credentialServiceExchangeCredential(v2ExchangeCredentialRequest)

OAuth client credentials exchange for access token

### Example

```typescript
import {
    APICredentialsApi,
    Configuration,
    V2ExchangeCredentialRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let v2ExchangeCredentialRequest: V2ExchangeCredentialRequest; //

const { status, data } = await apiInstance.credentialServiceExchangeCredential(
    v2ExchangeCredentialRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ExchangeCredentialRequest** | **V2ExchangeCredentialRequest**|  | |


### Return type

**V2ExchangeCredentialResponse**

### Authorization

No authorization required

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

# **credentialServiceGetCredential**
> V2Credential credentialServiceGetCredential()

Get a set of API credentials by ID

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let id: string; //The credential ID (default to undefined)

const { status, data } = await apiInstance.credentialServiceGetCredential(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The credential ID | defaults to undefined|


### Return type

**V2Credential**

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

# **credentialServiceGetCredentialInfo**
> V2CredentialInfo credentialServiceGetCredentialInfo()

Get a set of API credential info by ID

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let id: string; //The credential ID (default to undefined)

const { status, data } = await apiInstance.credentialServiceGetCredentialInfo(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The credential ID | defaults to undefined|


### Return type

**V2CredentialInfo**

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

# **credentialServiceListCredentialInfo**
> Array<V2CredentialInfo> credentialServiceListCredentialInfo()

List all credential info

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

const { status, data } = await apiInstance.credentialServiceListCredentialInfo();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2CredentialInfo>**

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

# **credentialServiceListCredentials**
> Array<V2Credential> credentialServiceListCredentials()

List all credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

const { status, data } = await apiInstance.credentialServiceListCredentials();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2Credential>**

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

# **credentialServiceListVariants**
> V2ListVariantsResponse credentialServiceListVariants()

List available permissions for the use with API credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

const { status, data } = await apiInstance.credentialServiceListVariants();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2ListVariantsResponse**

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

# **credentialServiceUpdateCredentialActiveStatus**
> V2Credential credentialServiceUpdateCredentialActiveStatus(credentialServiceUpdateCredentialActiveStatusRequest)

Update the active status on a specific set of API credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration,
    CredentialServiceUpdateCredentialActiveStatusRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let id: string; //The credential ID (default to undefined)
let credentialServiceUpdateCredentialActiveStatusRequest: CredentialServiceUpdateCredentialActiveStatusRequest; //

const { status, data } = await apiInstance.credentialServiceUpdateCredentialActiveStatus(
    id,
    credentialServiceUpdateCredentialActiveStatusRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **credentialServiceUpdateCredentialActiveStatusRequest** | **CredentialServiceUpdateCredentialActiveStatusRequest**|  | |
| **id** | [**string**] | The credential ID | defaults to undefined|


### Return type

**V2Credential**

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

# **credentialServiceUpdateCredentialPermissions**
> V2Credential credentialServiceUpdateCredentialPermissions(credentialServiceUpdateCredentialPermissionsRequest)

Update the permissions set on a specific set of API credentials

### Example

```typescript
import {
    APICredentialsApi,
    Configuration,
    CredentialServiceUpdateCredentialPermissionsRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new APICredentialsApi(configuration);

let id: string; //The credential ID (default to undefined)
let credentialServiceUpdateCredentialPermissionsRequest: CredentialServiceUpdateCredentialPermissionsRequest; //

const { status, data } = await apiInstance.credentialServiceUpdateCredentialPermissions(
    id,
    credentialServiceUpdateCredentialPermissionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **credentialServiceUpdateCredentialPermissionsRequest** | **CredentialServiceUpdateCredentialPermissionsRequest**|  | |
| **id** | [**string**] | The credential ID | defaults to undefined|


### Return type

**V2Credential**

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

