# V2AssetChange


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**purpose** | [**V2AssetChangePurpose**](V2AssetChangePurpose.md) |  | [default to undefined]
**asset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [default to undefined]
**qty** | **string** | The quantity of the asset to transfer | [default to undefined]
**source** | [**V2AssetChangeWallet**](V2AssetChangeWallet.md) |  | [optional] [default to undefined]
**destination** | [**V2AssetChangeWallet**](V2AssetChangeWallet.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2AssetChange } from '@palisade-inc/typescript-sdk';

const instance: V2AssetChange = {
    purpose,
    asset,
    qty,
    source,
    destination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
