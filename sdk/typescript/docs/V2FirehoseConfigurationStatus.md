# V2FirehoseConfigurationStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**state** | [**V2FirehoseConfigurationState**](V2FirehoseConfigurationState.md) |  | [default to undefined]
**lastError** | **string** | Last error message if any | [optional] [default to undefined]
**lastErrorAt** | **string** | Timestamp of the last error | [optional] [default to undefined]
**consecutiveFailures** | **number** | Number of consecutive failures | [default to undefined]
**successfulUploads** | **number** | Total number of successful uploads | [default to undefined]
**failedUploads** | **number** | Total number of failed uploads | [default to undefined]

## Example

```typescript
import { V2FirehoseConfigurationStatus } from '@palisade-inc/typescript-sdk';

const instance: V2FirehoseConfigurationStatus = {
    state,
    lastError,
    lastErrorAt,
    consecutiveFailures,
    successfulUploads,
    failedUploads,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
