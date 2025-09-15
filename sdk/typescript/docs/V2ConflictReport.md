# V2ConflictReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assetId** | **string** | ID of the asset with conflict | [optional] [default to undefined]
**existingSource** | **string** | Source of existing asset data | [optional] [default to undefined]
**newSource** | **string** | Source of new asset data | [optional] [default to undefined]
**resolution** | **string** | How the conflict was resolved | [optional] [default to undefined]
**reason** | **string** | Reason for the resolution | [optional] [default to undefined]

## Example

```typescript
import { V2ConflictReport } from '@palisade-inc/typescript-sdk';

const instance: V2ConflictReport = {
    assetId,
    existingSource,
    newSource,
    resolution,
    reason,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
