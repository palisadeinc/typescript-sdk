# V2Subscription


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The webhook subscription ID | [default to undefined]
**webhookId** | **string** | The webhook ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user who created this webhook | [default to undefined]
**createdAt** | **string** | The date and time the webhook was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this webhook | [default to undefined]
**updatedAt** | **string** | The date and time the webhook was updated | [default to undefined]
**config** | [**V2SubscriptionConfig**](V2SubscriptionConfig.md) |  | [default to undefined]

## Example

```typescript
import { V2Subscription } from '@palisade-inc/typescript-sdk';

const instance: V2Subscription = {
    id,
    webhookId,
    organizationId,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    config,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
