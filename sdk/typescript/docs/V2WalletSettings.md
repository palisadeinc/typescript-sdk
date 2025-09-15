# V2WalletSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **boolean** | Whether the wallet is enabled or not | [default to undefined]
**rawSigningEnabled** | **boolean** | Whether raw signing is enabled for the wallet | [default to undefined]
**sweepingEnabled** | **boolean** | Whether sweeping is enabled for the wallet | [default to undefined]
**defaultFreezeEnabled** | **boolean** | Whether to freeze inbound transactions by default | [default to undefined]

## Example

```typescript
import { V2WalletSettings } from '@palisade-inc/typescript-sdk';

const instance: V2WalletSettings = {
    enabled,
    rawSigningEnabled,
    sweepingEnabled,
    defaultFreezeEnabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
