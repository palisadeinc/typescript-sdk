# V2GetOrgBalancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currencyCode** | **string** | The currency code to be used for the fiat value. When omitted, \&#39;USD\&#39; will be used. | [default to undefined]
**aggregatedFiatValue** | **string** | The aggregated fiat value of the organization\&#39;s balances | [optional] [default to undefined]
**balances** | [**Array&lt;V2VaultBalance&gt;**](V2VaultBalance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2GetOrgBalancesResponse } from '@palisade-inc/typescript-sdk';

const instance: V2GetOrgBalancesResponse = {
    currencyCode,
    aggregatedFiatValue,
    balances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
