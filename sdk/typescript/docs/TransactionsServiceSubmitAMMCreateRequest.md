# TransactionsServiceSubmitAMMCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**amount2** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**tradingFee** | **number** | The fee to charge for trades against this AMM instance, in units of 1/100,000 | [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitAMMCreateRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitAMMCreateRequest = {
    amount,
    amount2,
    tradingFee,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
