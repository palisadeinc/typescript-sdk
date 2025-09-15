# V2FeeEstimate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**evm** | [**V2EvmFeeEstimate**](V2EvmFeeEstimate.md) |  | [optional] [default to undefined]
**networkFees** | **{ [key: string]: string; }** | Map of fee options where keys are fee types (slowest, slow, medium, fast, fastest) and values are the fee amounts in base asset units | [default to undefined]

## Example

```typescript
import { V2FeeEstimate } from '@palisade-inc/typescript-sdk';

const instance: V2FeeEstimate = {
    evm,
    networkFees,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
