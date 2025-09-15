# V2EvmFeeEstimate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gasPrice** | **string** | Gas price in wei (base_fee + priority_fee) | [default to undefined]
**baseFee** | **string** | Base Fee in wei | [default to undefined]
**priorityFee** | **string** | Average priority Fee in wei | [default to undefined]
**gasLimit** | **string** | Gas limit | [default to undefined]

## Example

```typescript
import { V2EvmFeeEstimate } from '@palisade-inc/typescript-sdk';

const instance: V2EvmFeeEstimate = {
    gasPrice,
    baseFee,
    priorityFee,
    gasLimit,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
