# RegistryApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**registryManagementServiceManagementCreateBlockchain**](#registrymanagementservicemanagementcreateblockchain) | **POST** /v2/blockchains | Create a new blockchain|
|[**registryManagementServiceManagementCreateCurrency**](#registrymanagementservicemanagementcreatecurrency) | **POST** /v2/currencies | Create a new currency|
|[**registryManagementServiceManagementDeleteAsset**](#registrymanagementservicemanagementdeleteasset) | **DELETE** /v2/assets/{id} | Delete an asset|
|[**registryManagementServiceManagementDeleteBlockchain**](#registrymanagementservicemanagementdeleteblockchain) | **DELETE** /v2/blockchains/{id} | Delete a blockchain|
|[**registryManagementServiceManagementDeleteCurrency**](#registrymanagementservicemanagementdeletecurrency) | **DELETE** /v2/currencies/{code} | Delete a currency|
|[**registryManagementServiceManagementGetImport**](#registrymanagementservicemanagementgetimport) | **GET** /v2/sync/imports/{importId} | Get import details|
|[**registryManagementServiceManagementGetImportHistory**](#registrymanagementservicemanagementgetimporthistory) | **GET** /v2/sync/imports | Get import history|
|[**registryManagementServiceManagementGetSyncStatus**](#registrymanagementservicemanagementgetsyncstatus) | **GET** /v2/sync/status | Get sync status|
|[**registryManagementServiceManagementTriggerSync**](#registrymanagementservicemanagementtriggersync) | **POST** /v2/sync:trigger | Trigger asset sync|
|[**registryManagementServiceManagementUpdateAsset**](#registrymanagementservicemanagementupdateasset) | **PATCH** /v2/assets/{id} | Update an asset|
|[**registryManagementServiceManagementUpdateBlockchain**](#registrymanagementservicemanagementupdateblockchain) | **PATCH** /v2/blockchains/{id} | Update a blockchain|
|[**registryManagementServiceManagementUpdateCurrency**](#registrymanagementservicemanagementupdatecurrency) | **PATCH** /v2/currencies/{code} | Update a currency|
|[**registryServiceCreateAsset**](#registryservicecreateasset) | **POST** /v2/assets | Create a new asset|
|[**registryServiceGetAsset**](#registryservicegetasset) | **GET** /v2/assets/{id} | Get an asset|
|[**registryServiceGetBlockchain**](#registryservicegetblockchain) | **GET** /v2/blockchains/{id} | Get a blockchain|
|[**registryServiceGetCurrency**](#registryservicegetcurrency) | **GET** /v2/currencies/{code} | Get a currency|
|[**registryServiceListAssets**](#registryservicelistassets) | **POST** /v2/assets:list | List assets|
|[**registryServiceListAssets2**](#registryservicelistassets2) | **GET** /v2/assets | List assets|
|[**registryServiceListBlockchains**](#registryservicelistblockchains) | **POST** /v2/blockchains:list | List blockchains|
|[**registryServiceListBlockchains2**](#registryservicelistblockchains2) | **GET** /v2/blockchains | List blockchains|
|[**registryServiceListCurrencies**](#registryservicelistcurrencies) | **POST** /v2/currencies:list | List currencies|
|[**registryServiceListCurrencies2**](#registryservicelistcurrencies2) | **GET** /v2/currencies | List currencies|

# **registryManagementServiceManagementCreateBlockchain**
> V2BlockchainInfo registryManagementServiceManagementCreateBlockchain(v2ManagementCreateBlockchainRequest)

Create a new blockchain configuration in the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ManagementCreateBlockchainRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ManagementCreateBlockchainRequest: V2ManagementCreateBlockchainRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementCreateBlockchain(
    v2ManagementCreateBlockchainRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ManagementCreateBlockchainRequest** | **V2ManagementCreateBlockchainRequest**|  | |


### Return type

**V2BlockchainInfo**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryManagementServiceManagementCreateCurrency**
> V2Currency registryManagementServiceManagementCreateCurrency(v2ManagementCreateCurrencyRequest)

Create a new currency in the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ManagementCreateCurrencyRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ManagementCreateCurrencyRequest: V2ManagementCreateCurrencyRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementCreateCurrency(
    v2ManagementCreateCurrencyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ManagementCreateCurrencyRequest** | **V2ManagementCreateCurrencyRequest**|  | |


### Return type

**V2Currency**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryManagementServiceManagementDeleteAsset**
> object registryManagementServiceManagementDeleteAsset()

Soft delete an asset from the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: string; //Asset ID to delete (default to undefined)

const { status, data } = await apiInstance.registryManagementServiceManagementDeleteAsset(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Asset ID to delete | defaults to undefined|


### Return type

**object**

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

# **registryManagementServiceManagementDeleteBlockchain**
> object registryManagementServiceManagementDeleteBlockchain()

Soft delete a blockchain from the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; //The blockchain ID to delete (default to undefined)

const { status, data } = await apiInstance.registryManagementServiceManagementDeleteBlockchain(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** | The blockchain ID to delete | defaults to undefined|


### Return type

**object**

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

# **registryManagementServiceManagementDeleteCurrency**
> object registryManagementServiceManagementDeleteCurrency()

Soft delete a currency from the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let code: string; //Currency code to delete (default to undefined)

const { status, data } = await apiInstance.registryManagementServiceManagementDeleteCurrency(
    code
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **code** | [**string**] | Currency code to delete | defaults to undefined|


### Return type

**object**

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

# **registryManagementServiceManagementGetImport**
> V2Import registryManagementServiceManagementGetImport()

Get details of a specific import operation

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let importId: string; //Import ID to retrieve (default to undefined)

const { status, data } = await apiInstance.registryManagementServiceManagementGetImport(
    importId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **importId** | [**string**] | Import ID to retrieve | defaults to undefined|


### Return type

**V2Import**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryManagementServiceManagementGetImportHistory**
> V2ManagementGetImportHistoryResponse registryManagementServiceManagementGetImportHistory()

Get the history of sync import operations

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let paginationPageSize: number; //Number of results per page (default 50, max 1000) (optional) (default to undefined)
let paginationPageToken: string; //Token for pagination from previous response (optional) (default to undefined)
let paginationOrderBy: string; //Field to order results by (optional) (default to undefined)
let paginationOrder: 'SORT_ORDER_ASC' | 'SORT_ORDER_DESC'; //Sort order (ASC or DESC) (optional) (default to undefined)
let source: string; //Filter by import source (optional) (default to undefined)
let status: string; //Filter by import status (optional) (default to undefined)
let startedAtEq: string; //Exact timestamp match (optional) (default to undefined)
let startedAtNotEq: string; //Not equal to timestamp (optional) (default to undefined)
let startedAtBefore: string; //Before this timestamp (optional) (default to undefined)
let startedAtAfter: string; //After this timestamp (optional) (default to undefined)
let startedAtGte: string; //Greater than or equal to timestamp (optional) (default to undefined)
let startedAtLte: string; //Less than or equal to timestamp (optional) (default to undefined)
let startedAtBetweenStart: string; //Start of time range (inclusive) (optional) (default to undefined)
let startedAtBetweenEnd: string; //End of time range (inclusive) (optional) (default to undefined)
let startedAtIsNull: boolean; //Check if field is null (optional) (default to undefined)
let startedAtRelativeDays: number; //Relative days from now (negative for past, positive for future) (optional) (default to undefined)
let completedAtEq: string; //Exact timestamp match (optional) (default to undefined)
let completedAtNotEq: string; //Not equal to timestamp (optional) (default to undefined)
let completedAtBefore: string; //Before this timestamp (optional) (default to undefined)
let completedAtAfter: string; //After this timestamp (optional) (default to undefined)
let completedAtGte: string; //Greater than or equal to timestamp (optional) (default to undefined)
let completedAtLte: string; //Less than or equal to timestamp (optional) (default to undefined)
let completedAtBetweenStart: string; //Start of time range (inclusive) (optional) (default to undefined)
let completedAtBetweenEnd: string; //End of time range (inclusive) (optional) (default to undefined)
let completedAtIsNull: boolean; //Check if field is null (optional) (default to undefined)
let completedAtRelativeDays: number; //Relative days from now (negative for past, positive for future) (optional) (default to undefined)

const { status, data } = await apiInstance.registryManagementServiceManagementGetImportHistory(
    paginationPageSize,
    paginationPageToken,
    paginationOrderBy,
    paginationOrder,
    source,
    status,
    startedAtEq,
    startedAtNotEq,
    startedAtBefore,
    startedAtAfter,
    startedAtGte,
    startedAtLte,
    startedAtBetweenStart,
    startedAtBetweenEnd,
    startedAtIsNull,
    startedAtRelativeDays,
    completedAtEq,
    completedAtNotEq,
    completedAtBefore,
    completedAtAfter,
    completedAtGte,
    completedAtLte,
    completedAtBetweenStart,
    completedAtBetweenEnd,
    completedAtIsNull,
    completedAtRelativeDays
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paginationPageSize** | [**number**] | Number of results per page (default 50, max 1000) | (optional) defaults to undefined|
| **paginationPageToken** | [**string**] | Token for pagination from previous response | (optional) defaults to undefined|
| **paginationOrderBy** | [**string**] | Field to order results by | (optional) defaults to undefined|
| **paginationOrder** | [**&#39;SORT_ORDER_ASC&#39; | &#39;SORT_ORDER_DESC&#39;**]**Array<&#39;SORT_ORDER_ASC&#39; &#124; &#39;SORT_ORDER_DESC&#39;>** | Sort order (ASC or DESC) | (optional) defaults to undefined|
| **source** | [**string**] | Filter by import source | (optional) defaults to undefined|
| **status** | [**string**] | Filter by import status | (optional) defaults to undefined|
| **startedAtEq** | [**string**] | Exact timestamp match | (optional) defaults to undefined|
| **startedAtNotEq** | [**string**] | Not equal to timestamp | (optional) defaults to undefined|
| **startedAtBefore** | [**string**] | Before this timestamp | (optional) defaults to undefined|
| **startedAtAfter** | [**string**] | After this timestamp | (optional) defaults to undefined|
| **startedAtGte** | [**string**] | Greater than or equal to timestamp | (optional) defaults to undefined|
| **startedAtLte** | [**string**] | Less than or equal to timestamp | (optional) defaults to undefined|
| **startedAtBetweenStart** | [**string**] | Start of time range (inclusive) | (optional) defaults to undefined|
| **startedAtBetweenEnd** | [**string**] | End of time range (inclusive) | (optional) defaults to undefined|
| **startedAtIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **startedAtRelativeDays** | [**number**] | Relative days from now (negative for past, positive for future) | (optional) defaults to undefined|
| **completedAtEq** | [**string**] | Exact timestamp match | (optional) defaults to undefined|
| **completedAtNotEq** | [**string**] | Not equal to timestamp | (optional) defaults to undefined|
| **completedAtBefore** | [**string**] | Before this timestamp | (optional) defaults to undefined|
| **completedAtAfter** | [**string**] | After this timestamp | (optional) defaults to undefined|
| **completedAtGte** | [**string**] | Greater than or equal to timestamp | (optional) defaults to undefined|
| **completedAtLte** | [**string**] | Less than or equal to timestamp | (optional) defaults to undefined|
| **completedAtBetweenStart** | [**string**] | Start of time range (inclusive) | (optional) defaults to undefined|
| **completedAtBetweenEnd** | [**string**] | End of time range (inclusive) | (optional) defaults to undefined|
| **completedAtIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **completedAtRelativeDays** | [**number**] | Relative days from now (negative for past, positive for future) | (optional) defaults to undefined|


### Return type

**V2ManagementGetImportHistoryResponse**

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

# **registryManagementServiceManagementGetSyncStatus**
> V2ManagementGetSyncStatusResponse registryManagementServiceManagementGetSyncStatus()

Get the current status of the sync scheduler

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

const { status, data } = await apiInstance.registryManagementServiceManagementGetSyncStatus();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2ManagementGetSyncStatusResponse**

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

# **registryManagementServiceManagementTriggerSync**
> V2ManagementTriggerSyncResponse registryManagementServiceManagementTriggerSync(v2ManagementTriggerSyncRequest)

Manually trigger a synchronization of assets from CoinGecko

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ManagementTriggerSyncRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ManagementTriggerSyncRequest: V2ManagementTriggerSyncRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementTriggerSync(
    v2ManagementTriggerSyncRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ManagementTriggerSyncRequest** | **V2ManagementTriggerSyncRequest**|  | |


### Return type

**V2ManagementTriggerSyncResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **registryManagementServiceManagementUpdateAsset**
> Commonv2Asset registryManagementServiceManagementUpdateAsset(registryManagementServiceManagementUpdateAssetRequest)

Update an existing asset in the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    RegistryManagementServiceManagementUpdateAssetRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: string; //Asset ID to update (default to undefined)
let registryManagementServiceManagementUpdateAssetRequest: RegistryManagementServiceManagementUpdateAssetRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementUpdateAsset(
    id,
    registryManagementServiceManagementUpdateAssetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryManagementServiceManagementUpdateAssetRequest** | **RegistryManagementServiceManagementUpdateAssetRequest**|  | |
| **id** | [**string**] | Asset ID to update | defaults to undefined|


### Return type

**Commonv2Asset**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryManagementServiceManagementUpdateBlockchain**
> V2BlockchainInfo registryManagementServiceManagementUpdateBlockchain(registryManagementServiceManagementUpdateBlockchainRequest)

Update an existing blockchain configuration

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    RegistryManagementServiceManagementUpdateBlockchainRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; //The blockchain ID to update (default to undefined)
let registryManagementServiceManagementUpdateBlockchainRequest: RegistryManagementServiceManagementUpdateBlockchainRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementUpdateBlockchain(
    id,
    registryManagementServiceManagementUpdateBlockchainRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryManagementServiceManagementUpdateBlockchainRequest** | **RegistryManagementServiceManagementUpdateBlockchainRequest**|  | |
| **id** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** | The blockchain ID to update | defaults to undefined|


### Return type

**V2BlockchainInfo**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryManagementServiceManagementUpdateCurrency**
> V2Currency registryManagementServiceManagementUpdateCurrency(registryManagementServiceManagementUpdateCurrencyRequest)

Update an existing currency in the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    RegistryManagementServiceManagementUpdateCurrencyRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let code: string; //Currency code to update (default to undefined)
let registryManagementServiceManagementUpdateCurrencyRequest: RegistryManagementServiceManagementUpdateCurrencyRequest; //

const { status, data } = await apiInstance.registryManagementServiceManagementUpdateCurrency(
    code,
    registryManagementServiceManagementUpdateCurrencyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryManagementServiceManagementUpdateCurrencyRequest** | **RegistryManagementServiceManagementUpdateCurrencyRequest**|  | |
| **code** | [**string**] | Currency code to update | defaults to undefined|


### Return type

**V2Currency**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryServiceCreateAsset**
> Commonv2Asset registryServiceCreateAsset(v2CreateAssetRequest)

Create a new asset in the registry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2CreateAssetRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2CreateAssetRequest: V2CreateAssetRequest; //

const { status, data } = await apiInstance.registryServiceCreateAsset(
    v2CreateAssetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateAssetRequest** | **V2CreateAssetRequest**|  | |


### Return type

**Commonv2Asset**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryServiceGetAsset**
> Commonv2Asset registryServiceGetAsset()

Get asset configuration by ID

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: string; //Asset ID in format blockchain:contract:symbol (default to undefined)

const { status, data } = await apiInstance.registryServiceGetAsset(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Asset ID in format blockchain:contract:symbol | defaults to undefined|


### Return type

**Commonv2Asset**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryServiceGetBlockchain**
> V2BlockchainInfo registryServiceGetBlockchain()

Get blockchain configuration by ID

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; //The blockchain ID to retrieve (default to undefined)

const { status, data } = await apiInstance.registryServiceGetBlockchain(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** | The blockchain ID to retrieve | defaults to undefined|


### Return type

**V2BlockchainInfo**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryServiceGetCurrency**
> V2Currency registryServiceGetCurrency()

Get currency configuration by code

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let code: string; //ISO 4217 currency code (default to undefined)

const { status, data } = await apiInstance.registryServiceGetCurrency(
    code
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **code** | [**string**] | ISO 4217 currency code | defaults to undefined|


### Return type

**V2Currency**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** | Returned when the request is malformed or invalid. |  -  |
|**401** | Returned when the request was unauthorized. |  -  |
|**403** | Returned when the request was forbidden. |  -  |
|**404** | Returned when the resource does not exist. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryServiceListAssets**
> V2ListAssetsResponse registryServiceListAssets(v2ListAssetsRequest)

List assets with advanced filtering and search. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ListAssetsRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ListAssetsRequest: V2ListAssetsRequest; //

const { status, data } = await apiInstance.registryServiceListAssets(
    v2ListAssetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ListAssetsRequest** | **V2ListAssetsRequest**|  | |


### Return type

**V2ListAssetsResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **registryServiceListAssets2**
> V2ListAssetsResponse registryServiceListAssets2()

List assets with advanced filtering and search. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let filterBlockchainEq: number; //Equals (optional) (default to undefined)
let filterBlockchainNotEq: number; //Not equal to (optional) (default to undefined)
let filterBlockchainIn: Array<number>; //Value is in the list (optional) (default to undefined)
let filterBlockchainNotIn: Array<number>; //Value is not in the list (optional) (default to undefined)
let filterBlockchainIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterBlockchainGt: number; //Greater than (optional) (default to undefined)
let filterBlockchainGte: number; //Greater than or equal to (optional) (default to undefined)
let filterBlockchainLt: number; //Less than (optional) (default to undefined)
let filterBlockchainLte: number; //Less than or equal to (optional) (default to undefined)
let filterEnabledEq: boolean; //Equals (optional) (default to undefined)
let filterEnabledIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterIsVettedEq: boolean; //Equals (optional) (default to undefined)
let filterIsVettedIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterStandardEq: number; //Equals (optional) (default to undefined)
let filterStandardNotEq: number; //Not equal to (optional) (default to undefined)
let filterStandardIn: Array<number>; //Value is in the list (optional) (default to undefined)
let filterStandardNotIn: Array<number>; //Value is not in the list (optional) (default to undefined)
let filterStandardIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterStandardGt: number; //Greater than (optional) (default to undefined)
let filterStandardGte: number; //Greater than or equal to (optional) (default to undefined)
let filterStandardLt: number; //Less than (optional) (default to undefined)
let filterStandardLte: number; //Less than or equal to (optional) (default to undefined)
let filterOrganizationIdEq: string; //Exact match (optional) (default to undefined)
let filterOrganizationIdNotEq: string; //Not equal to (optional) (default to undefined)
let filterOrganizationIdContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterOrganizationIdStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterOrganizationIdEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterOrganizationIdIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterOrganizationIdNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterOrganizationIdRegex: string; //Regular expression match (optional) (default to undefined)
let filterOrganizationIdIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterOrganizationIdFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterOrganizationIdFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterSymbolEq: string; //Exact match (optional) (default to undefined)
let filterSymbolNotEq: string; //Not equal to (optional) (default to undefined)
let filterSymbolContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterSymbolStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterSymbolEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterSymbolIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterSymbolNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterSymbolRegex: string; //Regular expression match (optional) (default to undefined)
let filterSymbolIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterSymbolFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterSymbolFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterNameEq: string; //Exact match (optional) (default to undefined)
let filterNameNotEq: string; //Not equal to (optional) (default to undefined)
let filterNameContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterNameStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterNameEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterNameIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterNameNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterNameRegex: string; //Regular expression match (optional) (default to undefined)
let filterNameIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterNameFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterNameFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterContractAddressEq: string; //Exact match (optional) (default to undefined)
let filterContractAddressNotEq: string; //Not equal to (optional) (default to undefined)
let filterContractAddressContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterContractAddressStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterContractAddressEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterContractAddressIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterContractAddressNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterContractAddressRegex: string; //Regular expression match (optional) (default to undefined)
let filterContractAddressIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterContractAddressFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterContractAddressFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterSourceEq: string; //Exact match (optional) (default to undefined)
let filterSourceNotEq: string; //Not equal to (optional) (default to undefined)
let filterSourceContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterSourceStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterSourceEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterSourceIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterSourceNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterSourceRegex: string; //Regular expression match (optional) (default to undefined)
let filterSourceIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterSourceFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterSourceFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterLastSyncedAtEq: string; //Exact timestamp match (optional) (default to undefined)
let filterLastSyncedAtNotEq: string; //Not equal to timestamp (optional) (default to undefined)
let filterLastSyncedAtBefore: string; //Before this timestamp (optional) (default to undefined)
let filterLastSyncedAtAfter: string; //After this timestamp (optional) (default to undefined)
let filterLastSyncedAtGte: string; //Greater than or equal to timestamp (optional) (default to undefined)
let filterLastSyncedAtLte: string; //Less than or equal to timestamp (optional) (default to undefined)
let filterLastSyncedAtBetweenStart: string; //Start of time range (inclusive) (optional) (default to undefined)
let filterLastSyncedAtBetweenEnd: string; //End of time range (inclusive) (optional) (default to undefined)
let filterLastSyncedAtIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterLastSyncedAtRelativeDays: number; //Relative days from now (negative for past, positive for future) (optional) (default to undefined)
let filterHasChecksumEq: boolean; //Equals (optional) (default to undefined)
let filterHasChecksumIsNull: boolean; //Check if field is null (optional) (default to undefined)
let searchTerm: string; //Search term (optional) (default to undefined)
let searchFields: Array<string>; //Fields to search in (optional) (default to undefined)
let searchType: 'SEARCH_TYPE_CONTAINS' | 'SEARCH_TYPE_STARTS_WITH' | 'SEARCH_TYPE_EXACT' | 'SEARCH_TYPE_FUZZY' | 'SEARCH_TYPE_FULLTEXT'; //Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) (optional) (default to undefined)
let searchMinScore: number; //Minimum relevance score for fuzzy/fulltext search (optional) (default to undefined)
let searchOptionsCaseSensitive: boolean; //Enable case-sensitive search (default: false) (optional) (default to undefined)
let searchOptionsMinTermLength: number; //Minimum search term length (optional) (default to undefined)
let searchOptionsMaxResults: number; //Maximum number of results to return (optional) (default to undefined)
let searchOptionsMultiTermAnd: boolean; //Use AND logic for multiple terms (default: false for OR) (optional) (default to undefined)
let paginationPageSize: number; //Number of results per page (default 50, max 1000) (optional) (default to undefined)
let paginationPageToken: string; //Token for pagination from previous response (optional) (default to undefined)
let paginationOrderBy: string; //Field to order results by (optional) (default to undefined)
let paginationOrder: 'SORT_ORDER_ASC' | 'SORT_ORDER_DESC'; //Sort order (ASC or DESC) (optional) (default to undefined)

const { status, data } = await apiInstance.registryServiceListAssets2(
    filterBlockchainEq,
    filterBlockchainNotEq,
    filterBlockchainIn,
    filterBlockchainNotIn,
    filterBlockchainIsNull,
    filterBlockchainGt,
    filterBlockchainGte,
    filterBlockchainLt,
    filterBlockchainLte,
    filterEnabledEq,
    filterEnabledIsNull,
    filterIsVettedEq,
    filterIsVettedIsNull,
    filterStandardEq,
    filterStandardNotEq,
    filterStandardIn,
    filterStandardNotIn,
    filterStandardIsNull,
    filterStandardGt,
    filterStandardGte,
    filterStandardLt,
    filterStandardLte,
    filterOrganizationIdEq,
    filterOrganizationIdNotEq,
    filterOrganizationIdContains,
    filterOrganizationIdStartsWith,
    filterOrganizationIdEndsWith,
    filterOrganizationIdIn,
    filterOrganizationIdNotIn,
    filterOrganizationIdRegex,
    filterOrganizationIdIsNull,
    filterOrganizationIdFuzzyValue,
    filterOrganizationIdFuzzyMinSimilarity,
    filterSymbolEq,
    filterSymbolNotEq,
    filterSymbolContains,
    filterSymbolStartsWith,
    filterSymbolEndsWith,
    filterSymbolIn,
    filterSymbolNotIn,
    filterSymbolRegex,
    filterSymbolIsNull,
    filterSymbolFuzzyValue,
    filterSymbolFuzzyMinSimilarity,
    filterNameEq,
    filterNameNotEq,
    filterNameContains,
    filterNameStartsWith,
    filterNameEndsWith,
    filterNameIn,
    filterNameNotIn,
    filterNameRegex,
    filterNameIsNull,
    filterNameFuzzyValue,
    filterNameFuzzyMinSimilarity,
    filterContractAddressEq,
    filterContractAddressNotEq,
    filterContractAddressContains,
    filterContractAddressStartsWith,
    filterContractAddressEndsWith,
    filterContractAddressIn,
    filterContractAddressNotIn,
    filterContractAddressRegex,
    filterContractAddressIsNull,
    filterContractAddressFuzzyValue,
    filterContractAddressFuzzyMinSimilarity,
    filterSourceEq,
    filterSourceNotEq,
    filterSourceContains,
    filterSourceStartsWith,
    filterSourceEndsWith,
    filterSourceIn,
    filterSourceNotIn,
    filterSourceRegex,
    filterSourceIsNull,
    filterSourceFuzzyValue,
    filterSourceFuzzyMinSimilarity,
    filterLastSyncedAtEq,
    filterLastSyncedAtNotEq,
    filterLastSyncedAtBefore,
    filterLastSyncedAtAfter,
    filterLastSyncedAtGte,
    filterLastSyncedAtLte,
    filterLastSyncedAtBetweenStart,
    filterLastSyncedAtBetweenEnd,
    filterLastSyncedAtIsNull,
    filterLastSyncedAtRelativeDays,
    filterHasChecksumEq,
    filterHasChecksumIsNull,
    searchTerm,
    searchFields,
    searchType,
    searchMinScore,
    searchOptionsCaseSensitive,
    searchOptionsMinTermLength,
    searchOptionsMaxResults,
    searchOptionsMultiTermAnd,
    paginationPageSize,
    paginationPageToken,
    paginationOrderBy,
    paginationOrder
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filterBlockchainEq** | [**number**] | Equals | (optional) defaults to undefined|
| **filterBlockchainNotEq** | [**number**] | Not equal to | (optional) defaults to undefined|
| **filterBlockchainIn** | **Array&lt;number&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterBlockchainNotIn** | **Array&lt;number&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterBlockchainIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterBlockchainGt** | [**number**] | Greater than | (optional) defaults to undefined|
| **filterBlockchainGte** | [**number**] | Greater than or equal to | (optional) defaults to undefined|
| **filterBlockchainLt** | [**number**] | Less than | (optional) defaults to undefined|
| **filterBlockchainLte** | [**number**] | Less than or equal to | (optional) defaults to undefined|
| **filterEnabledEq** | [**boolean**] | Equals | (optional) defaults to undefined|
| **filterEnabledIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterIsVettedEq** | [**boolean**] | Equals | (optional) defaults to undefined|
| **filterIsVettedIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterStandardEq** | [**number**] | Equals | (optional) defaults to undefined|
| **filterStandardNotEq** | [**number**] | Not equal to | (optional) defaults to undefined|
| **filterStandardIn** | **Array&lt;number&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterStandardNotIn** | **Array&lt;number&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterStandardIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterStandardGt** | [**number**] | Greater than | (optional) defaults to undefined|
| **filterStandardGte** | [**number**] | Greater than or equal to | (optional) defaults to undefined|
| **filterStandardLt** | [**number**] | Less than | (optional) defaults to undefined|
| **filterStandardLte** | [**number**] | Less than or equal to | (optional) defaults to undefined|
| **filterOrganizationIdEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterOrganizationIdNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterOrganizationIdContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterOrganizationIdStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterOrganizationIdEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterOrganizationIdIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterOrganizationIdNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterOrganizationIdRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterOrganizationIdIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterOrganizationIdFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterOrganizationIdFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterSymbolEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterSymbolNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterSymbolContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterSymbolNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterSymbolRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterSymbolIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterSymbolFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterSymbolFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterNameEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterNameNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterNameContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterNameStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterNameEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterNameIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterNameNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterNameRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterNameIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterNameFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterNameFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterContractAddressEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterContractAddressNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterContractAddressContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterContractAddressStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterContractAddressEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterContractAddressIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterContractAddressNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterContractAddressRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterContractAddressIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterContractAddressFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterContractAddressFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterSourceEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterSourceNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterSourceContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterSourceStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterSourceEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterSourceIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterSourceNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterSourceRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterSourceIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterSourceFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterSourceFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterLastSyncedAtEq** | [**string**] | Exact timestamp match | (optional) defaults to undefined|
| **filterLastSyncedAtNotEq** | [**string**] | Not equal to timestamp | (optional) defaults to undefined|
| **filterLastSyncedAtBefore** | [**string**] | Before this timestamp | (optional) defaults to undefined|
| **filterLastSyncedAtAfter** | [**string**] | After this timestamp | (optional) defaults to undefined|
| **filterLastSyncedAtGte** | [**string**] | Greater than or equal to timestamp | (optional) defaults to undefined|
| **filterLastSyncedAtLte** | [**string**] | Less than or equal to timestamp | (optional) defaults to undefined|
| **filterLastSyncedAtBetweenStart** | [**string**] | Start of time range (inclusive) | (optional) defaults to undefined|
| **filterLastSyncedAtBetweenEnd** | [**string**] | End of time range (inclusive) | (optional) defaults to undefined|
| **filterLastSyncedAtIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterLastSyncedAtRelativeDays** | [**number**] | Relative days from now (negative for past, positive for future) | (optional) defaults to undefined|
| **filterHasChecksumEq** | [**boolean**] | Equals | (optional) defaults to undefined|
| **filterHasChecksumIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **searchTerm** | [**string**] | Search term | (optional) defaults to undefined|
| **searchFields** | **Array&lt;string&gt;** | Fields to search in | (optional) defaults to undefined|
| **searchType** | [**&#39;SEARCH_TYPE_CONTAINS&#39; | &#39;SEARCH_TYPE_STARTS_WITH&#39; | &#39;SEARCH_TYPE_EXACT&#39; | &#39;SEARCH_TYPE_FUZZY&#39; | &#39;SEARCH_TYPE_FULLTEXT&#39;**]**Array<&#39;SEARCH_TYPE_CONTAINS&#39; &#124; &#39;SEARCH_TYPE_STARTS_WITH&#39; &#124; &#39;SEARCH_TYPE_EXACT&#39; &#124; &#39;SEARCH_TYPE_FUZZY&#39; &#124; &#39;SEARCH_TYPE_FULLTEXT&#39;>** | Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) | (optional) defaults to undefined|
| **searchMinScore** | [**number**] | Minimum relevance score for fuzzy/fulltext search | (optional) defaults to undefined|
| **searchOptionsCaseSensitive** | [**boolean**] | Enable case-sensitive search (default: false) | (optional) defaults to undefined|
| **searchOptionsMinTermLength** | [**number**] | Minimum search term length | (optional) defaults to undefined|
| **searchOptionsMaxResults** | [**number**] | Maximum number of results to return | (optional) defaults to undefined|
| **searchOptionsMultiTermAnd** | [**boolean**] | Use AND logic for multiple terms (default: false for OR) | (optional) defaults to undefined|
| **paginationPageSize** | [**number**] | Number of results per page (default 50, max 1000) | (optional) defaults to undefined|
| **paginationPageToken** | [**string**] | Token for pagination from previous response | (optional) defaults to undefined|
| **paginationOrderBy** | [**string**] | Field to order results by | (optional) defaults to undefined|
| **paginationOrder** | [**&#39;SORT_ORDER_ASC&#39; | &#39;SORT_ORDER_DESC&#39;**]**Array<&#39;SORT_ORDER_ASC&#39; &#124; &#39;SORT_ORDER_DESC&#39;>** | Sort order (ASC or DESC) | (optional) defaults to undefined|


### Return type

**V2ListAssetsResponse**

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

# **registryServiceListBlockchains**
> V2ListBlockchainsResponse registryServiceListBlockchains(v2ListBlockchainsRequest)

List blockchains with advanced filtering. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ListBlockchainsRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ListBlockchainsRequest: V2ListBlockchainsRequest; //

const { status, data } = await apiInstance.registryServiceListBlockchains(
    v2ListBlockchainsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ListBlockchainsRequest** | **V2ListBlockchainsRequest**|  | |


### Return type

**V2ListBlockchainsResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **registryServiceListBlockchains2**
> V2ListBlockchainsResponse registryServiceListBlockchains2()

List blockchains with advanced filtering. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let filterStatusEq: number; //Equals (optional) (default to undefined)
let filterStatusNotEq: number; //Not equal to (optional) (default to undefined)
let filterStatusIn: Array<number>; //Value is in the list (optional) (default to undefined)
let filterStatusNotIn: Array<number>; //Value is not in the list (optional) (default to undefined)
let filterStatusIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterStatusGt: number; //Greater than (optional) (default to undefined)
let filterStatusGte: number; //Greater than or equal to (optional) (default to undefined)
let filterStatusLt: number; //Less than (optional) (default to undefined)
let filterStatusLte: number; //Less than or equal to (optional) (default to undefined)
let filterNameEq: string; //Exact match (optional) (default to undefined)
let filterNameNotEq: string; //Not equal to (optional) (default to undefined)
let filterNameContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterNameStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterNameEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterNameIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterNameNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterNameRegex: string; //Regular expression match (optional) (default to undefined)
let filterNameIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterNameFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterNameFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterChainIdEq: string; //Exact match (optional) (default to undefined)
let filterChainIdNotEq: string; //Not equal to (optional) (default to undefined)
let filterChainIdContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterChainIdStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterChainIdEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterChainIdIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterChainIdNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterChainIdRegex: string; //Regular expression match (optional) (default to undefined)
let filterChainIdIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterChainIdFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterChainIdFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterChecksumTypeEq: number; //Equals (optional) (default to undefined)
let filterChecksumTypeNotEq: number; //Not equal to (optional) (default to undefined)
let filterChecksumTypeIn: Array<number>; //Value is in the list (optional) (default to undefined)
let filterChecksumTypeNotIn: Array<number>; //Value is not in the list (optional) (default to undefined)
let filterChecksumTypeIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterChecksumTypeGt: number; //Greater than (optional) (default to undefined)
let filterChecksumTypeGte: number; //Greater than or equal to (optional) (default to undefined)
let filterChecksumTypeLt: number; //Less than (optional) (default to undefined)
let filterChecksumTypeLte: number; //Less than or equal to (optional) (default to undefined)
let filterChainEq: string; //Exact match (optional) (default to undefined)
let filterChainNotEq: string; //Not equal to (optional) (default to undefined)
let filterChainContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterChainStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterChainEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterChainIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterChainNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterChainRegex: string; //Regular expression match (optional) (default to undefined)
let filterChainIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterChainFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterChainFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let searchTerm: string; //Search term (optional) (default to undefined)
let searchFields: Array<string>; //Fields to search in (optional) (default to undefined)
let searchType: 'SEARCH_TYPE_CONTAINS' | 'SEARCH_TYPE_STARTS_WITH' | 'SEARCH_TYPE_EXACT' | 'SEARCH_TYPE_FUZZY' | 'SEARCH_TYPE_FULLTEXT'; //Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) (optional) (default to undefined)
let searchMinScore: number; //Minimum relevance score for fuzzy/fulltext search (optional) (default to undefined)
let searchOptionsCaseSensitive: boolean; //Enable case-sensitive search (default: false) (optional) (default to undefined)
let searchOptionsMinTermLength: number; //Minimum search term length (optional) (default to undefined)
let searchOptionsMaxResults: number; //Maximum number of results to return (optional) (default to undefined)
let searchOptionsMultiTermAnd: boolean; //Use AND logic for multiple terms (default: false for OR) (optional) (default to undefined)
let paginationPageSize: number; //Number of results per page (default 50, max 1000) (optional) (default to undefined)
let paginationPageToken: string; //Token for pagination from previous response (optional) (default to undefined)
let paginationOrderBy: string; //Field to order results by (optional) (default to undefined)
let paginationOrder: 'SORT_ORDER_ASC' | 'SORT_ORDER_DESC'; //Sort order (ASC or DESC) (optional) (default to undefined)

const { status, data } = await apiInstance.registryServiceListBlockchains2(
    filterStatusEq,
    filterStatusNotEq,
    filterStatusIn,
    filterStatusNotIn,
    filterStatusIsNull,
    filterStatusGt,
    filterStatusGte,
    filterStatusLt,
    filterStatusLte,
    filterNameEq,
    filterNameNotEq,
    filterNameContains,
    filterNameStartsWith,
    filterNameEndsWith,
    filterNameIn,
    filterNameNotIn,
    filterNameRegex,
    filterNameIsNull,
    filterNameFuzzyValue,
    filterNameFuzzyMinSimilarity,
    filterChainIdEq,
    filterChainIdNotEq,
    filterChainIdContains,
    filterChainIdStartsWith,
    filterChainIdEndsWith,
    filterChainIdIn,
    filterChainIdNotIn,
    filterChainIdRegex,
    filterChainIdIsNull,
    filterChainIdFuzzyValue,
    filterChainIdFuzzyMinSimilarity,
    filterChecksumTypeEq,
    filterChecksumTypeNotEq,
    filterChecksumTypeIn,
    filterChecksumTypeNotIn,
    filterChecksumTypeIsNull,
    filterChecksumTypeGt,
    filterChecksumTypeGte,
    filterChecksumTypeLt,
    filterChecksumTypeLte,
    filterChainEq,
    filterChainNotEq,
    filterChainContains,
    filterChainStartsWith,
    filterChainEndsWith,
    filterChainIn,
    filterChainNotIn,
    filterChainRegex,
    filterChainIsNull,
    filterChainFuzzyValue,
    filterChainFuzzyMinSimilarity,
    searchTerm,
    searchFields,
    searchType,
    searchMinScore,
    searchOptionsCaseSensitive,
    searchOptionsMinTermLength,
    searchOptionsMaxResults,
    searchOptionsMultiTermAnd,
    paginationPageSize,
    paginationPageToken,
    paginationOrderBy,
    paginationOrder
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filterStatusEq** | [**number**] | Equals | (optional) defaults to undefined|
| **filterStatusNotEq** | [**number**] | Not equal to | (optional) defaults to undefined|
| **filterStatusIn** | **Array&lt;number&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterStatusNotIn** | **Array&lt;number&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterStatusIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterStatusGt** | [**number**] | Greater than | (optional) defaults to undefined|
| **filterStatusGte** | [**number**] | Greater than or equal to | (optional) defaults to undefined|
| **filterStatusLt** | [**number**] | Less than | (optional) defaults to undefined|
| **filterStatusLte** | [**number**] | Less than or equal to | (optional) defaults to undefined|
| **filterNameEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterNameNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterNameContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterNameStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterNameEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterNameIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterNameNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterNameRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterNameIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterNameFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterNameFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterChainIdEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterChainIdNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterChainIdContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterChainIdStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterChainIdEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterChainIdIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterChainIdNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterChainIdRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterChainIdIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterChainIdFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterChainIdFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterChecksumTypeEq** | [**number**] | Equals | (optional) defaults to undefined|
| **filterChecksumTypeNotEq** | [**number**] | Not equal to | (optional) defaults to undefined|
| **filterChecksumTypeIn** | **Array&lt;number&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterChecksumTypeNotIn** | **Array&lt;number&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterChecksumTypeIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterChecksumTypeGt** | [**number**] | Greater than | (optional) defaults to undefined|
| **filterChecksumTypeGte** | [**number**] | Greater than or equal to | (optional) defaults to undefined|
| **filterChecksumTypeLt** | [**number**] | Less than | (optional) defaults to undefined|
| **filterChecksumTypeLte** | [**number**] | Less than or equal to | (optional) defaults to undefined|
| **filterChainEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterChainNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterChainContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterChainStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterChainEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterChainIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterChainNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterChainRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterChainIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterChainFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterChainFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **searchTerm** | [**string**] | Search term | (optional) defaults to undefined|
| **searchFields** | **Array&lt;string&gt;** | Fields to search in | (optional) defaults to undefined|
| **searchType** | [**&#39;SEARCH_TYPE_CONTAINS&#39; | &#39;SEARCH_TYPE_STARTS_WITH&#39; | &#39;SEARCH_TYPE_EXACT&#39; | &#39;SEARCH_TYPE_FUZZY&#39; | &#39;SEARCH_TYPE_FULLTEXT&#39;**]**Array<&#39;SEARCH_TYPE_CONTAINS&#39; &#124; &#39;SEARCH_TYPE_STARTS_WITH&#39; &#124; &#39;SEARCH_TYPE_EXACT&#39; &#124; &#39;SEARCH_TYPE_FUZZY&#39; &#124; &#39;SEARCH_TYPE_FULLTEXT&#39;>** | Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) | (optional) defaults to undefined|
| **searchMinScore** | [**number**] | Minimum relevance score for fuzzy/fulltext search | (optional) defaults to undefined|
| **searchOptionsCaseSensitive** | [**boolean**] | Enable case-sensitive search (default: false) | (optional) defaults to undefined|
| **searchOptionsMinTermLength** | [**number**] | Minimum search term length | (optional) defaults to undefined|
| **searchOptionsMaxResults** | [**number**] | Maximum number of results to return | (optional) defaults to undefined|
| **searchOptionsMultiTermAnd** | [**boolean**] | Use AND logic for multiple terms (default: false for OR) | (optional) defaults to undefined|
| **paginationPageSize** | [**number**] | Number of results per page (default 50, max 1000) | (optional) defaults to undefined|
| **paginationPageToken** | [**string**] | Token for pagination from previous response | (optional) defaults to undefined|
| **paginationOrderBy** | [**string**] | Field to order results by | (optional) defaults to undefined|
| **paginationOrder** | [**&#39;SORT_ORDER_ASC&#39; | &#39;SORT_ORDER_DESC&#39;**]**Array<&#39;SORT_ORDER_ASC&#39; &#124; &#39;SORT_ORDER_DESC&#39;>** | Sort order (ASC or DESC) | (optional) defaults to undefined|


### Return type

**V2ListBlockchainsResponse**

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

# **registryServiceListCurrencies**
> V2ListCurrenciesResponse registryServiceListCurrencies(v2ListCurrenciesRequest)

List currencies with advanced filtering. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    V2ListCurrenciesRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let v2ListCurrenciesRequest: V2ListCurrenciesRequest; //

const { status, data } = await apiInstance.registryServiceListCurrencies(
    v2ListCurrenciesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2ListCurrenciesRequest** | **V2ListCurrenciesRequest**|  | |


### Return type

**V2ListCurrenciesResponse**

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

# **registryServiceListCurrencies2**
> V2ListCurrenciesResponse registryServiceListCurrencies2()

List currencies with advanced filtering. Supports both GET (bookmarkable) and POST (complex filters).

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let filterEnabledEq: boolean; //Equals (optional) (default to undefined)
let filterEnabledIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterNameEq: string; //Exact match (optional) (default to undefined)
let filterNameNotEq: string; //Not equal to (optional) (default to undefined)
let filterNameContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterNameStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterNameEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterNameIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterNameNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterNameRegex: string; //Regular expression match (optional) (default to undefined)
let filterNameIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterNameFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterNameFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterCodeEq: string; //Exact match (optional) (default to undefined)
let filterCodeNotEq: string; //Not equal to (optional) (default to undefined)
let filterCodeContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterCodeStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterCodeEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterCodeIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterCodeNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterCodeRegex: string; //Regular expression match (optional) (default to undefined)
let filterCodeIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterCodeFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterCodeFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let filterSymbolEq: string; //Exact match (optional) (default to undefined)
let filterSymbolNotEq: string; //Not equal to (optional) (default to undefined)
let filterSymbolContains: string; //Contains substring (case-insensitive) (optional) (default to undefined)
let filterSymbolStartsWith: string; //Starts with prefix (case-insensitive) (optional) (default to undefined)
let filterSymbolEndsWith: string; //Ends with suffix (case-insensitive) (optional) (default to undefined)
let filterSymbolIn: Array<string>; //Value is in the list (optional) (default to undefined)
let filterSymbolNotIn: Array<string>; //Value is not in the list (optional) (default to undefined)
let filterSymbolRegex: string; //Regular expression match (optional) (default to undefined)
let filterSymbolIsNull: boolean; //Check if field is null (optional) (default to undefined)
let filterSymbolFuzzyValue: string; //Value to match against (optional) (default to undefined)
let filterSymbolFuzzyMinSimilarity: number; //Minimum similarity threshold (0.0-1.0) (optional) (default to undefined)
let searchTerm: string; //Search term (optional) (default to undefined)
let searchFields: Array<string>; //Fields to search in (optional) (default to undefined)
let searchType: 'SEARCH_TYPE_CONTAINS' | 'SEARCH_TYPE_STARTS_WITH' | 'SEARCH_TYPE_EXACT' | 'SEARCH_TYPE_FUZZY' | 'SEARCH_TYPE_FULLTEXT'; //Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) (optional) (default to undefined)
let searchMinScore: number; //Minimum relevance score for fuzzy/fulltext search (optional) (default to undefined)
let searchOptionsCaseSensitive: boolean; //Enable case-sensitive search (default: false) (optional) (default to undefined)
let searchOptionsMinTermLength: number; //Minimum search term length (optional) (default to undefined)
let searchOptionsMaxResults: number; //Maximum number of results to return (optional) (default to undefined)
let searchOptionsMultiTermAnd: boolean; //Use AND logic for multiple terms (default: false for OR) (optional) (default to undefined)
let paginationPageSize: number; //Number of results per page (default 50, max 1000) (optional) (default to undefined)
let paginationPageToken: string; //Token for pagination from previous response (optional) (default to undefined)
let paginationOrderBy: string; //Field to order results by (optional) (default to undefined)
let paginationOrder: 'SORT_ORDER_ASC' | 'SORT_ORDER_DESC'; //Sort order (ASC or DESC) (optional) (default to undefined)

const { status, data } = await apiInstance.registryServiceListCurrencies2(
    filterEnabledEq,
    filterEnabledIsNull,
    filterNameEq,
    filterNameNotEq,
    filterNameContains,
    filterNameStartsWith,
    filterNameEndsWith,
    filterNameIn,
    filterNameNotIn,
    filterNameRegex,
    filterNameIsNull,
    filterNameFuzzyValue,
    filterNameFuzzyMinSimilarity,
    filterCodeEq,
    filterCodeNotEq,
    filterCodeContains,
    filterCodeStartsWith,
    filterCodeEndsWith,
    filterCodeIn,
    filterCodeNotIn,
    filterCodeRegex,
    filterCodeIsNull,
    filterCodeFuzzyValue,
    filterCodeFuzzyMinSimilarity,
    filterSymbolEq,
    filterSymbolNotEq,
    filterSymbolContains,
    filterSymbolStartsWith,
    filterSymbolEndsWith,
    filterSymbolIn,
    filterSymbolNotIn,
    filterSymbolRegex,
    filterSymbolIsNull,
    filterSymbolFuzzyValue,
    filterSymbolFuzzyMinSimilarity,
    searchTerm,
    searchFields,
    searchType,
    searchMinScore,
    searchOptionsCaseSensitive,
    searchOptionsMinTermLength,
    searchOptionsMaxResults,
    searchOptionsMultiTermAnd,
    paginationPageSize,
    paginationPageToken,
    paginationOrderBy,
    paginationOrder
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filterEnabledEq** | [**boolean**] | Equals | (optional) defaults to undefined|
| **filterEnabledIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterNameEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterNameNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterNameContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterNameStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterNameEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterNameIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterNameNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterNameRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterNameIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterNameFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterNameFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterCodeEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterCodeNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterCodeContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterCodeStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterCodeEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterCodeIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterCodeNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterCodeRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterCodeIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterCodeFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterCodeFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **filterSymbolEq** | [**string**] | Exact match | (optional) defaults to undefined|
| **filterSymbolNotEq** | [**string**] | Not equal to | (optional) defaults to undefined|
| **filterSymbolContains** | [**string**] | Contains substring (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolStartsWith** | [**string**] | Starts with prefix (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolEndsWith** | [**string**] | Ends with suffix (case-insensitive) | (optional) defaults to undefined|
| **filterSymbolIn** | **Array&lt;string&gt;** | Value is in the list | (optional) defaults to undefined|
| **filterSymbolNotIn** | **Array&lt;string&gt;** | Value is not in the list | (optional) defaults to undefined|
| **filterSymbolRegex** | [**string**] | Regular expression match | (optional) defaults to undefined|
| **filterSymbolIsNull** | [**boolean**] | Check if field is null | (optional) defaults to undefined|
| **filterSymbolFuzzyValue** | [**string**] | Value to match against | (optional) defaults to undefined|
| **filterSymbolFuzzyMinSimilarity** | [**number**] | Minimum similarity threshold (0.0-1.0) | (optional) defaults to undefined|
| **searchTerm** | [**string**] | Search term | (optional) defaults to undefined|
| **searchFields** | **Array&lt;string&gt;** | Fields to search in | (optional) defaults to undefined|
| **searchType** | [**&#39;SEARCH_TYPE_CONTAINS&#39; | &#39;SEARCH_TYPE_STARTS_WITH&#39; | &#39;SEARCH_TYPE_EXACT&#39; | &#39;SEARCH_TYPE_FUZZY&#39; | &#39;SEARCH_TYPE_FULLTEXT&#39;**]**Array<&#39;SEARCH_TYPE_CONTAINS&#39; &#124; &#39;SEARCH_TYPE_STARTS_WITH&#39; &#124; &#39;SEARCH_TYPE_EXACT&#39; &#124; &#39;SEARCH_TYPE_FUZZY&#39; &#124; &#39;SEARCH_TYPE_FULLTEXT&#39;>** | Type of search to perform   - SEARCH_TYPE_CONTAINS: Default substring search  - SEARCH_TYPE_STARTS_WITH: Prefix search  - SEARCH_TYPE_EXACT: Exact match  - SEARCH_TYPE_FUZZY: Fuzzy/similarity search  - SEARCH_TYPE_FULLTEXT: Full-text search (future) | (optional) defaults to undefined|
| **searchMinScore** | [**number**] | Minimum relevance score for fuzzy/fulltext search | (optional) defaults to undefined|
| **searchOptionsCaseSensitive** | [**boolean**] | Enable case-sensitive search (default: false) | (optional) defaults to undefined|
| **searchOptionsMinTermLength** | [**number**] | Minimum search term length | (optional) defaults to undefined|
| **searchOptionsMaxResults** | [**number**] | Maximum number of results to return | (optional) defaults to undefined|
| **searchOptionsMultiTermAnd** | [**boolean**] | Use AND logic for multiple terms (default: false for OR) | (optional) defaults to undefined|
| **paginationPageSize** | [**number**] | Number of results per page (default 50, max 1000) | (optional) defaults to undefined|
| **paginationPageToken** | [**string**] | Token for pagination from previous response | (optional) defaults to undefined|
| **paginationOrderBy** | [**string**] | Field to order results by | (optional) defaults to undefined|
| **paginationOrder** | [**&#39;SORT_ORDER_ASC&#39; | &#39;SORT_ORDER_DESC&#39;**]**Array<&#39;SORT_ORDER_ASC&#39; &#124; &#39;SORT_ORDER_DESC&#39;>** | Sort order (ASC or DESC) | (optional) defaults to undefined|


### Return type

**V2ListCurrenciesResponse**

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

