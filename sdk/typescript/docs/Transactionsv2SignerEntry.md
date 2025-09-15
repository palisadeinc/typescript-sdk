# Transactionsv2SignerEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **string** | Wallet address of the signer. The wallet does not need to exist. | [default to undefined]
**signerWeight** | **number** | Weight of the signature produced by this signer. | [default to undefined]

## Example

```typescript
import { Transactionsv2SignerEntry } from '@palisade-inc/typescript-sdk';

const instance: Transactionsv2SignerEntry = {
    account,
    signerWeight,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
