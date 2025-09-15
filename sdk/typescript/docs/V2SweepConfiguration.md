# V2SweepConfiguration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The sweep configuration ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user who created this sweep configuration | [default to undefined]
**createdAt** | **string** | The date and time the sweep configuration was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this sweep configuration | [default to undefined]
**updatedAt** | **string** | The date and time the sweep configuration was updated | [default to undefined]
**name** | **string** | The sweep configuration name | [default to undefined]
**description** | **string** | The sweep configuration description | [optional] [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**feeWallet** | [**V2VaultWalletIdentifier**](V2VaultWalletIdentifier.md) |  | [default to undefined]
**destinationWallet** | [**V2VaultWalletIdentifier**](V2VaultWalletIdentifier.md) |  | [default to undefined]
**sweepFrequency** | [**V2SweepFrequency**](V2SweepFrequency.md) |  | [default to undefined]
**assets** | [**Array&lt;V2HydratedSweepAsset&gt;**](V2HydratedSweepAsset.md) | The assets to sweep | [default to undefined]
**status** | [**V2SweepStatus**](V2SweepStatus.md) |  | [default to undefined]
**lastSwept** | **string** | The date and time the sweep configuration was last executed | [optional] [default to undefined]
**sweepRunning** | **boolean** | Whether the sweep is currently running | [default to undefined]

## Example

```typescript
import { V2SweepConfiguration } from '@palisade-inc/typescript-sdk';

const instance: V2SweepConfiguration = {
    id,
    organizationId,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    name,
    description,
    blockchain,
    feeWallet,
    destinationWallet,
    sweepFrequency,
    assets,
    status,
    lastSwept,
    sweepRunning,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
