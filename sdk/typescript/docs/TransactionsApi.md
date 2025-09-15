# TransactionsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**transactionsServiceEstimateTransferFee**](#transactionsserviceestimatetransferfee) | **POST** /v2/transactions/transfer/estimate-fee | Estimate the fee for a transfer transaction|
|[**transactionsServiceFreezeTransaction**](#transactionsservicefreezetransaction) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}/freeze | Freeze a transaction|
|[**transactionsServiceGetFreezeHistory**](#transactionsservicegetfreezehistory) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}/freeze-history | Get freeze history for a transaction|
|[**transactionsServiceGetTransaction**](#transactionsservicegettransaction) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId} | Get a transaction|
|[**transactionsServiceListWalletTransactions**](#transactionsservicelistwallettransactions) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/transactions | List wallet transactions|
|[**transactionsServiceRawTransaction**](#transactionsservicerawtransaction) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/raw | Create a new raw transaction|
|[**transactionsServiceSignPlaintext**](#transactionsservicesignplaintext) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/sign-plaintext | (BETA) Create a new sign plaintext transaction|
|[**transactionsServiceTransferTransaction**](#transactionsservicetransfertransaction) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/transfer | Create a new transfer transaction|
|[**transactionsServiceUnfreezeTransaction**](#transactionsserviceunfreezetransaction) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}/unfreeze | Unfreeze a transaction|

# **transactionsServiceEstimateTransferFee**
> V2FeeEstimate transactionsServiceEstimateTransferFee(v2EstimateTransferFeeRequest)

Estimate the fee for a transfer transaction

### Example

```typescript
import {
    TransactionsApi,
    Configuration,
    V2EstimateTransferFeeRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let v2EstimateTransferFeeRequest: V2EstimateTransferFeeRequest; //

const { status, data } = await apiInstance.transactionsServiceEstimateTransferFee(
    v2EstimateTransferFeeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2EstimateTransferFeeRequest** | **V2EstimateTransferFeeRequest**|  | |


### Return type

**V2FeeEstimate**

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

# **transactionsServiceFreezeTransaction**
> Transactionsv2Transaction transactionsServiceFreezeTransaction()

Freeze a transaction by ID

### Example

```typescript
import {
    TransactionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionId: string; //The transaction ID (default to undefined)
let reason: string; //Reason for freezing the transaction (default to undefined)

const { status, data } = await apiInstance.transactionsServiceFreezeTransaction(
    vaultId,
    walletId,
    transactionId,
    reason
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **transactionId** | [**string**] | The transaction ID | defaults to undefined|
| **reason** | [**string**] | Reason for freezing the transaction | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceGetFreezeHistory**
> V2GetFreezeHistoryResponse transactionsServiceGetFreezeHistory()

Get the complete freeze/unfreeze history for a transaction

### Example

```typescript
import {
    TransactionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionId: string; //The transaction ID (default to undefined)

const { status, data } = await apiInstance.transactionsServiceGetFreezeHistory(
    vaultId,
    walletId,
    transactionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **transactionId** | [**string**] | The transaction ID | defaults to undefined|


### Return type

**V2GetFreezeHistoryResponse**

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

# **transactionsServiceGetTransaction**
> Transactionsv2Transaction transactionsServiceGetTransaction()

Get a transaction by ID

### Example

```typescript
import {
    TransactionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionId: string; //The transaction ID (default to undefined)

const { status, data } = await apiInstance.transactionsServiceGetTransaction(
    vaultId,
    walletId,
    transactionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **transactionId** | [**string**] | The transaction ID | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

# **transactionsServiceListWalletTransactions**
> V2ListWalletTransactionsResponse transactionsServiceListWalletTransactions()

List all transactions for a given wallet

### Example

```typescript
import {
    TransactionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)
let correlationId: string; //Correlation ID for this request, used to correlate multiple actions (optional) (default to undefined)

const { status, data } = await apiInstance.transactionsServiceListWalletTransactions(
    vaultId,
    walletId,
    pageSize,
    pageToken,
    correlationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|
| **correlationId** | [**string**] | Correlation ID for this request, used to correlate multiple actions | (optional) defaults to undefined|


### Return type

**V2ListWalletTransactionsResponse**

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

# **transactionsServiceRawTransaction**
> Transactionsv2Transaction transactionsServiceRawTransaction(transactionsServiceRawTransactionRequest)

Create a new raw transaction, and optionally publish it to the blockchain

### Example

```typescript
import {
    TransactionsApi,
    Configuration,
    TransactionsServiceRawTransactionRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceRawTransactionRequest: TransactionsServiceRawTransactionRequest; //

const { status, data } = await apiInstance.transactionsServiceRawTransaction(
    vaultId,
    walletId,
    transactionsServiceRawTransactionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceRawTransactionRequest** | **TransactionsServiceRawTransactionRequest**|  | |
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

# **transactionsServiceSignPlaintext**
> Transactionsv2Transaction transactionsServiceSignPlaintext(transactionsServiceSignPlaintextRequest)

(BETA) Create a new sign plaintext transaction

### Example

```typescript
import {
    TransactionsApi,
    Configuration,
    TransactionsServiceSignPlaintextRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceSignPlaintextRequest: TransactionsServiceSignPlaintextRequest; //

const { status, data } = await apiInstance.transactionsServiceSignPlaintext(
    vaultId,
    walletId,
    transactionsServiceSignPlaintextRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceSignPlaintextRequest** | **TransactionsServiceSignPlaintextRequest**|  | |
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

# **transactionsServiceTransferTransaction**
> Transactionsv2Transaction transactionsServiceTransferTransaction(transactionsServiceTransferTransactionRequest)

Create a new transfer transaction

### Example

```typescript
import {
    TransactionsApi,
    Configuration,
    TransactionsServiceTransferTransactionRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionsServiceTransferTransactionRequest: TransactionsServiceTransferTransactionRequest; //

const { status, data } = await apiInstance.transactionsServiceTransferTransaction(
    vaultId,
    walletId,
    transactionsServiceTransferTransactionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transactionsServiceTransferTransactionRequest** | **TransactionsServiceTransferTransactionRequest**|  | |
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

# **transactionsServiceUnfreezeTransaction**
> Transactionsv2Transaction transactionsServiceUnfreezeTransaction()

Unfreeze a transaction by ID

### Example

```typescript
import {
    TransactionsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let transactionId: string; //The transaction ID (default to undefined)
let reason: string; //Reason for unfreezing the transaction (default to undefined)

const { status, data } = await apiInstance.transactionsServiceUnfreezeTransaction(
    vaultId,
    walletId,
    transactionId,
    reason
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **transactionId** | [**string**] | The transaction ID | defaults to undefined|
| **reason** | [**string**] | Reason for unfreezing the transaction | defaults to undefined|


### Return type

**Transactionsv2Transaction**

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

