# Approvalv2Summary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sourceId** | **string** | The summary ID | [default to undefined]
**sourceType** | [**V2SourceType**](V2SourceType.md) |  | [default to undefined]
**sourceRaw** | **string** | The raw source containing the item to be approved | [default to undefined]
**expiresAt** | **string** | The date and time the approval set expires | [default to undefined]
**metAt** | **string** | The date and time the approval set was met | [optional] [default to undefined]
**currentApprovedCount** | **number** | The current number of approvals | [default to undefined]
**requiredApproverCount** | **number** | The required number of approvals | [default to undefined]
**status** | [**Approvalv2ApprovalSetStatus**](Approvalv2ApprovalSetStatus.md) |  | [default to undefined]
**requestedBy** | **string** |  | [optional] [default to undefined]
**action** | [**V2Action**](V2Action.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Approvalv2Summary } from '@palisade-inc/typescript-sdk';

const instance: Approvalv2Summary = {
    sourceId,
    sourceType,
    sourceRaw,
    expiresAt,
    metAt,
    currentApprovedCount,
    requiredApproverCount,
    status,
    requestedBy,
    action,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
