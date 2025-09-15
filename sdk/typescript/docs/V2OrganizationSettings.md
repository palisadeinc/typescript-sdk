# V2OrganizationSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organizationType** | [**V2OrganizationType**](V2OrganizationType.md) |  | [default to undefined]
**enabledComplianceIntegrations** | [**Array&lt;V2ComplianceIntegration&gt;**](V2ComplianceIntegration.md) |  | [default to undefined]
**enabledKeystores** | [**Array&lt;V2Keystore&gt;**](V2Keystore.md) |  | [default to undefined]
**region** | **string** | The region in which the organization data is stored | [default to undefined]
**enabled** | **boolean** | Whether the organization is enabled | [default to undefined]
**logo** | **string** |  | [optional] [default to undefined]
**legalName** | **string** | The full legal name of the organization | [default to undefined]
**vaspName** | **string** | The Virtual Asset Service Provider | [default to undefined]
**vaspDid** | **string** | The Virtual Asset Service Providers\&#39; Decentralized Identifier | [default to undefined]

## Example

```typescript
import { V2OrganizationSettings } from '@palisade-inc/typescript-sdk';

const instance: V2OrganizationSettings = {
    organizationType,
    enabledComplianceIntegrations,
    enabledKeystores,
    region,
    enabled,
    logo,
    legalName,
    vaspName,
    vaspDid,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
