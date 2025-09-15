# V2Balance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [optional] [default to undefined]
**balance** | **string** | The total balance of the asset on the blockchain. When breakdown fields are present, this equals available_balance + pending_balance + frozen_balance | [optional] [default to undefined]
**rate** | **string** | The exchange rate between the asset and \&#39;currencyCode\&#39; | [optional] [default to undefined]
**fiatValue** | **string** | The aggregated fiat value of an asset for a wallet | [optional] [default to undefined]
**availableBalance** | **string** | The available balance that can be spent | [optional] [default to undefined]
**pendingBalance** | **string** | The balance tied up in pending transactions | [optional] [default to undefined]
**frozenBalance** | **string** | The balance frozen by policy actions | [optional] [default to undefined]

## Example

```typescript
import { V2Balance } from '@palisade-inc/typescript-sdk';

const instance: V2Balance = {
    asset,
    balance,
    rate,
    fiatValue,
    availableBalance,
    pendingBalance,
    frozenBalance,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
