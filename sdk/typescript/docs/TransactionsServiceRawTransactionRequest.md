# TransactionsServiceRawTransactionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**encodedTransaction** | **string** | The encoded transaction. Note that this must be encoded in the relevant blockchain format. RLP encoded for EVM chains. Binary codec encoding for XRP. | [default to undefined]
**signOnly** | **boolean** | Whether to only sign the transaction, or also publish it to the blockchain | [default to undefined]

## Example

```typescript
import { TransactionsServiceRawTransactionRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceRawTransactionRequest = {
    encodedTransaction,
    signOnly,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
