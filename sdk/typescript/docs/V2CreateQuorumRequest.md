# V2CreateQuorumRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deviceIds** | **Array&lt;string&gt;** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**requiredSigners** | **number** |  | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**quorumType** | [**V2QuorumType**](V2QuorumType.md) |  | [default to undefined]
**backupStrategyId** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { V2CreateQuorumRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateQuorumRequest = {
    deviceIds,
    name,
    requiredSigners,
    description,
    quorumType,
    backupStrategyId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
