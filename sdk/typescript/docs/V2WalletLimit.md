# V2WalletLimit


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The wallet limit policy ID | [default to undefined]
**createdBy** | **string** | The creator ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**walletId** | **string** | The wallet ID | [default to undefined]
**vaultId** | **string** | The vault ID | [default to undefined]
**limitQty** | **string** | The limit quantity | [optional] [default to undefined]
**duration** | **string** | The limit duration | [optional] [default to undefined]
**limitType** | [**V2LimitType**](V2LimitType.md) |  | [default to undefined]
**createdAt** | **string** | The date and time the wallet limit policy was created | [default to undefined]
**updatedAt** | **string** | The date and time the wallet limit policy was updated | [default to undefined]
**asset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [default to undefined]
**matchers** | [**Array&lt;V2Matcher&gt;**](V2Matcher.md) |  | [optional] [default to undefined]
**status** | [**V2WalletLimitStatus**](V2WalletLimitStatus.md) |  | [default to undefined]
**active** | **boolean** | Whether the limit is active | [default to undefined]

## Example

```typescript
import { V2WalletLimit } from '@palisade-inc/typescript-sdk';

const instance: V2WalletLimit = {
    id,
    createdBy,
    organizationId,
    walletId,
    vaultId,
    limitQty,
    duration,
    limitType,
    createdAt,
    updatedAt,
    asset,
    matchers,
    status,
    active,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
