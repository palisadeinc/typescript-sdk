# TransactionsServiceSubmitAccountSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**setFlag** | [**Transactionsv2AccountSetFlag**](Transactionsv2AccountSetFlag.md) |  | [optional] [default to undefined]
**clearFlag** | [**Transactionsv2AccountSetFlag**](Transactionsv2AccountSetFlag.md) |  | [optional] [default to undefined]
**domain** | **string** | Hex encoded string representing domain that owns this account in ASCII, less than 256 chars. Set empty to unset. | [optional] [default to undefined]
**emailHash** | **string** | Hex encoded 128-bit hash bytes of the email address representing this account. Set empty to unset. | [optional] [default to undefined]
**messageKey** | **string** | 33-byte public key for sending encrypted messages to this account. First byte must be one of (0x02, 0x03, 0xED). Set empty to unset. | [optional] [default to undefined]
**nfTokenMinter** | **string** | Address of another account that can mint NFTokens for this account | [optional] [default to undefined]
**transferRate** | **number** | Fee to charge when users transfer tokens issued by this account, represented as billionths of a unit between 1000000000 and 2000000000 or 0. | [optional] [default to undefined]
**tickSize** | **number** | Tick size to use for offers involving a currency issued by this address, must be 3 to 15 (inclusive) or 0 | [optional] [default to undefined]
**walletLocator** | **string** | An arbitrary 256-bit hash value to associate with this account | [optional] [default to undefined]
**walletSize** | **number** | Unused field to associate on the account | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**lastLedgerSequence** | **string** | Highest ledger index this transaction can appear in. | [optional] [default to undefined]
**sourceTag** | **string** | Source tag to use for this transaction | [optional] [default to undefined]

## Example

```typescript
import { TransactionsServiceSubmitAccountSetRequest } from '@palisade-inc/typescript-sdk';

const instance: TransactionsServiceSubmitAccountSetRequest = {
    setFlag,
    clearFlag,
    domain,
    emailHash,
    messageKey,
    nfTokenMinter,
    transferRate,
    tickSize,
    walletLocator,
    walletSize,
    sequence,
    lastLedgerSequence,
    sourceTag,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
