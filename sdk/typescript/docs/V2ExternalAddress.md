# V2ExternalAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **string** | The address | [default to undefined]
**name** | **string** | The address name | [default to undefined]
**description** | **string** | The address description | [optional] [default to undefined]
**blockchains** | [**Array&lt;V2Blockchain&gt;**](V2Blockchain.md) | The blockchains supported by the address | [default to undefined]

## Example

```typescript
import { V2ExternalAddress } from '@palisade-inc/typescript-sdk';

const instance: V2ExternalAddress = {
    address,
    name,
    description,
    blockchains,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
