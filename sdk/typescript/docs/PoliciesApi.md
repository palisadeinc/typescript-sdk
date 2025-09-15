# PoliciesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**policyServiceCreateWalletLimit**](#policyservicecreatewalletlimit) | **PUT** /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits | Create a wallet limit policy|
|[**policyServiceDeleteWalletLimit**](#policyservicedeletewalletlimit) | **DELETE** /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits/{id} | Delete a wallet limit policy|
|[**policyServiceGetWalletLimit**](#policyservicegetwalletlimit) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits/{id} | Get a wallet limit policy|
|[**policyServiceListGlobalWalletLimits**](#policyservicelistglobalwalletlimits) | **GET** /v2/policy-rules/limits | List organization wallet limits|
|[**policyServiceListPermittedDestinations**](#policyservicelistpermitteddestinations) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/permitted-destinations | List permitted destinations|
|[**policyServiceListWalletLimits**](#policyservicelistwalletlimits) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits | List wallet limit policies|

# **policyServiceCreateWalletLimit**
> V2WalletLimit policyServiceCreateWalletLimit(policyServiceCreateWalletLimitRequest)

Create a wallet limit policy for the specified wallet

### Example

```typescript
import {
    PoliciesApi,
    Configuration,
    PolicyServiceCreateWalletLimitRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let policyServiceCreateWalletLimitRequest: PolicyServiceCreateWalletLimitRequest; //

const { status, data } = await apiInstance.policyServiceCreateWalletLimit(
    vaultId,
    walletId,
    policyServiceCreateWalletLimitRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **policyServiceCreateWalletLimitRequest** | **PolicyServiceCreateWalletLimitRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**V2WalletLimit**

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

# **policyServiceDeleteWalletLimit**
> object policyServiceDeleteWalletLimit()

Delete the specified wallet limit policy

### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let id: string; //The wallet limit policy ID (default to undefined)

const { status, data } = await apiInstance.policyServiceDeleteWalletLimit(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **id** | [**string**] | The wallet limit policy ID | defaults to undefined|


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

# **policyServiceGetWalletLimit**
> V2WalletLimit policyServiceGetWalletLimit()

Get the specified wallet limit policy

### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let id: string; //The wallet limit policy ID (default to undefined)

const { status, data } = await apiInstance.policyServiceGetWalletLimit(
    vaultId,
    walletId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **id** | [**string**] | The wallet limit policy ID | defaults to undefined|


### Return type

**V2WalletLimit**

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

# **policyServiceListGlobalWalletLimits**
> V2ListGlobalWalletLimitsResponse policyServiceListGlobalWalletLimits()

List all wallet limits within the organization

### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.policyServiceListGlobalWalletLimits(
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListGlobalWalletLimitsResponse**

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

# **policyServiceListPermittedDestinations**
> V2ListPermittedDestinationsResponse policyServiceListPermittedDestinations()

List all permitted destinations for this wallet

### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.policyServiceListPermittedDestinations(
    vaultId,
    walletId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListPermittedDestinationsResponse**

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

# **policyServiceListWalletLimits**
> V2ListWalletLimitsResponse policyServiceListWalletLimits()

List wallet limit policies for the specified wallet

### Example

```typescript
import {
    PoliciesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new PoliciesApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.policyServiceListWalletLimits(
    vaultId,
    walletId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListWalletLimitsResponse**

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

