# V2RPCEndpoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **string** | The RPC endpoint URL | [default to undefined]
**priority** | **number** | Priority for endpoint selection (lower number &#x3D; higher priority) | [optional] [default to undefined]
**type** | [**V2RPCEndpointType**](V2RPCEndpointType.md) |  | [default to undefined]

## Example

```typescript
import { V2RPCEndpoint } from '@palisade-inc/typescript-sdk';

const instance: V2RPCEndpoint = {
    url,
    priority,
    type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
