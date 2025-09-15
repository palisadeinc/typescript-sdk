# V2CreateWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The webhook name. | [default to undefined]
**description** | **string** | The webhook description. | [optional] [default to undefined]
**endpoint** | **string** | The webhook endpoint to send data to | [default to undefined]

## Example

```typescript
import { V2CreateWebhookRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateWebhookRequest = {
    name,
    description,
    endpoint,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
