# V2FreezeHistoryEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for this history entry | [optional] [default to undefined]
**action** | [**V2FreezeAction**](V2FreezeAction.md) |  | [optional] [default to undefined]
**reason** | **string** | Reason for the freeze or unfreeze action | [optional] [default to undefined]
**userId** | **string** | User who performed the action (empty for automatic actions) | [optional] [default to undefined]
**organizationId** | **string** | Organization of the user who performed the action (empty for automatic actions) | [optional] [default to undefined]
**performedAt** | **string** | Timestamp when the action was performed | [optional] [default to undefined]
**freezeType** | [**V2FreezeType**](V2FreezeType.md) |  | [optional] [default to undefined]
**riskScore** | **number** | Risk score that triggered auto-freeze (0-100) | [optional] [default to undefined]

## Example

```typescript
import { V2FreezeHistoryEntry } from '@palisade-inc/typescript-sdk';

const instance: V2FreezeHistoryEntry = {
    id,
    action,
    reason,
    userId,
    organizationId,
    performedAt,
    freezeType,
    riskScore,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
