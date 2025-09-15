# WalletConnectApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**walletConnectServiceAcceptConnection**](#walletconnectserviceacceptconnection) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/connections/{id}/accept | Accept a wallet connect connection|
|[**walletConnectServiceCreateConnection**](#walletconnectservicecreateconnection) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/connections | Propose a new wallet connect connection|
|[**walletConnectServiceDisconnectConnection**](#walletconnectservicedisconnectconnection) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/connections/{id}/disconnect | Disconnects a wallet connect connection|
|[**walletConnectServiceGetConnection**](#walletconnectservicegetconnection) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/connections/{id} | Get a wallet connect connection|
|[**walletConnectServiceListConnections**](#walletconnectservicelistconnections) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/connections | List connections for the wallet|
|[**walletConnectServiceListGlobalConnections**](#walletconnectservicelistglobalconnections) | **GET** /v2/connections | List connections for the organization|
|[**walletConnectServiceRejectConnection**](#walletconnectservicerejectconnection) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/connections/{id}/reject | Reject a wallet connect connection|

# **walletConnectServiceAcceptConnection**
> V2Connection walletConnectServiceAcceptConnection()

Accept a wallet connect connection by ID

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let id: string; //The connection ID (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceAcceptConnection(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|
| **id** | [**string**] | The connection ID | defaults to undefined|


### Return type

**V2Connection**

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

# **walletConnectServiceCreateConnection**
> V2Connection walletConnectServiceCreateConnection(walletConnectServiceCreateConnectionRequest)

Proposes a new wallet connect connection using the provided URI

### Example

```typescript
import {
    WalletConnectApi,
    Configuration,
    WalletConnectServiceCreateConnectionRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let walletConnectServiceCreateConnectionRequest: WalletConnectServiceCreateConnectionRequest; //

const { status, data } = await apiInstance.walletConnectServiceCreateConnection(
    vaultId,
    walletId,
    walletConnectServiceCreateConnectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **walletConnectServiceCreateConnectionRequest** | **WalletConnectServiceCreateConnectionRequest**|  | |
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|


### Return type

**V2Connection**

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

# **walletConnectServiceDisconnectConnection**
> V2Connection walletConnectServiceDisconnectConnection()

Disconnects a wallet connect connection by ID

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let id: string; //The connection ID (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceDisconnectConnection(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|
| **id** | [**string**] | The connection ID | defaults to undefined|


### Return type

**V2Connection**

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

# **walletConnectServiceGetConnection**
> V2Connection walletConnectServiceGetConnection()

Get a wallet connect connection by ID

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let id: string; //The connection ID (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceGetConnection(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|
| **id** | [**string**] | The connection ID | defaults to undefined|


### Return type

**V2Connection**

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

# **walletConnectServiceListConnections**
> Array<V2Connection> walletConnectServiceListConnections()

List all wallet connect connections for the wallet

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let status: 'CREATED' | 'PROPOSING' | 'PROPOSED' | 'CONNECTED' | 'DISCONNECTED' | 'REJECTED' | 'UNSUPPORTED' | 'EXPIRED' | 'ERROR'; //The connection status (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceListConnections(
    vaultId,
    walletId,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|
| **status** | [**&#39;CREATED&#39; | &#39;PROPOSING&#39; | &#39;PROPOSED&#39; | &#39;CONNECTED&#39; | &#39;DISCONNECTED&#39; | &#39;REJECTED&#39; | &#39;UNSUPPORTED&#39; | &#39;EXPIRED&#39; | &#39;ERROR&#39;**]**Array<&#39;CREATED&#39; &#124; &#39;PROPOSING&#39; &#124; &#39;PROPOSED&#39; &#124; &#39;CONNECTED&#39; &#124; &#39;DISCONNECTED&#39; &#124; &#39;REJECTED&#39; &#124; &#39;UNSUPPORTED&#39; &#124; &#39;EXPIRED&#39; &#124; &#39;ERROR&#39;>** | The connection status | defaults to undefined|


### Return type

**Array<V2Connection>**

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

# **walletConnectServiceListGlobalConnections**
> Array<V2Connection> walletConnectServiceListGlobalConnections()

List all wallet connect connections for the organization

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let status: 'CREATED' | 'PROPOSING' | 'PROPOSED' | 'CONNECTED' | 'DISCONNECTED' | 'REJECTED' | 'UNSUPPORTED' | 'EXPIRED' | 'ERROR'; //The connection status (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceListGlobalConnections(
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **status** | [**&#39;CREATED&#39; | &#39;PROPOSING&#39; | &#39;PROPOSED&#39; | &#39;CONNECTED&#39; | &#39;DISCONNECTED&#39; | &#39;REJECTED&#39; | &#39;UNSUPPORTED&#39; | &#39;EXPIRED&#39; | &#39;ERROR&#39;**]**Array<&#39;CREATED&#39; &#124; &#39;PROPOSING&#39; &#124; &#39;PROPOSED&#39; &#124; &#39;CONNECTED&#39; &#124; &#39;DISCONNECTED&#39; &#124; &#39;REJECTED&#39; &#124; &#39;UNSUPPORTED&#39; &#124; &#39;EXPIRED&#39; &#124; &#39;ERROR&#39;>** | The connection status | defaults to undefined|


### Return type

**Array<V2Connection>**

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

# **walletConnectServiceRejectConnection**
> V2Connection walletConnectServiceRejectConnection()

Reject a wallet connect connection by ID

### Example

```typescript
import {
    WalletConnectApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletConnectApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let walletId: string; //The wallet ID that the connection is associated with (default to undefined)
let id: string; //The connection ID (default to undefined)

const { status, data } = await apiInstance.walletConnectServiceRejectConnection(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **walletId** | [**string**] | The wallet ID that the connection is associated with | defaults to undefined|
| **id** | [**string**] | The connection ID | defaults to undefined|


### Return type

**V2Connection**

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

