# V2InternalDecompileTransactionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [optional] [default to undefined]
**destinationAddress** | **string** |  | [optional] [default to undefined]
**qty** | **string** |  | [optional] [default to undefined]
**feeQtyLimit** | **string** |  | [optional] [default to undefined]
**sequence** | **string** |  | [optional] [default to undefined]
**transactionType** | **string** |  | [optional] [default to undefined]
**attributes** | **{ [key: string]: string; }** |  | [optional] [default to undefined]
**originAddress** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { V2InternalDecompileTransactionResponse } from '@palisade-inc/typescript-sdk';

const instance: V2InternalDecompileTransactionResponse = {
    asset,
    destinationAddress,
    qty,
    feeQtyLimit,
    sequence,
    transactionType,
    attributes,
    originAddress,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
