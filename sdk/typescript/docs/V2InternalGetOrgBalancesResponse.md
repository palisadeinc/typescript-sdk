# V2InternalGetOrgBalancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currencyCode** | **string** |  | [optional] [default to undefined]
**aggregatedFiatValue** | **string** |  | [optional] [default to undefined]
**balances** | [**Array&lt;V2VaultBalance&gt;**](V2VaultBalance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2InternalGetOrgBalancesResponse } from '@palisade-inc/typescript-sdk';

const instance: V2InternalGetOrgBalancesResponse = {
    currencyCode,
    aggregatedFiatValue,
    balances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
