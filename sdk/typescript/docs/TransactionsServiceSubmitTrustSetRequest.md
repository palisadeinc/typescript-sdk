# TransactionsServiceSubmitTrustSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limitAmount** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**qualityIn** | **number** | Value incoming balances on this trust line at the ratio of this number per 1,000,000,000 units. A value of 0 is shorthand for treating balances at face value. | [optional] [default to undefined]
**qualityOut** | **number** | Value outgoing balances on this trust line at the ratio of this number per 1,000,000,000 units. A value of 0 is shorthand for treating balances at face value. | [optional] [default to undefined]
**flags** | [**Array&lt;Transactionsv2TrustSetFlag&gt;**](Transactionsv2TrustSetFlag.md) | Configuration flags | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitTrustSetRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitTrustSetRequest = {
    limitAmount,
    qualityIn,
    qualityOut,
    flags,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
