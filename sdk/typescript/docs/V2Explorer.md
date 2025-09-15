# V2Explorer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the explorer | [default to undefined]
**url** | **string** | Base URL of the explorer | [default to undefined]
**transactionFormat** | **string** | URL format for transaction links (use {txHash} as placeholder) | [default to undefined]
**addressFormat** | **string** | URL format for address links (use {address} as placeholder) | [default to undefined]

## Example

```typescript
import { V2Explorer } from '@palisade-inc/typescript-sdk';

const instance: V2Explorer = {
    name,
    url,
    transactionFormat,
    addressFormat,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
