# BalancesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**balanceServiceGetOrgBalances**](#balanceservicegetorgbalances) | **GET** /v2/balances | Get Organization Balances|
|[**balanceServiceGetVaultBalances**](#balanceservicegetvaultbalances) | **GET** /v2/vaults/{vaultId}/balances | Get Vault Balances|
|[**balanceServiceGetWalletBalances**](#balanceservicegetwalletbalances) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/balances | Get Wallet Balances|

# **balanceServiceGetOrgBalances**
> V2GetOrgBalancesResponse balanceServiceGetOrgBalances()

Get the balance of an organization

### Example

```typescript
import {
    BalancesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new BalancesApi(configuration);

let currencyCode: string; //The currency code to be used for the fiat value. When omitted, \'USD\' will be used. (optional) (default to undefined)

const { status, data } = await apiInstance.balanceServiceGetOrgBalances(
    currencyCode
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **currencyCode** | [**string**] | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | (optional) defaults to undefined|


### Return type

**V2GetOrgBalancesResponse**

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

# **balanceServiceGetVaultBalances**
> V2GetVaultBalancesResponse balanceServiceGetVaultBalances()

Get the balances of a vault

### Example

```typescript
import {
    BalancesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new BalancesApi(configuration);

let vaultId: string; //The vault ID that the connection is associated with (default to undefined)
let currencyCode: string; //The currency code to be used for the fiat value. When omitted, \'USD\' will be used. (optional) (default to undefined)

const { status, data } = await apiInstance.balanceServiceGetVaultBalances(
    vaultId,
    currencyCode
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID that the connection is associated with | defaults to undefined|
| **currencyCode** | [**string**] | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | (optional) defaults to undefined|


### Return type

**V2GetVaultBalancesResponse**

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

# **balanceServiceGetWalletBalances**
> V2GetWalletBalancesResponse balanceServiceGetWalletBalances()

Get the balances of a wallet

### Example

```typescript
import {
    BalancesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new BalancesApi(configuration);

let vaultId: string; // (default to undefined)
let walletId: string; // (default to undefined)
let currencyCode: string; //The currency code to be used for the fiat value. When omitted, \'USD\' will be used. (optional) (default to undefined)

const { status, data } = await apiInstance.balanceServiceGetWalletBalances(
    vaultId,
    walletId,
    currencyCode
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] |  | defaults to undefined|
| **walletId** | [**string**] |  | defaults to undefined|
| **currencyCode** | [**string**] | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | (optional) defaults to undefined|


### Return type

**V2GetWalletBalancesResponse**

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

