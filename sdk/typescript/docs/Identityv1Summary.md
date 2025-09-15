# Identityv1Summary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sourceId** | **string** |  | [optional] [default to undefined]
**sourceType** | [**V1SummarySourceType**](V1SummarySourceType.md) |  | [optional] [default to undefined]
**sourceRaw** | **string** |  | [optional] [default to undefined]
**expiresAt** | **string** |  | [optional] [default to undefined]
**metAt** | **string** |  | [optional] [default to undefined]
**currentApprovedCount** | **number** |  | [optional] [default to undefined]
**requiredApproverCount** | **number** |  | [optional] [default to undefined]
**status** | [**Identityv1ApprovalSetStatus**](Identityv1ApprovalSetStatus.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Identityv1Summary } from '@palisade-inc/typescript-sdk';

const instance: Identityv1Summary = {
    sourceId,
    sourceType,
    sourceRaw,
    expiresAt,
    metAt,
    currentApprovedCount,
    requiredApproverCount,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
