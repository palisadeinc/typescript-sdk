# V2ManagementCreateCurrencyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | ISO 4217 currency code | [default to undefined]
**name** | **string** | Currency name | [default to undefined]
**symbol** | **string** | Currency symbol | [default to undefined]
**decimals** | **number** | Number of decimal places (default: 2) | [optional] [default to undefined]
**enabled** | **boolean** | Whether the currency is enabled (default: true) | [optional] [default to undefined]

## Example

```typescript
import { V2ManagementCreateCurrencyRequest } from '@palisade-inc/typescript-sdk';

const instance: V2ManagementCreateCurrencyRequest = {
    code,
    name,
    symbol,
    decimals,
    enabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
