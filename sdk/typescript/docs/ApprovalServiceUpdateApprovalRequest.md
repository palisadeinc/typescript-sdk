# ApprovalServiceUpdateApprovalRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**signature** | **string** | The approval signature | [optional] [default to undefined]
**reasons** | **Array&lt;string&gt;** | The reasons for an approval or rejection | [default to undefined]
**status** | [**Approvalv2ApprovalStatus**](Approvalv2ApprovalStatus.md) |  | [default to undefined]

## Example

```typescript
import { ApprovalServiceUpdateApprovalRequest } from '@palisade-inc/typescript-sdk';

const instance: ApprovalServiceUpdateApprovalRequest = {
    signature,
    reasons,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
