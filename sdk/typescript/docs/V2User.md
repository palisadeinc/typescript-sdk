# V2User


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The user ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**firstName** | **string** | The users first name | [default to undefined]
**lastName** | **string** | The users last name | [default to undefined]
**email** | **string** | The users email | [default to undefined]
**roles** | [**Array&lt;V2Role&gt;**](V2Role.md) | The roles that the user has | [default to undefined]
**createdBy** | **string** | The ID of the user who created this user | [default to undefined]
**createdAt** | **string** | The date and time the user was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this user | [default to undefined]
**updatedAt** | **string** | The date and time the user was updated | [default to undefined]
**status** | [**V2UserStatus**](V2UserStatus.md) |  | [default to undefined]
**blockedBy** | **string** | The ID of the user who blocked this user | [optional] [default to undefined]
**blockedReason** | **string** | The reason the user was blocked | [optional] [default to undefined]
**authLoginCount** | **number** | The number of time the user has logged in | [optional] [default to undefined]
**authLastLogin** | **string** | The date and time the user last logged in | [optional] [default to undefined]
**authLastPasswordReset** | **string** | The date and time the user last reset their password | [optional] [default to undefined]
**authLastIp** | **string** | The last IP address from which this user logged in | [optional] [default to undefined]
**picture** | **string** | A link to the users gravatar image | [optional] [default to undefined]
**proposedFirstName** | **string** | The proposed first name for the user | [optional] [default to undefined]
**proposedUpdatedBy** | **string** | The ID of the user who proposed the update | [optional] [default to undefined]
**proposedLastName** | **string** | The proposed last name for the user | [optional] [default to undefined]
**proposedRoles** | [**Array&lt;V2Role&gt;**](V2Role.md) | The proposed roles for the user | [optional] [default to undefined]
**proposedBlockedReason** | **string** | The proposed reason the user was blocked | [optional] [default to undefined]

## Example

```typescript
import { V2User } from '@palisade-inc/typescript-sdk';

const instance: V2User = {
    id,
    organizationId,
    firstName,
    lastName,
    email,
    roles,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    status,
    blockedBy,
    blockedReason,
    authLoginCount,
    authLastLogin,
    authLastPasswordReset,
    authLastIp,
    picture,
    proposedFirstName,
    proposedUpdatedBy,
    proposedLastName,
    proposedRoles,
    proposedBlockedReason,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
