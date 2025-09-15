# TransactionsServiceSubmitOfferCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expiration** | **string** | Unix timestamp after which this offer is no longer active | [optional] [default to undefined]
**offerSequence** | **string** | Sequence of offer to delete first, specified in the same way as OfferCancel | [optional] [default to undefined]
**takerGets** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**takerPays** | [**Transactionsv2CurrencyAmount**](Transactionsv2CurrencyAmount.md) |  | [default to undefined]
**flags** | [**Array&lt;Transactionsv2OfferCreateFlags&gt;**](Transactionsv2OfferCreateFlags.md) | Configuration flags | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitOfferCreateRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitOfferCreateRequest = {
    expiration,
    offerSequence,
    takerGets,
    takerPays,
    flags,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
