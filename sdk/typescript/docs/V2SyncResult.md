# V2SyncResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**importId** | **string** | Unique identifier for this import | [optional] [default to undefined]
**totalProcessed** | **number** | Total number of assets processed | [optional] [default to undefined]
**newAssets** | **number** | Number of new assets created | [optional] [default to undefined]
**updatedAssets** | **number** | Number of existing assets updated | [optional] [default to undefined]
**failedAssets** | **number** | Number of assets that failed to process | [optional] [default to undefined]
**conflicts** | [**Array&lt;V2ConflictReport&gt;**](V2ConflictReport.md) | List of conflicts encountered during sync | [optional] [default to undefined]
**startedAt** | **string** | When the sync started | [optional] [default to undefined]
**completedAt** | **string** | When the sync completed | [optional] [default to undefined]

## Example

```typescript
import { V2SyncResult } from '@palisade-inc/typescript-sdk';

const instance: V2SyncResult = {
    importId,
    totalProcessed,
    newAssets,
    updatedAssets,
    failedAssets,
    conflicts,
    startedAt,
    completedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
