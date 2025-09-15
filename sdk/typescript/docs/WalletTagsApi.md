# WalletTagsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vaultServiceAddWalletTag**](#vaultserviceaddwallettag) | **POST** /v2/vaults/{vaultId}/wallets/{walletId}/tags | Add a new wallet tag|
|[**vaultServiceDeleteWalletTag**](#vaultservicedeletewallettag) | **DELETE** /v2/vaults/{vaultId}/wallets/{walletId}/tags | Delete a wallet tag|
|[**vaultServiceListWalletTags**](#vaultservicelistwallettags) | **GET** /v2/vaults/{vaultId}/wallets/{walletId}/tags | List wallet tags for the wallet|
|[**vaultServiceListWalletTagsInVault**](#vaultservicelistwallettagsinvault) | **GET** /v2/vaults/{vaultId}/wallets/tags | List all wallet tags in vault|

# **vaultServiceAddWalletTag**
> Array<V2WalletTag> vaultServiceAddWalletTag(vaultServiceAddWalletTagRequest)

Add a new wallet tag to a wallet

### Example

```typescript
import {
    WalletTagsApi,
    Configuration,
    VaultServiceAddWalletTagRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let vaultServiceAddWalletTagRequest: VaultServiceAddWalletTagRequest; //

const { status, data } = await apiInstance.vaultServiceAddWalletTag(
    vaultId,
    walletId,
    vaultServiceAddWalletTagRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceAddWalletTagRequest** | **VaultServiceAddWalletTagRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Array<V2WalletTag>**

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

# **vaultServiceDeleteWalletTag**
> object vaultServiceDeleteWalletTag()

Delete a wallet tag from a wallet

### Example

```typescript
import {
    WalletTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)
let tag: string; //The tag (default to undefined)

const { status, data } = await apiInstance.vaultServiceDeleteWalletTag(
    vaultId,
    walletId,
    tag
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|
| **tag** | [**string**] | The tag | defaults to undefined|


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

# **vaultServiceListWalletTags**
> Array<V2WalletTag> vaultServiceListWalletTags()

List all wallet tags for the wallet

### Example

```typescript
import {
    WalletTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let walletId: string; //The wallet ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceListWalletTags(
    vaultId,
    walletId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
| **walletId** | [**string**] | The wallet ID | defaults to undefined|


### Return type

**Array<V2WalletTag>**

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

# **vaultServiceListWalletTagsInVault**
> Array<V2WalletTag> vaultServiceListWalletTagsInVault()

List all tags from all wallets in the vault

### Example

```typescript
import {
    WalletTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WalletTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceListWalletTagsInVault(
    vaultId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|


### Return type

**Array<V2WalletTag>**

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

