# Accountv2Organization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The organization ID | [default to undefined]
**name** | **string** | The organization name | [default to undefined]
**createdBy** | **string** | The ID of the user who created this organization | [default to undefined]
**createdAt** | **string** | The date and time the organization was created | [default to undefined]
**updatedBy** | **string** | The ID of the user who updated this organization | [default to undefined]
**updatedAt** | **string** | The date and time the organization was updated | [default to undefined]
**settings** | [**V2OrganizationSettings**](V2OrganizationSettings.md) |  | [default to undefined]
**address** | [**Commonv2Address**](Commonv2Address.md) |  | [default to undefined]

## Example

```typescript
import { Accountv2Organization } from '@palisade-inc/typescript-sdk';

const instance: Accountv2Organization = {
    id,
    name,
    createdBy,
    createdAt,
    updatedBy,
    updatedAt,
    settings,
    address,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
