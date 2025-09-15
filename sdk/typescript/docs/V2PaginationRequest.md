# V2PaginationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pageSize** | **number** | Number of results per page (default 50, max 1000) | [optional] [default to undefined]
**pageToken** | **string** | Token for pagination from previous response | [optional] [default to undefined]
**orderBy** | **string** | Field to order results by | [optional] [default to undefined]
**order** | [**V2SortOrder**](V2SortOrder.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2PaginationRequest } from '@palisade-inc/typescript-sdk';

const instance: V2PaginationRequest = {
    pageSize,
    pageToken,
    orderBy,
    order,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
