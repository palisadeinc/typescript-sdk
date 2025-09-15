# Transactionsv2Transaction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The transaction ID | [default to undefined]
**walletId** | **string** | The wallet ID | [default to undefined]
**vaultId** | **string** | The vault ID | [default to undefined]
**organizationId** | **string** | The organization ID | [default to undefined]
**createdBy** | **string** | The ID of the user that created the transaction | [default to undefined]
**createdAt** | **string** | The date and time the transaction was created | [default to undefined]
**updatedAt** | **string** | The date and time the transaction was updated | [default to undefined]
**attributes** | **{ [key: string]: string; }** |  | [optional] [default to undefined]
**status** | [**Transactionsv2TransactionStatus**](Transactionsv2TransactionStatus.md) |  | [default to undefined]
**action** | [**Transactionsv2TransactionAction**](Transactionsv2TransactionAction.md) |  | [default to undefined]
**externalId** | **string** | External ID of this transaction, unique to the organization | [optional] [default to undefined]
**correlationId** | **string** | The correlation ID of the transaction, used to link related transactions | [optional] [default to undefined]
**asset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [default to undefined]
**feeAsset** | [**Commonv2Asset**](Commonv2Asset.md) |  | [default to undefined]
**blockchain** | [**V2Blockchain**](V2Blockchain.md) |  | [default to undefined]
**destinationAddress** | **string** | The destination address | [optional] [default to undefined]
**destination** | [**Transactionsv2Address**](Transactionsv2Address.md) |  | [optional] [default to undefined]
**originAddress** | **string** | The origin address | [default to undefined]
**origin** | [**Transactionsv2Address**](Transactionsv2Address.md) |  | [default to undefined]
**qty** | **string** | The quantity of the asset to transfer | [default to undefined]
**feeQtyLimit** | **string** | The maximum network fee to pay for this transaction in base asset units (eg ETH for Ethereum) | [optional] [default to undefined]
**sequence** | **string** | The blockchain nonce/sequence to use | [optional] [default to undefined]
**encodedTransaction** | **string** | The encoded transaction | [optional] [default to undefined]
**signOnly** | **boolean** | Whether to only sign the transaction, or also publish it to the blockchain | [default to undefined]
**config** | [**V2XRPTransactionConfig**](V2XRPTransactionConfig.md) |  | [optional] [default to undefined]
**freezeInfo** | [**V2FreezeInfo**](V2FreezeInfo.md) |  | [default to undefined]
**feeQty** | **string** | The actual network fee for this transaction in base asset units (eg ETH for Ethereum) | [optional] [default to undefined]
**hash** | **string** | The transaction hash | [optional] [default to undefined]
**signingHash** | **string** | The transaction signing hash | [optional] [default to undefined]
**signature** | **string** | The transaction signature | [optional] [default to undefined]
**transactionType** | **string** | The transaction type | [optional] [default to undefined]
**reasons** | **Array&lt;string&gt;** | The reasons for transaction failure | [optional] [default to undefined]
**canonicalSignature** | **string** | The canonical transaction signature | [optional] [default to undefined]
**signedTransaction** | **string** | The signed transaction (multi-sign is not supported) | [optional] [default to undefined]
**proposedAssetChanges** | [**Array&lt;V2AssetChange&gt;**](V2AssetChange.md) | Proposed asset changes | [optional] [default to undefined]
**confirmedAssetChanges** | [**Array&lt;V2AssetChange&gt;**](V2AssetChange.md) | Confirmed asset changes | [optional] [default to undefined]
**signingPayloads** | [**Array&lt;V2SigningPayload&gt;**](V2SigningPayload.md) | Multiple signing payloads for UTXO-based transactions, one per input | [optional] [default to undefined]

## Example

```typescript
import { Transactionsv2Transaction } from '@palisade-inc/typescript-sdk';

const instance: Transactionsv2Transaction = {
    id,
    walletId,
    vaultId,
    organizationId,
    createdBy,
    createdAt,
    updatedAt,
    attributes,
    status,
    action,
    externalId,
    correlationId,
    asset,
    feeAsset,
    blockchain,
    destinationAddress,
    destination,
    originAddress,
    origin,
    qty,
    feeQtyLimit,
    sequence,
    encodedTransaction,
    signOnly,
    config,
    freezeInfo,
    feeQty,
    hash,
    signingHash,
    signature,
    transactionType,
    reasons,
    canonicalSignature,
    signedTransaction,
    proposedAssetChanges,
    confirmedAssetChanges,
    signingPayloads,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
