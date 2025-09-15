# V2CreateCredentialRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A helpful name to help identify the credentials | [default to undefined]
**description** | **string** | A helpful description to help identify the credentials | [optional] [default to undefined]
**category** | [**V2Category**](V2Category.md) |  | [default to undefined]
**permissions** | **Array&lt;string&gt;** | The permissions that the credential will have | [default to undefined]
**allowedIps** | **Array&lt;string&gt;** | List of IP addresses (in IP address or CIDR notation) that the credential is allowed to use | [optional] [default to undefined]

## Example

```typescript
import { V2CreateCredentialRequest } from '@palisade-inc/typescript-sdk';

const instance: V2CreateCredentialRequest = {
    name,
    description,
    category,
    permissions,
    allowedIps,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
