# Transactionsv2Address


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Either addressID or walletID, or allowAddressID, or not set when the address does not exist within palisade e.g. a deposit from outside of Palisade | [optional] [default to undefined]
**organizationId** | **string** | The organization ID | [optional] [default to undefined]
**counterpartyId** | **string** | The counterparty ID | [optional] [default to undefined]
**vaultId** | **string** | The vault ID | [optional] [default to undefined]
**type** | [**Transactionsv2AddressType**](Transactionsv2AddressType.md) |  | [default to undefined]
**address** | **string** | The address | [default to undefined]

## Example

```typescript
import { Transactionsv2Address } from '@palisade-inc/typescript-sdk';

const instance: Transactionsv2Address = {
    id,
    organizationId,
    counterpartyId,
    vaultId,
    type,
    address,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
