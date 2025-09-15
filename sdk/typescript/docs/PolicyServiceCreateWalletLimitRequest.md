# PolicyServiceCreateWalletLimitRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limitQty** | **string** | The limit quantity | [default to undefined]
**duration** | **string** | The limit duration | [optional] [default to undefined]
**limitType** | [**V2LimitType**](V2LimitType.md) |  | [default to undefined]
**contract** | **string** | The contract/issuing address | [optional] [default to undefined]
**symbol** | **string** | The asset symbol | [default to undefined]
**matchers** | [**Array&lt;V2Matcher&gt;**](V2Matcher.md) |  | [optional] [default to undefined]

## Example

```typescript
import { PolicyServiceCreateWalletLimitRequest } from '@palisade-inc/typescript-sdk';

const instance: PolicyServiceCreateWalletLimitRequest = {
    limitQty,
    duration,
    limitType,
    contract,
    symbol,
    matchers,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
