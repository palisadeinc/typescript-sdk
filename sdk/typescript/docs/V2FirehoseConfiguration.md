# V2FirehoseConfiguration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**streamName** | **string** | Firehose stream name | [default to undefined]
**region** | **string** | Firehose region | [default to undefined]
**assumeRoleArn** | **string** | ARN of the role for the Palisade auditor to assume for Firehose access. Must have &#x60;firehose:PutRecordBatch&#x60; permissions on the stream. | [default to undefined]
**status** | [**V2FirehoseConfigurationStatus**](V2FirehoseConfigurationStatus.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2FirehoseConfiguration } from '@palisade-inc/typescript-sdk';

const instance: V2FirehoseConfiguration = {
    streamName,
    region,
    assumeRoleArn,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
