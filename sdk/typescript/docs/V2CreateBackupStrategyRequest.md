# V2CreateBackupStrategyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the backup strategy (2-64 characters) | [optional] [default to undefined]
**recoveryPublicKeys** | [**Array&lt;V2CreateRecoveryPublicKeyRequest&gt;**](V2CreateRecoveryPublicKeyRequest.md) | List of backup keys - DER formatted, hex encoded RSA public keys (min 4096 bits) | [optional] [default to undefined]
**s3Config** | [**V2S3Config**](V2S3Config.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2CreateBackupStrategyRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateBackupStrategyRequest = {
    name,
    recoveryPublicKeys,
    s3Config,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
