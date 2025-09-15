# V2UserAuthMethod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The ID of the authentication method | [default to undefined]
**type** | **string** | The type of the authentication method | [default to undefined]
**name** | **string** | A human-readable label to identify the authentication method | [default to undefined]
**createdAt** | **string** | The date and time the authenticator was created | [default to undefined]
**lastAuthedAt** | **string** | The date and time the authenticator was last used | [default to undefined]

## Example

```typescript
import { V2UserAuthMethod } from '@palisade-inc/typescript-sdk';

const instance: V2UserAuthMethod = {
    id,
    type,
    name,
    createdAt,
    lastAuthedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
