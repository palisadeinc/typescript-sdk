# V2SearchOptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**caseSensitive** | **boolean** | Enable case-sensitive search (default: false) | [optional] [default to undefined]
**minTermLength** | **number** | Minimum search term length | [optional] [default to undefined]
**maxResults** | **number** | Maximum number of results to return | [optional] [default to undefined]
**multiTermAnd** | **boolean** | Use AND logic for multiple terms (default: false for OR) | [optional] [default to undefined]

## Example

```typescript
import { V2SearchOptions } from '@palisade-inc/typescript-sdk';

const instance: V2SearchOptions = {
    caseSensitive,
    minTermLength,
    maxResults,
    multiTermAnd,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
