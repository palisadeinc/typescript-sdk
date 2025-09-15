# V2CreateRecoveryPublicKeyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the recovery public key | [optional] [default to undefined]
**publicKey** | **string** | The DER formatted, hex encoded RSA public key | [optional] [default to undefined]

## Example

```typescript
import { V2CreateRecoveryPublicKeyRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateRecoveryPublicKeyRequest = {
    name,
    publicKey,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
