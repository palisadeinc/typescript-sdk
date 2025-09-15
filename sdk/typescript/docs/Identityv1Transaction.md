# Identityv1Transaction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**attributes** | **{ [key: string]: string; }** |  | [optional] [default to undefined]
**status** | [**Identityv1TransactionStatus**](Identityv1TransactionStatus.md) |  | [optional] [default to undefined]
**action** | [**Identityv1TransactionAction**](Identityv1TransactionAction.md) |  | [optional] [default to undefined]
**encodedTransaction** | **string** |  | [optional] [default to undefined]
**signature** | **string** |  | [optional] [default to undefined]
**canonicalSignature** | **string** |  | [optional] [default to undefined]
**signedTransaction** | **string** |  | [optional] [default to undefined]
**signOnly** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { Identityv1Transaction } from '@palisade-inc/typescript-sdk';

const instance: Identityv1Transaction = {
    id,
    attributes,
    status,
    action,
    encodedTransaction,
    signature,
    canonicalSignature,
    signedTransaction,
    signOnly,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
