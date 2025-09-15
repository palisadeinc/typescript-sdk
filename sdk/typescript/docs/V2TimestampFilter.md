# V2TimestampFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eq** | **string** | Exact timestamp match | [optional] [default to undefined]
**notEq** | **string** | Not equal to timestamp | [optional] [default to undefined]
**before** | **string** | Before this timestamp | [optional] [default to undefined]
**after** | **string** | After this timestamp | [optional] [default to undefined]
**gte** | **string** | Greater than or equal to timestamp | [optional] [default to undefined]
**lte** | **string** | Less than or equal to timestamp | [optional] [default to undefined]
**between** | [**TimestampFilterTimestampRange**](TimestampFilterTimestampRange.md) |  | [optional] [default to undefined]
**isNull** | **boolean** | Check if field is null | [optional] [default to undefined]
**relativeDays** | **number** | Relative days from now (negative for past, positive for future) | [optional] [default to undefined]

## Example

```typescript
import { V2TimestampFilter } from '@palisade-inc/typescript-sdk';

const instance: V2TimestampFilter = {
    eq,
    notEq,
    before,
    after,
    gte,
    lte,
    between,
    isNull,
    relativeDays,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
