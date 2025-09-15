# Counterpartyv2Address


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addressId** | **string** | The address ID | [default to undefined]
**counterpartyId** | **string** | The counterparty ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user who created this address | [default to undefined]
**createdAt** | **string** | The date and time the address was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this address | [default to undefined]
**updatedAt** | **string** | The date and time the address was updated | [default to undefined]
**custodian** | [**V2Custodian**](V2Custodian.md) |  | [optional] [default to undefined]
**termsAndConditionsAccepted** | **boolean** | Whether the user has accepted the terms and conditions | [default to undefined]
**details** | [**V2AddressDetails**](V2AddressDetails.md) |  | [default to undefined]
**status** | [**V2AddressStatus**](V2AddressStatus.md) |  | [default to undefined]
**active** | **boolean** | Whether the address is active | [default to undefined]

## Example

```typescript
import { Counterpartyv2Address } from '@palisade-inc/typescript-sdk';

const instance: Counterpartyv2Address = {
    addressId,
    counterpartyId,
    organizationId,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    custodian,
    termsAndConditionsAccepted,
    details,
    status,
    active,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
