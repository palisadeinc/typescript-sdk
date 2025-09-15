# V2IntFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eq** | **number** | Equals | [optional] [default to undefined]
**notEq** | **number** | Not equal to | [optional] [default to undefined]
**_in** | **Array&lt;number&gt;** | Value is in the list | [optional] [default to undefined]
**notIn** | **Array&lt;number&gt;** | Value is not in the list | [optional] [default to undefined]
**isNull** | **boolean** | Check if field is null | [optional] [default to undefined]
**gt** | **number** | Greater than | [optional] [default to undefined]
**gte** | **number** | Greater than or equal to | [optional] [default to undefined]
**lt** | **number** | Less than | [optional] [default to undefined]
**lte** | **number** | Less than or equal to | [optional] [default to undefined]

## Example

```typescript
import { V2IntFilter } from '@palisade-inc/typescript-sdk';

const instance: V2IntFilter = {
    eq,
    notEq,
    _in,
    notIn,
    isNull,
    gt,
    gte,
    lt,
    lte,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
