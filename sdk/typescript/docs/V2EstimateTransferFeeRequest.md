# V2EstimateTransferFeeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**contract** | **string** | The contract/issuing address | [optional] [default to undefined]
**symbol** | **string** | The asset symbol | [default to undefined]
**originAddress** | **string** | The origin address | [default to undefined]

## Example

```typescript
import { V2EstimateTransferFeeRequest } from '@palisade-inc/typescript-sdk';

const instance: V2EstimateTransferFeeRequest = {
    blockchain,
    contract,
    symbol,
    originAddress,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
