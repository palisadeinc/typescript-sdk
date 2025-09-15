# TransactionsServiceTransferTransactionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**destinationAddress** | **string** | The destination address | [default to undefined]
**contract** | **string** | The contract/issuing address | [optional] [default to undefined]
**symbol** | **string** | The asset symbol | [default to undefined]
**qty** | **string** | The quantity of the asset to transfer | [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**externalId** | **string** | External ID of this transaction, unique to the organization | [optional] [default to undefined]
**networkFee** | **string** | The maximum network fee to pay for this transaction in base asset units (eg ETH for Ethereum) | [optional] [default to undefined]
**config** | [**V2XRPTransactionConfig**](V2XRPTransactionConfig.md) |  | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for this transaction, used to correlate multiple actions | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceTransferTransactionRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceTransferTransactionRequest = {
    destinationAddress,
    contract,
    symbol,
    qty,
    sequence,
    externalId,
    networkFee,
    config,
    correlationId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
