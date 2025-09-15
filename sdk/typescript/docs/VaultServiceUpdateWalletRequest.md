# VaultServiceUpdateWalletRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The name of the wallet | [default to undefined]
**description** | **string** | The description of the wallet | [optional] [default to undefined]
**correlationId** | **string** | Correlation ID for tracking correlated actions on the wallet | [optional] [default to undefined]

## Example

```typescript
import { VaultServiceUpdateWalletRequest } from '@palisade-inc/typescript-sdk';

const instance: VaultServiceUpdateWalletRequest = {
    name,
    description,
    correlationId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
