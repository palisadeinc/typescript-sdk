# TransactionsXRPApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**transactionsServiceSubmitAMMCreate**](#transactionsservicesubmitammcreate) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-create | Create a new XRP AMM Create transaction|
|[**transactionsServiceSubmitAMMDeposit**](#transactionsservicesubmitammdeposit) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-deposit | Create a new XRP AMM Deposit transaction|
|[**transactionsServiceSubmitAMMWithdraw**](#transactionsservicesubmitammwithdraw) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-withdraw | Create a new XRP AMM Withdraw transaction|
|[**transactionsServiceSubmitAccountSet**](#transactionsservicesubmitaccountset) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/account-set | Create a new XRP Account Set transaction|
|[**transactionsServiceSubmitClawback**](#transactionsservicesubmitclawback) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/clawback | Create a new XRP Clawback transaction|
|[**transactionsServiceSubmitOfferCancel**](#transactionsservicesubmitoffercancel) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/offer-cancel | Create a new XRP Offer Cancel transaction|
|[**transactionsServiceSubmitOfferCreate**](#transactionsservicesubmitoffercreate) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/offer-create | Create a new XRP Offer Create transaction|
|[**transactionsServiceSubmitSignerListSet**](#transactionsservicesubmitsignerlistset) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/signer-list-set | Create a new XRP SignerList Set transaction|
|[**transactionsServiceSubmitTrustSet**](#transactionsservicesubmittrustset) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/trust-set | Create a new XRP Trust Set transaction|

# **transactionsServiceSubmitAMMCreate**
> Transactionsv2Transaction transactionsServiceSubmitAMMCreate(transactionsServiceSubmitAMMCreateRequest)

Create a new XRP AMM Create transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitAMMCreateRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitAMMCreateRequest: TransactionsServiceSubmitAMMCreateRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitAMMCreate(
    vaultId,
    walletId,
    transactionsServiceSubmitAMMCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitAMMCreateRequest** | **TransactionsServiceSubmitAMMCreateRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitAMMDeposit**
> Transactionsv2Transaction transactionsServiceSubmitAMMDeposit(transactionsServiceSubmitAMMDepositRequest)

Create a new XRP AMM Deposit transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitAMMDepositRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitAMMDepositRequest: TransactionsServiceSubmitAMMDepositRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitAMMDeposit(
    vaultId,
    walletId,
    transactionsServiceSubmitAMMDepositRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitAMMDepositRequest** | **TransactionsServiceSubmitAMMDepositRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitAMMWithdraw**
> Transactionsv2Transaction transactionsServiceSubmitAMMWithdraw(transactionsServiceSubmitAMMWithdrawRequest)

Create a new XRP AMM Withdraw transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitAMMWithdrawRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitAMMWithdrawRequest: TransactionsServiceSubmitAMMWithdrawRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitAMMWithdraw(
    vaultId,
    walletId,
    transactionsServiceSubmitAMMWithdrawRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitAMMWithdrawRequest** | **TransactionsServiceSubmitAMMWithdrawRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitAccountSet**
> Transactionsv2Transaction transactionsServiceSubmitAccountSet(transactionsServiceSubmitAccountSetRequest)

Create a new XRP Account Set transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitAccountSetRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitAccountSetRequest: TransactionsServiceSubmitAccountSetRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitAccountSet(
    vaultId,
    walletId,
    transactionsServiceSubmitAccountSetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitAccountSetRequest** | **TransactionsServiceSubmitAccountSetRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitClawback**
> Transactionsv2Transaction transactionsServiceSubmitClawback(transactionsServiceSubmitClawbackRequest)

Create a new XRP Clawback transaction to recover issued tokens

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitClawbackRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitClawbackRequest: TransactionsServiceSubmitClawbackRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitClawback(
    vaultId,
    walletId,
    transactionsServiceSubmitClawbackRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitClawbackRequest** | **TransactionsServiceSubmitClawbackRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitOfferCancel**
> Transactionsv2Transaction transactionsServiceSubmitOfferCancel(transactionsServiceSubmitOfferCancelRequest)

Create a new XRP Offer Cancel transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitOfferCancelRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitOfferCancelRequest: TransactionsServiceSubmitOfferCancelRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitOfferCancel(
    vaultId,
    walletId,
    transactionsServiceSubmitOfferCancelRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitOfferCancelRequest** | **TransactionsServiceSubmitOfferCancelRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitOfferCreate**
> Transactionsv2Transaction transactionsServiceSubmitOfferCreate(transactionsServiceSubmitOfferCreateRequest)

Create a new XRP Offer Create transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitOfferCreateRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitOfferCreateRequest: TransactionsServiceSubmitOfferCreateRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitOfferCreate(
    vaultId,
    walletId,
    transactionsServiceSubmitOfferCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitOfferCreateRequest** | **TransactionsServiceSubmitOfferCreateRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitSignerListSet**
> Transactionsv2Transaction transactionsServiceSubmitSignerListSet(transactionsServiceSubmitSignerListSetRequest)

Create a new XRP SignerList Set transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitSignerListSetRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitSignerListSetRequest: TransactionsServiceSubmitSignerListSetRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitSignerListSet(
    vaultId,
    walletId,
    transactionsServiceSubmitSignerListSetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitSignerListSetRequest** | **TransactionsServiceSubmitSignerListSetRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceSubmitTrustSet**
> Transactionsv2Transaction transactionsServiceSubmitTrustSet(transactionsServiceSubmitTrustSetRequest)

Create a new XRP Trust Set transaction

### Example

```typescript
import {
    TransactionsXRPApi,
    Configuration,
    TransactionsServiceSubmitTrustSetRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsXRPApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSubmitTrustSetRequest: TransactionsServiceSubmitTrustSetRequest; //

const { status, data } = await apiInstance.transactionsServiceSubmitTrustSet(
    vaultId,
    walletId,
    transactionsServiceSubmitTrustSetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSubmitTrustSetRequest** | **TransactionsServiceSubmitTrustSetRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

