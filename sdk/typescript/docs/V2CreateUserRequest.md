# V2CreateUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**firstName** | **string** | The users first name | [default to undefined]
**lastName** | **string** | The users last name | [default to undefined]
**email** | **string** | The users email | [default to undefined]
**roles** | [**Array&lt;V2Role&gt;**](V2Role.md) | The roles that the user has | [default to undefined]

## Example

```typescript
import { V2CreateUserRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateUserRequest = {
    firstName,
    lastName,
    email,
    roles,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
