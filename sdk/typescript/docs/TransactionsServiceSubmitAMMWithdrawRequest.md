# TransactionsServiceSubmitAMMWithdrawRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset** | [**Transactionsv2Asset**](Transactionsv2Asset.md) |  | [default to undefined]
**amount** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [optional] [default to undefined]
**asset2** | [**Transactionsv2Asset**](Transactionsv2Asset.md) |  | [default to undefined]
**amount2** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [optional] [default to undefined]
**ePrice** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [optional] [default to undefined]
**lpTokenIn** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [optional] [default to undefined]
**flags** | [**Transactionsv2AMMWithdrawFlag**](Transactionsv2AMMWithdrawFlag.md) |  | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitAMMWithdrawRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitAMMWithdrawRequest = {
    asset,
    amount,
    asset2,
    amount2,
    ePrice,
    lpTokenIn,
    flags,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
