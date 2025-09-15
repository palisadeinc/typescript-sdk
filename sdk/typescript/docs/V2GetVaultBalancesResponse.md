# V2GetVaultBalancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currencyCode** | **string** | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | [default to undefined]
**aggregatedFiatValue** | **string** | The aggregated fiat value of the vault\&#39;s balances | [optional] [default to undefined]
**balances** | [**Array&lt;V2WalletBalance&gt;**](V2WalletBalance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2GetVaultBalancesResponse } from '@palisade-inc/typescript-sdk';

const instance: V2GetVaultBalancesResponse = {
    currencyCode,
    aggregatedFiatValue,
    balances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
