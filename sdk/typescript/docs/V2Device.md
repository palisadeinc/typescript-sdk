# V2Device


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The device ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The user ID that created the device | [default to undefined]
**createdAt** | **string** | The date and time the device was created | [default to undefined]
**pairedAt** | **string** | The date and time the device was paired | [default to undefined]
**updatedAt** | **string** | The date and time the device was updated | [default to undefined]
**clientId** | **string** | The client ID | [optional] [default to undefined]
**displayName** | **string** | The name of the device | [default to undefined]
**approvalStatus** | [**Devicev2ApprovalStatus**](Devicev2ApprovalStatus.md) |  | [default to undefined]
**enabledStatus** | [**V2EnabledStatus**](V2EnabledStatus.md) |  | [default to undefined]
**publicKeyHash** | **string** | The hash of the devices public key | [default to undefined]
**deleted** | **boolean** | Whether the device has been deleted | [default to undefined]
**deviceType** | [**V2DeviceType**](V2DeviceType.md) |  | [default to undefined]
**playerId** | **number** | The player ID | [optional] [default to undefined]
**version** | **string** | The version of the device | [optional] [default to undefined]

## Example

```typescript
import { V2Device } from '@palisade-inc/typescript-sdk';

const instance: V2Device = {
    id,
    organizationId,
    createdBy,
    createdAt,
    pairedAt,
    updatedAt,
    clientId,
    displayName,
    approvalStatus,
    enabledStatus,
    publicKeyHash,
    deleted,
    deviceType,
    playerId,
    version,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
