# V2BlockchainInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**name** | **string** | Human-readable name of the blockchain | [default to undefined]
**namespace** | **string** | The CAIP-2 namespace identifier | [default to undefined]
**chainId** | **string** | The chain ID (supports large numbers) | [default to undefined]
**rpcEndpoints** | [**Array&lt;V2RPCEndpoint&gt;**](V2RPCEndpoint.md) | RPC endpoints for blockchain connectivity | [optional] [default to undefined]
**supportedEvents** | **Array&lt;string&gt;** | WalletConnect event types supported by this blockchain | [optional] [default to undefined]
**supportedMethods** | **Array&lt;string&gt;** | WalletConnect methods supported by this blockchain | [optional] [default to undefined]
**keystoreTypes** | [**Array&lt;V2Keystore&gt;**](V2Keystore.md) | Supported keystore types (HSM, MPC) | [optional] [default to undefined]
**keyAlgorithms** | [**Array&lt;V2KeyAlgorithm&gt;**](V2KeyAlgorithm.md) | Supported key algorithms | [optional] [default to undefined]
**routing** | **string** | Message queue routing key base | [default to undefined]
**status** | [**V2BlockchainStatus**](V2BlockchainStatus.md) |  | [default to undefined]
**supportsWalletConnect** | **boolean** | Whether this blockchain supports WalletConnect | [optional] [default to undefined]
**explorers** | [**Array&lt;V2Explorer&gt;**](V2Explorer.md) | Blockchain explorers for viewing transactions and addresses | [optional] [default to undefined]
**createdAt** | **string** | When the blockchain was created | [optional] [readonly] [default to undefined]
**updatedAt** | **string** | When the blockchain was last updated | [optional] [readonly] [default to undefined]
**chain** | **string** | Chain identifier (e.g., \&#39;ethereum-mainnet\&#39;, \&#39;ethereum-goerli\&#39;) | [optional] [default to undefined]
**coingeckoPlatformId** | **string** | CoinGecko platform identifier for sync (optional for testnets) | [optional] [default to undefined]
**checksumType** | [**V2ChecksumType**](V2ChecksumType.md) |  | [optional] [default to undefined]
**blockTime** | **number** | Average block time in seconds | [optional] [default to undefined]
**confirmationBlocks** | **number** | Recommended number of confirmations for finality | [optional] [default to undefined]

## Example

```typescript
import { V2BlockchainInfo } from '@palisade-inc/typescript-sdk';

const instance: V2BlockchainInfo = {
    id,
    name,
    namespace,
    chainId,
    rpcEndpoints,
    supportedEvents,
    supportedMethods,
    keystoreTypes,
    keyAlgorithms,
    routing,
    status,
    supportsWalletConnect,
    explorers,
    createdAt,
    updatedAt,
    chain,
    coingeckoPlatformId,
    checksumType,
    blockTime,
    confirmationBlocks,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
