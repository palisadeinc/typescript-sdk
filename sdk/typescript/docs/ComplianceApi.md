# ComplianceApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**complianceServiceGetNotabeneCustomerToken**](#complianceservicegetnotabenecustomertoken) | **GET** /v2/notabene/token | Create customer tokens|
|[**complianceServiceGetNotabeneVASPSearch**](#complianceservicegetnotabenevaspsearch) | **GET** /v2/notabene/search | Search for VASPs|

# **complianceServiceGetNotabeneCustomerToken**
> V2GetNotabeneCustomerTokenResponse complianceServiceGetNotabeneCustomerToken()

Create a new notabene customer token

### Example

```typescript
import {
    ComplianceApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ComplianceApi(configuration);

const { status, data } = await apiInstance.complianceServiceGetNotabeneCustomerToken();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2GetNotabeneCustomerTokenResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **complianceServiceGetNotabeneVASPSearch**
> V2GetNotabeneVASPSearchResponse complianceServiceGetNotabeneVASPSearch()

Search for VASPs using the notabene search endpoint

### Example

```typescript
import {
    ComplianceApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new ComplianceApi(configuration);

let q: string; //string to query (optional) (default to undefined)
let emailDomain: string; //filter on email domain (optional) (default to undefined)
let chainalysisName: string; //filter on chainalysis name (optional) (default to undefined)
let hasAdmin: boolean; //filter on hasAdmin (true or false) (optional) (default to undefined)
let badge: string; //filter by badge (optional) (default to undefined)
let jurisdictions: string; //filter by jurisdictions (multiple jurisdictions can be provided as a comma-separated list) (optional) (default to undefined)
let fields: string; //csv of fields to return (optional) (default to undefined)
let page: number; //page number (optional) (default to undefined)
let perPage: number; //records per page (optional) (default to undefined)
let order: string; //field to order by (optional) (default to undefined)
let all: boolean; //return all records (optional) (default to undefined)
let listingType: string; //Choose how gateway VASPs and non-gateway VASPs are returned. By default, exclude_subsidiaries. (optional) (default to undefined)
let includeUncheckedVasps: boolean; //Defaults to false Include VASPs that have not been internally checked (optional) (default to undefined)
let includeActiveSendersOnly: boolean; //Defaults to false Include only VASPs that are actively sending transactions (optional) (default to undefined)
let includeActiveReceiversOnly: boolean; //Defaults to false Include only VASPs that are actively receiving transactions (optional) (default to undefined)
let regulatoryStatus: string; //Include only VASPs matching the specified regulatory status (optional) (default to undefined)
let networkStatus: string; //Include only VASPs matching the specified network status (optional) (default to undefined)
let asset: string; //Asset symbol, provide when filtering by wallet (optional) (default to undefined)
let reviewedByVaspDid: string; //Include reviewed VASPs for the specified DID (optional) (default to undefined)
let showJurisdictionStatus: boolean; //Include jurisdiction status information (optional) (default to undefined)
let reviewValue: string; //Include reviewed VASPs containing the specified value (optional) (default to undefined)
let reviewIncludeInWidget: Array<string>; //Include VASPs based on review \"included in widget\" status (optional) (default to undefined)
let filterByJurisdictionStatus: string; //Filter by specified jurisdiction status (optional) (default to undefined)

const { status, data } = await apiInstance.complianceServiceGetNotabeneVASPSearch(
    q,
    emailDomain,
    chainalysisName,
    hasAdmin,
    badge,
    jurisdictions,
    fields,
    page,
    perPage,
    order,
    all,
    listingType,
    includeUncheckedVasps,
    includeActiveSendersOnly,
    includeActiveReceiversOnly,
    regulatoryStatus,
    networkStatus,
    asset,
    reviewedByVaspDid,
    showJurisdictionStatus,
    reviewValue,
    reviewIncludeInWidget,
    filterByJurisdictionStatus
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **q** | [**string**] | string to query | (optional) defaults to undefined|
| **emailDomain** | [**string**] | filter on email domain | (optional) defaults to undefined|
| **chainalysisName** | [**string**] | filter on chainalysis name | (optional) defaults to undefined|
| **hasAdmin** | [**boolean**] | filter on hasAdmin (true or false) | (optional) defaults to undefined|
| **badge** | [**string**] | filter by badge | (optional) defaults to undefined|
| **jurisdictions** | [**string**] | filter by jurisdictions (multiple jurisdictions can be provided as a comma-separated list) | (optional) defaults to undefined|
| **fields** | [**string**] | csv of fields to return | (optional) defaults to undefined|
| **page** | [**number**] | page number | (optional) defaults to undefined|
| **perPage** | [**number**] | records per page | (optional) defaults to undefined|
| **order** | [**string**] | field to order by | (optional) defaults to undefined|
| **all** | [**boolean**] | return all records | (optional) defaults to undefined|
| **listingType** | [**string**] | Choose how gateway VASPs and non-gateway VASPs are returned. By default, exclude_subsidiaries. | (optional) defaults to undefined|
| **includeUncheckedVasps** | [**boolean**] | Defaults to false Include VASPs that have not been internally checked | (optional) defaults to undefined|
| **includeActiveSendersOnly** | [**boolean**] | Defaults to false Include only VASPs that are actively sending transactions | (optional) defaults to undefined|
| **includeActiveReceiversOnly** | [**boolean**] | Defaults to false Include only VASPs that are actively receiving transactions | (optional) defaults to undefined|
| **regulatoryStatus** | [**string**] | Include only VASPs matching the specified regulatory status | (optional) defaults to undefined|
| **networkStatus** | [**string**] | Include only VASPs matching the specified network status | (optional) defaults to undefined|
| **asset** | [**string**] | Asset symbol, provide when filtering by wallet | (optional) defaults to undefined|
| **reviewedByVaspDid** | [**string**] | Include reviewed VASPs for the specified DID | (optional) defaults to undefined|
| **showJurisdictionStatus** | [**boolean**] | Include jurisdiction status information | (optional) defaults to undefined|
| **reviewValue** | [**string**] | Include reviewed VASPs containing the specified value | (optional) defaults to undefined|
| **reviewIncludeInWidget** | **Array&lt;string&gt;** | Include VASPs based on review \&quot;included in widget\&quot; status | (optional) defaults to undefined|
| **filterByJurisdictionStatus** | [**string**] | Filter by specified jurisdiction status | (optional) defaults to undefined|


### Return type

**V2GetNotabeneVASPSearchResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

