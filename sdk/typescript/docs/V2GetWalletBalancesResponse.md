# V2GetWalletBalancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currencyCode** | **string** | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | [default to undefined]
**aggregatedFiatValue** | **string** |  | [optional] [default to undefined]
**balances** | [**Array&lt;V2Balance&gt;**](V2Balance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2GetWalletBalancesResponse } from '@palisade-inc/typescript-sdk';

const instance: V2GetWalletBalancesResponse = {
    currencyCode,
    aggregatedFiatValue,
    balances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
