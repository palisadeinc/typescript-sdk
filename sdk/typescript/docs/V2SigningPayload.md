# V2SigningPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inputIndex** | **number** | The index of the UTXO input this signing payload corresponds to | [default to undefined]
**signingHash** | **string** | The signing hash for this UTXO input | [default to undefined]
**signature** | **string** | The signature for this UTXO input | [optional] [default to undefined]

## Example

```typescript
import { V2SigningPayload } from '@palisade-inc/typescript-sdk';

const instance: V2SigningPayload = {
    inputIndex,
    signingHash,
    signature,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
