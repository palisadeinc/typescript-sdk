# V2Counterparty


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The counterparty ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user who created this counterparty | [default to undefined]
**createdAt** | **string** | The date and time the counterparty was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this counterparty | [default to undefined]
**updatedAt** | **string** | The date and time the counterparty was updated | [default to undefined]
**name** | **string** | The counterparty name | [default to undefined]
**description** | **string** | The counterparty description | [optional] [default to undefined]
**details** | [**V2CounterpartyDetails**](V2CounterpartyDetails.md) |  | [default to undefined]
**addressCount** | **number** | The number of addresses associated with the counterparty | [default to undefined]

## Example

```typescript
import { V2Counterparty } from '@palisade-inc/typescript-sdk';

const instance: V2Counterparty = {
    id,
    organizationId,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    name,
    description,
    details,
    addressCount,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
