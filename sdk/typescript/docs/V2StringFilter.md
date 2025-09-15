# V2StringFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eq** | **string** | Exact match | [optional] [default to undefined]
**notEq** | **string** | Not equal to | [optional] [default to undefined]
**contains** | **string** | Contains substring (case-insensitive) | [optional] [default to undefined]
**startsWith** | **string** | Starts with prefix (case-insensitive) | [optional] [default to undefined]
**endsWith** | **string** | Ends with suffix (case-insensitive) | [optional] [default to undefined]
**_in** | **Array&lt;string&gt;** | Value is in the list | [optional] [default to undefined]
**notIn** | **Array&lt;string&gt;** | Value is not in the list | [optional] [default to undefined]
**regex** | **string** | Regular expression match | [optional] [default to undefined]
**isNull** | **boolean** | Check if field is null | [optional] [default to undefined]
**fuzzy** | [**V2FuzzyMatch**](V2FuzzyMatch.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2StringFilter } from '@palisade-inc/typescript-sdk';

const instance: V2StringFilter = {
    eq,
    notEq,
    contains,
    startsWith,
    endsWith,
    _in,
    notIn,
    regex,
    isNull,
    fuzzy,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
