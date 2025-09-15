# V2RecoveryPublicKey


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the recovery public key | [optional] [default to undefined]
**publicKey** | **string** | The DER formatted, hex encoded RSA public key | [optional] [default to undefined]
**createdBy** | **string** | User who created the recovery public key | [optional] [default to undefined]

## Example

```typescript
import { V2RecoveryPublicKey } from '@palisade-inc/typescript-sdk';

const instance: V2RecoveryPublicKey = {
    name,
    publicKey,
    createdBy,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
