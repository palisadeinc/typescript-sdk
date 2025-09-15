# V2Webhook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The webhook ID. | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user who created this webhook | [default to undefined]
**createdAt** | **string** | The date and time the webhook was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this webhook | [default to undefined]
**updatedAt** | **string** | The date and time the webhook was updated | [default to undefined]
**name** | **string** | The webhook name | [default to undefined]
**description** | **string** | The webhook description | [optional] [default to undefined]
**endpoint** | **string** | The webhook endpoint to send data to | [default to undefined]
**subscriptionCount** | **number** | The number of subscriptions associated with the webhook | [default to undefined]
**publicKey** | **string** | The public key used to verify the webhook signature | [default to undefined]
**lastSuccess** | **string** | The timestamp of the last successful webhook delivery | [optional] [default to undefined]
**lastFailure** | **string** | The timestamp of the last failed webhook delivery | [optional] [default to undefined]
**successCount** | **number** | The number of successful webhook deliveries in the last hour | [default to undefined]
**failureCount** | **number** | The number of failed webhook deliveries in the last hour | [default to undefined]

## Example

```typescript
import { V2Webhook } from '@palisade-inc/typescript-sdk';

const instance: V2Webhook = {
    id,
    organizationId,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    name,
    description,
    endpoint,
    subscriptionCount,
    publicKey,
    lastSuccess,
    lastFailure,
    successCount,
    failureCount,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
