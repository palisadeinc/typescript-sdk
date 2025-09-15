# V2Vault


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The vault ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The user ID that created the vault | [default to undefined]
**createdAt** | **string** | The date and time the vault was created | [default to undefined]
**updatedAt** | **string** | The date and time the vault was updated | [default to undefined]
**name** | **string** | The name of the vault | [default to undefined]
**description** | **string** | The description of the vault | [optional] [default to undefined]
**externalId** | **string** | External ID of this vault, unique to the organization | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for the vault | [optional] [default to undefined]

## Example

```typescript
import { V2Vault } from '@palisade-inc/typescript-sdk';

const instance: V2Vault = {
    id,
    organizationId,
    createdBy,
    createdAt,
    updatedAt,
    name,
    description,
    externalId,
    correlationId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
