# VaultServiceUpdateVaultRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The name of the vault | [default to undefined]
**description** | **string** | The description of the vault | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for tracking various actions on the vault | [optional] [default to undefined]

## Example

```typescript
import { VaultServiceUpdateVaultRequest } from '@palisade-inc/typescript-sdk';

const instance: VaultServiceUpdateVaultRequest = {
    name,
    description,
    correlationId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
