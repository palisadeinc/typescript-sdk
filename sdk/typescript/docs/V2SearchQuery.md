# V2SearchQuery


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**term** | **string** | Search term | [optional] [default to undefined]
**fields** | **Array&lt;string&gt;** | Fields to search in | [optional] [default to undefined]
**type** | [**V2SearchType**](V2SearchType.md) |  | [optional] [default to undefined]
**minScore** | **number** | Minimum relevance score for fuzzy/fulltext search | [optional] [default to undefined]
**_options** | [**V2SearchOptions**](V2SearchOptions.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2SearchQuery } from '@palisade-inc/typescript-sdk';

const instance: V2SearchQuery = {
    term,
    fields,
    type,
    minScore,
    _options,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
