# V2InternalGetWalletBalancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currencyCode** | **string** |  | [default to undefined]
**aggregatedFiatValue** | **string** |  | [optional] [default to undefined]
**balances** | [**Array&lt;V2Balance&gt;**](V2Balance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2InternalGetWalletBalancesResponse } from '@palisade-inc/typescript-sdk';

const instance: V2InternalGetWalletBalancesResponse = {
    currencyCode,
    aggregatedFiatValue,
    balances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
