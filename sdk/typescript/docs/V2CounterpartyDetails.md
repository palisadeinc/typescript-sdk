# V2CounterpartyDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**V2CounterpartyType**](V2CounterpartyType.md) |  | [default to undefined]
**individual** | [**V2Individual**](V2Individual.md) |  | [optional] [default to undefined]
**organization** | [**Counterpartyv2Organization**](Counterpartyv2Organization.md) |  | [optional] [default to undefined]
**dApp** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { V2CounterpartyDetails } from '@palisade-inc/typescript-sdk';

const instance: V2CounterpartyDetails = {
    type,
    individual,
    organization,
    dApp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
