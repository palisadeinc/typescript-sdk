# V2Credential


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The credential ID | [default to undefined]
**name** | **string** | The credential name | [default to undefined]
**description** | **string** | The credential description | [default to undefined]
**category** | [**V2Category**](V2Category.md) |  | [default to undefined]
**permissions** | **Array&lt;string&gt;** | The credential permissions | [default to undefined]
**createdBy** | **string** | The ID of the user who created the credential | [default to undefined]
**organizationId** | **string** | The ID of the organization who created the credential | [default to undefined]
**createdAt** | **string** | The date and time the credential was created | [default to undefined]
**updatedAt** | **string** | The date and time the credential was updated | [default to undefined]
**clientId** | **string** | The credential client ID | [default to undefined]
**clientSecret** | **string** | The credential client secret | [optional] [default to undefined]
**active** | **boolean** | The credential active status | [default to undefined]
**status** | [**V2CredentialStatus**](V2CredentialStatus.md) |  | [default to undefined]
**proposedPermissions** | **Array&lt;string&gt;** | The proposed credential permissions | [default to undefined]
**allowedIps** | **Array&lt;string&gt;** | List of IP addresses (in IP address or CIDR notation) that the credential is allowed to use | [optional] [default to undefined]

## Example

```typescript
import { V2Credential } from '@palisade-inc/typescript-sdk';

const instance: V2Credential = {
    id,
    name,
    description,
    category,
    permissions,
    createdBy,
    organizationId,
    createdAt,
    updatedAt,
    clientId,
    clientSecret,
    active,
    status,
    proposedPermissions,
    allowedIps,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
