# TransactionsServiceSubmitClawbackRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**holder** | **string** | Optional holder address for MPTokens | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitClawbackRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitClawbackRequest = {
    amount,
    holder,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
