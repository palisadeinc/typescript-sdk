# Approvalv2Approval


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The approval ID | [default to undefined]
**approvalSetId** | **string** | The approval set ID | [default to undefined]
**userId** | **string** | The user ID | [default to undefined]
**createdAt** | **string** | The date and time the approval was created | [default to undefined]
**updatedAt** | **string** | The date and time the approval was updated | [default to undefined]
**signature** | **string** | The signed approval | [optional] [default to undefined]
**reasons** | **Array&lt;string&gt;** | The reasons for an approval or rejection | [default to undefined]
**status** | [**Approvalv2ApprovalStatus**](Approvalv2ApprovalStatus.md) |  | [default to undefined]

## Example

```typescript
import { Approvalv2Approval } from '@palisade-inc/typescript-sdk';

const instance: Approvalv2Approval = {
    id,
    approvalSetId,
    userId,
    createdAt,
    updatedAt,
    signature,
    reasons,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
