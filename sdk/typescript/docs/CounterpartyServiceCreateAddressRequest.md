# CounterpartyServiceCreateAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custodian** | [**V2Custodian**](V2Custodian.md) |  | [optional] [default to undefined]
**termsAndConditionsAccepted** | **boolean** | Whether the user has accepted the terms and conditions | [default to undefined]
**details** | [**V2AddressDetails**](V2AddressDetails.md) |  | [default to undefined]

## Example

```typescript
import { CounterpartyServiceCreateAddressRequest } from '@palisade-inc/typescript-sdk';

const instance: CounterpartyServiceCreateAddressRequest = {
    custodian,
    termsAndConditionsAccepted,
    details,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
