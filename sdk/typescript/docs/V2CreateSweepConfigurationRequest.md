# V2CreateSweepConfigurationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The sweep configuration name | [default to undefined]
**description** | **string** | The sweep configuration description | [optional] [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**feeWallet** | [**V2VaultWalletIdentifier**](V2VaultWalletIdentifier.md) |  | [default to undefined]
**destinationWallet** | [**V2VaultWalletIdentifier**](V2VaultWalletIdentifier.md) |  | [default to undefined]
**sweepFrequency** | [**V2SweepFrequency**](V2SweepFrequency.md) |  | [default to undefined]
**assets** | [**Array&lt;V2SweepAsset&gt;**](V2SweepAsset.md) | The assets to sweep | [default to undefined]

## Example

```typescript
import { V2CreateSweepConfigurationRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateSweepConfigurationRequest = {
    name,
    description,
    blockchain,
    feeWallet,
    destinationWallet,
    sweepFrequency,
    assets,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
