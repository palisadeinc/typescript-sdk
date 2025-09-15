# Xrpv2CurrencyAmount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **string** | The quantity of the asset | [default to undefined]
**asset** | **string** | The asset symbol | [default to undefined]
**issuer** | **string** | The contract/issuing address. Optional if asset is XRP. | [optional] [default to undefined]

## Example

```typescript
import { Xrpv2CurrencyAmount } from '@palisade-inc/typescript-sdk';

const instance: Xrpv2CurrencyAmount = {
    value,
    asset,
    issuer,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
