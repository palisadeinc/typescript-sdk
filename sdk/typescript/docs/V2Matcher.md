# V2Matcher

Policies are matched in the following override order: 1. Caller (User / API Credential) 2. Counterparty Address 3. Transaction Type 4. Sign For 5. Counterparty ID 6. Address ID 7. Wallet ID

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**V2MatcherType**](V2MatcherType.md) |  | [default to undefined]
**value** | **string** | Comma seperated list of matcher values. | [optional] [default to undefined]
**values** | **Array&lt;string&gt;** | Matcher values. | [optional] [default to undefined]

## Example

```typescript
import { V2Matcher } from '@palisade-inc/typescript-sdk';

const instance: V2Matcher = {
    type,
    value,
    values,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
