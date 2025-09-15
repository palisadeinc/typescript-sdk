# RegistryManagementServiceManagementUpdateBlockchainRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Updated blockchain name | [optional] [default to undefined]
**namespace** | **string** | Updated namespace | [optional] [default to undefined]
**chain** | **string** | Updated chain identifier | [optional] [default to undefined]
**chainId** | **string** | Updated chain ID | [optional] [default to undefined]
**routing** | **string** | Updated routing configuration | [optional] [default to undefined]
**status** | [**V2BlockchainStatus**](V2BlockchainStatus.md) |  | [optional] [default to undefined]
**supportsWalletConnect** | **boolean** | Updated WalletConnect support | [optional] [default to undefined]

## Example

```typescript
import { RegistryManagementServiceManagementUpdateBlockchainRequest } from '@palisade-inc/typescript-sdk';

const instance: RegistryManagementServiceManagementUpdateBlockchainRequest = {
    name,
    namespace,
    chain,
    chainId,
    routing,
    status,
    supportsWalletConnect,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
