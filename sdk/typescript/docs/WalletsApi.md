# WalletsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vaultServiceCreateWallet**](#vaultservicecreatewallet) | **POST** /v2/vaults/{vaultId}/wallets | Create a wallet|
|[**vaultServiceDeleteWallet**](#vaultservicedeletewallet) | **DELETE** /v2/vaults/{vaultId}/wallets/{walletId} | Delete a wallet|
|[**vaultServiceGetWallet**](#vaultservicegetwallet) | **GET** /v2/vaults/{vaultId}/wallets/{walletId} | Get a wallet|
|[**vaultServiceGetWalletByID**](#vaultservicegetwalletbyid) | **GET** /v2/wallets/{id} | Get a wallet by ID|
|[**vaultServiceGetWalletSequence**](#vaultservicegetwalletsequence) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/sequence | Get a wallet nonce/sequence|
|[**vaultServiceListGlobalWallets**](#vaultservicelistglobalwallets) | **GET** /v2/wallets | List organization wallets|
|[**vaultServiceListVaultWallets**](#vaultservicelistvaultwallets) | **GET** /v2/vaults/{vaultId}/wallets | List vault wallets|
|[**vaultServiceUpdateWallet**](#vaultserviceupdatewallet) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId} | Update a wallet|
|[**vaultServiceUpdateWalletSettings**](#vaultserviceupdatewalletsettings) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/settings | Update a wallet\&#39;s settings|

# **vaultServiceCreateWallet**
> Vaultv2Wallet vaultServiceCreateWallet(vaultServiceCreateWalletRequest)

Create a new HSM or MPC wallet within a vault

### Example

```typescript
import {
    WalletsApi,
    Configuration,
    VaultServiceCreateWalletRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let vaultServiceCreateWalletRequest: VaultServiceCreateWalletRequest; //

const { status, data } = await apiInstance.vaultServiceCreateWallet(
    vaultId,
    vaultServiceCreateWalletRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceCreateWalletRequest** | **VaultServiceCreateWalletRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|


### Return type

**Vaultv2Wallet**

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

# **vaultServiceDeleteWallet**
> object vaultServiceDeleteWallet()

Delete a wallet by ID (A wallet can only be deleted if it is in PROVISIONING_FAILED status)

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceDeleteWallet(
    vaultId,
    walletId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


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

# **vaultServiceGetWallet**
> Vaultv2Wallet vaultServiceGetWallet()

Get a wallet by ID

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceGetWallet(
    vaultId,
    walletId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Vaultv2Wallet**

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

# **vaultServiceGetWalletByID**
> Vaultv2Wallet vaultServiceGetWalletByID()

Get a wallet by its unique ID

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let id: string; //The wallet ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceGetWalletByID(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Vaultv2Wallet**

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

# **vaultServiceGetWalletSequence**
> V2GetWalletSequenceResponse vaultServiceGetWalletSequence()

Get blockchain nonce/sequence of a specific wallet by ID

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceGetWalletSequence(
    vaultId,
    walletId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**V2GetWalletSequenceResponse**

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

# **vaultServiceListGlobalWallets**
> V2ListGlobalWalletsResponse vaultServiceListGlobalWallets()

List all wallets within the organization

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)
let blockchain: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; //The blockchain of the wallet (optional) (default to undefined)
let correlationId: string; //Correlation ID for tracking various actions on the wallet (optional) (default to undefined)
let address: string; //The wallet address to filter by (optional) (default to undefined)

const { status, data } = await apiInstance.vaultServiceListGlobalWallets(
    pageSize,
    pageToken,
    blockchain,
    correlationId,
    address
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|
| **blockchain** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** | The blockchain of the wallet | (optional) defaults to undefined|
| **correlationId** | [**string**] | Correlation ID for tracking various actions on the wallet | (optional) defaults to undefined|
| **address** | [**string**] | The wallet address to filter by | (optional) defaults to undefined|


### Return type

**V2ListGlobalWalletsResponse**

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

# **vaultServiceListVaultWallets**
> V2ListVaultWalletsResponse vaultServiceListVaultWallets()

List all wallets within a vault

### Example

```typescript
import {
    WalletsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)
let blockchain: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; //The blockchain of the wallet (optional) (default to undefined)

const { status, data } = await apiInstance.vaultServiceListVaultWallets(
    vaultId,
    pageSize,
    pageToken,
    blockchain
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|
| **blockchain** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** | The blockchain of the wallet | (optional) defaults to undefined|


### Return type

**V2ListVaultWalletsResponse**

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

# **vaultServiceUpdateWallet**
> Vaultv2Wallet vaultServiceUpdateWallet(vaultServiceUpdateWalletRequest)

Update a wallet\'s name and description by ID

### Example

```typescript
import {
    WalletsApi,
    Configuration,
    VaultServiceUpdateWalletRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let vaultServiceUpdateWalletRequest: VaultServiceUpdateWalletRequest; //

const { status, data } = await apiInstance.vaultServiceUpdateWallet(
    vaultId,
    walletId,
    vaultServiceUpdateWalletRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceUpdateWalletRequest** | **VaultServiceUpdateWalletRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Vaultv2Wallet**

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

# **vaultServiceUpdateWalletSettings**
> Vaultv2Wallet vaultServiceUpdateWalletSettings(vaultServiceUpdateWalletSettingsRequest)

Update a wallet\'s settings by ID

### Example

```typescript
import {
    WalletsApi,
    Configuration,
    VaultServiceUpdateWalletSettingsRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let vaultServiceUpdateWalletSettingsRequest: VaultServiceUpdateWalletSettingsRequest; //

const { status, data } = await apiInstance.vaultServiceUpdateWalletSettings(
    vaultId,
    walletId,
    vaultServiceUpdateWalletSettingsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceUpdateWalletSettingsRequest** | **VaultServiceUpdateWalletSettingsRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Vaultv2Wallet**

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

