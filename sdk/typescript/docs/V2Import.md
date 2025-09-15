# V2Import


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**importId** | **string** | Unique identifier for this import | [optional] [default to undefined]
**batchId** | **string** | Import batch identifier | [optional] [default to undefined]
**source** | **string** | Source of the import (e.g., \&#39;coingecko\&#39;) | [optional] [default to undefined]
**status** | **string** | Current status of the import | [optional] [default to undefined]
**triggeredBy** | **string** | User or system that triggered the import | [optional] [default to undefined]
**dryRun** | **boolean** | Whether this was a dry-run | [optional] [default to undefined]
**startedAt** | **string** | When the import started | [optional] [default to undefined]
**completedAt** | **string** | When the import completed | [optional] [default to undefined]
**totalProcessed** | **number** | Total number of items processed | [optional] [default to undefined]
**newAssets** | **number** | Number of new assets created | [optional] [default to undefined]
**updatedAssets** | **number** | Number of assets updated | [optional] [default to undefined]
**failedAssets** | **number** | Number of failed assets | [optional] [default to undefined]
**conflicts** | [**Array&lt;V2ConflictReport&gt;**](V2ConflictReport.md) | Conflicts encountered during import | [optional] [default to undefined]
**errorMessage** | **string** | Error message if import failed | [optional] [default to undefined]

## Example

```typescript
import { V2Import } from '@palisade-inc/typescript-sdk';

const instance: V2Import = {
    importId,
    batchId,
    source,
    status,
    triggeredBy,
    dryRun,
    startedAt,
    completedAt,
    totalProcessed,
    newAssets,
    updatedAssets,
    failedAssets,
    conflicts,
    errorMessage,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
