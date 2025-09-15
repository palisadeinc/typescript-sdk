# V2PaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**previousPageToken** | **string** | The token to retrieve the previous page of results | [optional] [default to undefined]
**nextPageToken** | **string** | The token to retrieve the next page of results | [optional] [default to undefined]
**total** | **number** | The total number of results | [default to undefined]

## Example

```typescript
import { V2PaginationResponse } from '@palisade-inc/typescript-sdk';

const instance: V2PaginationResponse = {
    previousPageToken,
    nextPageToken,
    total,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
