# VaultsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vaultServiceCreateVault**](#vaultservicecreatevault) | **POST** /v2/vaults | Create a vault|
|[**vaultServiceGetVault**](#vaultservicegetvault) | **GET** /v2/vaults/{id} | Get a vault|
|[**vaultServiceListVaults**](#vaultservicelistvaults) | **GET** /v2/vaults | List vaults|
|[**vaultServiceUpdateVault**](#vaultserviceupdatevault) | **PUT** /v2/vaults/{id} | Update a vault|

# **vaultServiceCreateVault**
> V2Vault vaultServiceCreateVault(v2CreateVaultRequest)

Create a new vault

### Example

```typescript
import {
    VaultsApi,
    Configuration,
    V2CreateVaultRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultsApi(configuration);

let v2CreateVaultRequest: V2CreateVaultRequest; //

const { status, data } = await apiInstance.vaultServiceCreateVault(
    v2CreateVaultRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateVaultRequest** | **V2CreateVaultRequest**|  | |


### Return type

**V2Vault**

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

# **vaultServiceGetVault**
> V2Vault vaultServiceGetVault()

Get a vault by ID

### Example

```typescript
import {
    VaultsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultsApi(configuration);

let id: string; //The vault ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceGetVault(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The vault ID | defaults to undefined|


### Return type

**V2Vault**

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

# **vaultServiceListVaults**
> V2ListVaultsResponse vaultServiceListVaults()

List all vaults within the organization

### Example

```typescript
import {
    VaultsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultsApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)
let correlationId: string; //Correlation ID for tracking various actions on the vault (optional) (default to undefined)

const { status, data } = await apiInstance.vaultServiceListVaults(
    pageSize,
    pageToken,
    correlationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|
| **correlationId** | [**string**] | Correlation ID for tracking various actions on the vault | (optional) defaults to undefined|


### Return type

**V2ListVaultsResponse**

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

# **vaultServiceUpdateVault**
> V2Vault vaultServiceUpdateVault(vaultServiceUpdateVaultRequest)

Update a vault\'s name and description by ID

### Example

```typescript
import {
    VaultsApi,
    Configuration,
    VaultServiceUpdateVaultRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultsApi(configuration);

let id: string; //The vault ID (default to undefined)
let vaultServiceUpdateVaultRequest: VaultServiceUpdateVaultRequest; //

const { status, data } = await apiInstance.vaultServiceUpdateVault(
    id,
    vaultServiceUpdateVaultRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceUpdateVaultRequest** | **VaultServiceUpdateVaultRequest**|  | |
| **id** | [**string**] | The vault ID | defaults to undefined|


### Return type

**V2Vault**

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

