# V2Session


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**organizationId** | **string** |  | [default to undefined]
**membershipId** | **string** |  | [default to undefined]
**sessionSetId** | **string** |  | [default to undefined]
**createdBy** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**expiresAt** | **string** |  | [default to undefined]
**type** | [**V2SessionType**](V2SessionType.md) |  | [default to undefined]
**accepted** | **boolean** |  | [default to undefined]
**payloadId** | **string** |  | [default to undefined]
**devicePayload** | **string** |  | [default to undefined]
**notificationPayload** | **string** |  | [default to undefined]
**notificationTrigger** | **string** |  | [default to undefined]
**notificationBody** | **string** |  | [default to undefined]
**state** | [**V2SessionState**](V2SessionState.md) |  | [default to undefined]

## Example

```typescript
import { V2Session } from '@palisade-inc/typescript-sdk';

const instance: V2Session = {
    id,
    organizationId,
    membershipId,
    sessionSetId,
    createdBy,
    createdAt,
    updatedAt,
    expiresAt,
    type,
    accepted,
    payloadId,
    devicePayload,
    notificationPayload,
    notificationTrigger,
    notificationBody,
    state,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
