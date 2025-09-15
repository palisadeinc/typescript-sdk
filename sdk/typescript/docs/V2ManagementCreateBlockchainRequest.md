# V2ManagementCreateBlockchainRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**name** | **string** | Blockchain name | [default to undefined]
**namespace** | **string** | Blockchain namespace | [default to undefined]
**chain** | **string** | Chain identifier | [optional] [default to undefined]
**chainId** | **string** | Chain ID (for EVM chains) | [optional] [default to undefined]
**routing** | **string** | Routing configuration | [optional] [default to undefined]
**status** | [**V2BlockchainStatus**](V2BlockchainStatus.md) |  | [default to undefined]
**supportsWalletConnect** | **boolean** | Whether blockchain supports WalletConnect | [optional] [default to undefined]
**rpcEndpoints** | [**Array&lt;V2RPCEndpoint&gt;**](V2RPCEndpoint.md) | RPC endpoints for the blockchain | [optional] [default to undefined]
**explorers** | [**Array&lt;V2Explorer&gt;**](V2Explorer.md) | Block explorers for the blockchain | [optional] [default to undefined]
**keystoreTypes** | [**Array&lt;V2Keystore&gt;**](V2Keystore.md) | Supported keystore types | [optional] [default to undefined]
**keyAlgorithms** | [**Array&lt;V2KeyAlgorithm&gt;**](V2KeyAlgorithm.md) | Supported key algorithms | [optional] [default to undefined]
**supportedEvents** | **Array&lt;string&gt;** | Supported blockchain events | [optional] [default to undefined]
**supportedMethods** | **Array&lt;string&gt;** | Supported blockchain methods | [optional] [default to undefined]

## Example

```typescript
import { V2ManagementCreateBlockchainRequest } from '@palisade-inc/typescript-sdk';

const instance: V2ManagementCreateBlockchainRequest = {
    id,
    name,
    namespace,
    chain,
    chainId,
    routing,
    status,
    supportsWalletConnect,
    rpcEndpoints,
    explorers,
    keystoreTypes,
    keyAlgorithms,
    supportedEvents,
    supportedMethods,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
