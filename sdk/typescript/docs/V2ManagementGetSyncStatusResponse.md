# V2ManagementGetSyncStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **boolean** | Whether sync is enabled | [optional] [default to undefined]
**running** | **boolean** | Whether sync is currently running | [optional] [default to undefined]
**schedule** | **string** | Cron schedule for automatic sync | [optional] [default to undefined]
**nextRun** | **string** | Next scheduled sync time | [optional] [default to undefined]
**dryRun** | **boolean** | Whether dry-run mode is enabled | [optional] [default to undefined]
**batchSize** | **number** | Batch size for processing | [optional] [default to undefined]

## Example

```typescript
import { V2ManagementGetSyncStatusResponse } from '@palisade-inc/typescript-sdk';

const instance: V2ManagementGetSyncStatusResponse = {
    enabled,
    running,
    schedule,
    nextRun,
    dryRun,
    batchSize,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
