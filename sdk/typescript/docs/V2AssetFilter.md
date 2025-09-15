# V2AssetFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**blockchain** | [**V2IntFilter**](V2IntFilter.md) |  | [optional] [default to undefined]
**enabled** | [**V2BoolFilter**](V2BoolFilter.md) |  | [optional] [default to undefined]
**isVetted** | [**V2BoolFilter**](V2BoolFilter.md) |  | [optional] [default to undefined]
**standard** | [**V2IntFilter**](V2IntFilter.md) |  | [optional] [default to undefined]
**organizationId** | [**V2StringFilter**](V2StringFilter.md) |  | [optional] [default to undefined]
**symbol** | [**V2StringFilter**](V2StringFilter.md) |  | [optional] [default to undefined]
**name** | [**V2StringFilter**](V2StringFilter.md) |  | [optional] [default to undefined]
**contractAddress** | [**V2StringFilter**](V2StringFilter.md) |  | [optional] [default to undefined]
**source** | [**V2StringFilter**](V2StringFilter.md) |  | [optional] [default to undefined]
**lastSyncedAt** | [**V2TimestampFilter**](V2TimestampFilter.md) |  | [optional] [default to undefined]
**hasChecksum** | [**V2BoolFilter**](V2BoolFilter.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V2AssetFilter } from '@palisade-inc/typescript-sdk';

const instance: V2AssetFilter = {
    blockchain,
    enabled,
    isVetted,
    standard,
    organizationId,
    symbol,
    name,
    contractAddress,
    source,
    lastSyncedAt,
    hasChecksum,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
