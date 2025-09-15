# VaultServiceCreateWalletRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The name of the wallet | [default to undefined]
**description** | **string** | The description of the wallet | [optional] [default to undefined]
**quorumId** | **string** | The quorum ID | [optional] [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**keystore** | [**V2Keystore**](V2Keystore.md) |  | [default to undefined]
**recoveryPublicKey** | **string** | Optional, hex encoded PKCS1 formatted public key of a 4096-bit RSA private key | [optional] [default to undefined]
**externalId** | **string** | External ID of this wallet, unique to the organization | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for tracking correlations with the wallet | [optional] [default to undefined]

## Example

```typescript
import { VaultServiceCreateWalletRequest } from '@palisade-inc/typescript-sdk';

const instance: VaultServiceCreateWalletRequest = {
    name,
    description,
    quorumId,
    blockchain,
    keystore,
    recoveryPublicKey,
    externalId,
    correlationId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
