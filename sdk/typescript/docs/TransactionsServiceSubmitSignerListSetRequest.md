# TransactionsServiceSubmitSignerListSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**signerQuorum** | **number** | Minimum sum of weights required in order to authorise a transaction. Sum of all weights of individual signers must be greater than or equal to this value. | [default to undefined]
**signerEntries** | [**Array&lt;Transactionsv2SignerEntry&gt;**](Transactionsv2SignerEntry.md) | List of signers. Leave empty with &#x60;signerQuorum&#x60; set to 0 to disable. | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitSignerListSetRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitSignerListSetRequest = {
    signerQuorum,
    signerEntries,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
