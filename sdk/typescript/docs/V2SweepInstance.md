# V2SweepInstance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The sweep instance ID | [default to undefined]
**sweepConfigurationId** | **string** | The sweep configuration ID | [default to undefined]
**startedAt** | **string** | The date and time the sweep instance was started | [default to undefined]
**completedAt** | **string** | The date and time the sweep instance was completed | [optional] [default to undefined]
**totalWalletsSwept** | **string** | The total number of wallets swept in the sweep instance | [default to undefined]
**totalSuccessfulWallets** | **string** | The number of wallets successfully swept in the sweep instance | [default to undefined]
**totalFailedWallets** | **string** | The number of wallets that failed to sweep in the sweep instance | [default to undefined]
**totalAmountSwept** | **{ [key: string]: string; }** | A map of blockchain asset to total amount swept in the sweep instance | [default to undefined]
**incomingFee** | **string** | the incoming estimated fee from the funder wallets | [default to undefined]
**status** | [**V2SweepingInstanceStatus**](V2SweepingInstanceStatus.md) |  | [default to undefined]
**errorMessage** | **string** | Error message in case the sweep failed | [optional] [default to undefined]
**outgoingFee** | **string** | The actual outgoing fee for the sweep instance | [optional] [default to undefined]

## Example

```typescript
import { V2SweepInstance } from '@palisade-inc/typescript-sdk';

const instance: V2SweepInstance = {
    id,
    sweepConfigurationId,
    startedAt,
    completedAt,
    totalWalletsSwept,
    totalSuccessfulWallets,
    totalFailedWallets,
    totalAmountSwept,
    incomingFee,
    status,
    errorMessage,
    outgoingFee,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
