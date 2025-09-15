# V2S3Config


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bucket** | **string** | S3 bucket name | [optional] [default to undefined]
**region** | **string** | S3 region | [optional] [default to undefined]
**assumeRoleArn** | **string** | ARN of the role to assume for S3 access | [optional] [default to undefined]

## Example

```typescript
import { V2S3Config } from '@palisade-inc/typescript-sdk';

const instance: V2S3Config = {
    bucket,
    region,
    assumeRoleArn,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
