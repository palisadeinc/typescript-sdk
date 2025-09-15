# V2OrganizationAuthMethod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The ID of the authentication method | [default to undefined]
**name** | **string** | The name of the authentication method | [default to undefined]
**strategy** | **string** | The strategy of the authentication method | [default to undefined]
**_default** | **boolean** | Whether this is the default authentication method for the organization | [default to undefined]
**idpSettings** | [**V2OrganizationAuthMethodIdpSettings**](V2OrganizationAuthMethodIdpSettings.md) |  | [default to undefined]

## Example

```typescript
import { V2OrganizationAuthMethod } from '@palisade-inc/typescript-sdk';

const instance: V2OrganizationAuthMethod = {
    id,
    name,
    strategy,
    _default,
    idpSettings,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
