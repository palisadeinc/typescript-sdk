# V2ManagementCreateAssetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**blockchainId** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**contractAddress** | **string** | Contract address (empty for native assets) | [optional] [default to undefined]
**symbol** | **string** | Asset symbol | [default to undefined]
**name** | **string** | Asset name | [optional] [default to undefined]
**decimals** | **number** | Number of decimal places | [optional] [default to undefined]
**standard** | [**V2Standard**](V2Standard.md) |  | [default to undefined]
**coingeckoId** | **string** | CoinGecko identifier for price data | [optional] [default to undefined]
**enabled** | **boolean** | Whether the asset is enabled (default: true) | [optional] [default to undefined]
**vetted** | **boolean** | Whether the asset is vetted (default: false) | [optional] [default to undefined]

## Example

```typescript
import { V2ManagementCreateAssetRequest } from '@palisade-inc/typescript-sdk';

const instance: V2ManagementCreateAssetRequest = {
    blockchainId,
    contractAddress,
    symbol,
    name,
    decimals,
    standard,
    coingeckoId,
    enabled,
    vetted,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
