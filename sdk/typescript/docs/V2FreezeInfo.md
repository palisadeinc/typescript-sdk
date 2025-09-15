# V2FreezeInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**isFrozen** | **boolean** | Whether the transaction is currently frozen | [optional] [default to undefined]
**history** | [**Array&lt;V2FreezeHistoryEntry&gt;**](V2FreezeHistoryEntry.md) | History of all freeze/unfreeze actions. Latest entry contains current state details when frozen. | [optional] [default to undefined]

## Example

```typescript
import { V2FreezeInfo } from '@palisade-inc/typescript-sdk';

const instance: V2FreezeInfo = {
    isFrozen,
    history,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
