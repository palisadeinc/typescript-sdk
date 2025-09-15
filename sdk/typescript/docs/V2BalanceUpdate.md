# V2BalanceUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organizationId** | **string** |  | [optional] [default to undefined]
**vaultId** | **string** |  | [optional] [default to undefined]
**walletId** | **string** |  | [optional] [default to undefined]
**currencyCode** | **string** |  | [optional] [default to undefined]
**aggregatedFiatValue** | **string** |  | [optional] [default to undefined]
**assetBalances** | [**Array&lt;V2Balance&gt;**](V2Balance.md) |  | [optional] [default to undefined]
**walletBalances** | [**Array&lt;V2WalletBalance&gt;**](V2WalletBalance.md) |  | [optional] [default to undefined]
**vaultBalances** | [**Array&lt;V2VaultBalance&gt;**](V2VaultBalance.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2BalanceUpdate } from '@palisade-inc/typescript-sdk';

const instance: V2BalanceUpdate = {
    organizationId,
    vaultId,
    walletId,
    currencyCode,
    aggregatedFiatValue,
    assetBalances,
    walletBalances,
    vaultBalances,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
