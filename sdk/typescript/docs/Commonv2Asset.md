# Commonv2Asset

Asset is any blockchain asset e.g. USDC, XRP etc.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | ID is unique across all blockchains and created by combining the blockchain ID, contract address, and symbol | [default to undefined]
**standard** | [**V2Standard**](V2Standard.md) |  | [default to undefined]
**symbol** | **string** | The currency symbol of the asset | [default to undefined]
**name** | **string** | The human readable name of the asset | [optional] [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**decimals** | **number** | Count of decimal places for the asset | [optional] [default to undefined]
**vetted** | **boolean** | Whether the asset is vetted on the regulated platform | [optional] [default to undefined]
**enabled** | **boolean** | Whether the asset is currently enabled on the platform | [optional] [default to undefined]
**contract** | **string** | The token contract address. This field will be empty if the asset is the native coin of the blockchain | [optional] [default to undefined]
**createdAt** | **string** | The date and time the asset was created | [default to undefined]
**updatedAt** | **string** | The date and time the asset was last updated | [optional] [default to undefined]
**organizationId** | **string** | Organization ID for custom assets | [optional] [default to undefined]
**coingeckoId** | **string** | CoinGecko identifier for price data (optional for testnet assets) | [optional] [default to undefined]
**source** | [**V2AssetSource**](V2AssetSource.md) |  | [optional] [default to undefined]
**sourceMetadata** | [**ProtobufAny**](ProtobufAny.md) |  | [optional] [default to undefined]
**lastSyncedAt** | **string** | When this asset was last synchronized | [optional] [default to undefined]
**syncVersion** | **number** | Version counter for sync updates | [optional] [default to undefined]
**contractAddressChecksummed** | **string** | Checksummed version of the contract address | [optional] [default to undefined]

## Example

```typescript
import { Commonv2Asset } from '@palisade-inc/typescript-sdk';

const instance: Commonv2Asset = {
    id,
    standard,
    symbol,
    name,
    blockchain,
    decimals,
    vetted,
    enabled,
    contract,
    createdAt,
    updatedAt,
    organizationId,
    coingeckoId,
    source,
    sourceMetadata,
    lastSyncedAt,
    syncVersion,
    contractAddressChecksummed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
