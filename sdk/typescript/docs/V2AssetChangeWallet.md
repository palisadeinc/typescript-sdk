# V2AssetChangeWallet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **string** | The blockchain address of the wallet | [default to undefined]
**walletId** | **string** | The wallet ID that is part of this change, populated only if it belongs to the same organization that is party to the transaction | [optional] [default to undefined]

## Example

```typescript
import { V2AssetChangeWallet } from '@palisade-inc/typescript-sdk';

const instance: V2AssetChangeWallet = {
    address,
    walletId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
