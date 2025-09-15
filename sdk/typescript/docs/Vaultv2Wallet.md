# Vaultv2Wallet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The wallet ID | [default to undefined]
**vaultId** | **string** | The vault ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**quorumId** | **string** | The quorum ID | [optional] [default to undefined]
**createdBy** | **string** | The user ID that created the wallet | [default to undefined]
**createdAt** | **string** | The date and time the wallet was created | [default to undefined]
**updatedAt** | **string** | The date and time the wallet was update | [default to undefined]
**name** | **string** | The name of the wallet | [default to undefined]
**description** | **string** | The description of the wallet | [optional] [default to undefined]
**address** | **string** | The address of the wallet | [optional] [default to undefined]
**publicKey** | **string** | The public key of the wallet | [optional] [default to undefined]
**keystore** | [**V2Keystore**](V2Keystore.md) |  | [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**settings** | [**V2WalletSettings**](V2WalletSettings.md) |  | [default to undefined]
**status** | [**Vaultv2WalletStatus**](Vaultv2WalletStatus.md) |  | [default to undefined]
**reasons** | **Array&lt;string&gt;** | The reasons why the wallet may have failed to provision | [optional] [default to undefined]
**passkeyPublic** | **string** |  | [optional] [default to undefined]
**alias** | **string** | The alias of the wallet | [optional] [default to undefined]
**externalId** | **string** | External ID of this wallet, unique to the organization | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for the wallet | [optional] [default to undefined]
**keyAlgorithm** | [**V2KeyAlgorithm**](V2KeyAlgorithm.md) |  | [default to undefined]

## Example

```typescript
import { Vaultv2Wallet } from '@palisade-inc/typescript-sdk';

const instance: Vaultv2Wallet = {
    id,
    vaultId,
    organizationId,
    quorumId,
    createdBy,
    createdAt,
    updatedAt,
    name,
    description,
    address,
    publicKey,
    keystore,
    blockchain,
    settings,
    status,
    reasons,
    passkeyPublic,
    alias,
    externalId,
    correlationId,
    keyAlgorithm,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
