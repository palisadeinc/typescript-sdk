# V2Connection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The connection ID | [default to undefined]
**walletId** | **string** | The wallet ID that the connection is associated with | [default to undefined]
**vaultId** | **string** | The vault ID that the connection is associated with | [default to undefined]
**organizationId** | **string** | The organization ID that the connection is associated with | [default to undefined]
**createdBy** | **string** | The user ID that the connection is associated with | [default to undefined]
**createdAt** | **string** | The date and time the connection was created | [default to undefined]
**updatedAt** | **string** | The date and time the connection was updated | [default to undefined]
**status** | [**V2ConnectionStatus**](V2ConnectionStatus.md) |  | [default to undefined]
**proposer** | [**V2Proposer**](V2Proposer.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2Connection } from '@palisade-inc/typescript-sdk';

const instance: V2Connection = {
    id,
    walletId,
    vaultId,
    organizationId,
    createdBy,
    createdAt,
    updatedAt,
    status,
    proposer,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
