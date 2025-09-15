# V2Currency


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The human readable name of the currency | [default to undefined]
**code** | **string** | The unique currency code | [default to undefined]
**symbol** | **string** | The currency symbol | [default to undefined]
**decimals** | **number** | The number of decimal places for the currency | [optional] [readonly] [default to undefined]
**enabled** | **boolean** | Whether the currency is enabled for use | [optional] [readonly] [default to undefined]

## Example

```typescript
import { V2Currency } from '@palisade-inc/typescript-sdk';

const instance: V2Currency = {
    name,
    code,
    symbol,
    decimals,
    enabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
