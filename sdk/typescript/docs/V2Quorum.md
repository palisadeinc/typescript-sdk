# V2Quorum


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**organizationId** | **string** |  | [default to undefined]
**createdBy** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**deviceIds** | **Array&lt;string&gt;** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**operationTimeoutSeconds** | **number** |  | [default to undefined]
**sessionTimeoutSeconds** | **number** |  | [default to undefined]
**requiredSigners** | **number** |  | [default to undefined]
**state** | [**V2QuorumState**](V2QuorumState.md) |  | [default to undefined]
**type** | [**V2QuorumType**](V2QuorumType.md) |  | [default to undefined]
**backupStrategyId** | **string** |  | [optional] [default to undefined]
**modificationRequestJsonBase64** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { V2Quorum } from '@palisade-inc/typescript-sdk';

const instance: V2Quorum = {
    id,
    organizationId,
    createdBy,
    createdAt,
    updatedAt,
    description,
    deviceIds,
    name,
    operationTimeoutSeconds,
    sessionTimeoutSeconds,
    requiredSigners,
    state,
    type,
    backupStrategyId,
    modificationRequestJsonBase64,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
