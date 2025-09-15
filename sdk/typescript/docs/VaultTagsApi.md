# VaultTagsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vaultServiceAddVaultTag**](#vaultserviceaddvaulttag) | **POST** /v2/vaults/{vaultId}/tags | Add a new vault tag|
|[**vaultServiceDeleteVaultTag**](#vaultservicedeletevaulttag) | **DELETE** /v2/vaults/{vaultId}/tags | Delete a vault tag|
|[**vaultServiceListGlobalVaultTags**](#vaultservicelistglobalvaulttags) | **GET** /v2/vaults/tags | List all vault tags for the organization|
|[**vaultServiceListVaultTags**](#vaultservicelistvaulttags) | **GET** /v2/vaults/{vaultId}/tags | List tags for the vault|

# **vaultServiceAddVaultTag**
> Array<V2VaultTag> vaultServiceAddVaultTag(vaultServiceAddVaultTagRequest)

Add a new vault tag to a vault

### Example

```typescript
import {
    VaultTagsApi,
    Configuration,
    VaultServiceAddVaultTagRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let vaultServiceAddVaultTagRequest: VaultServiceAddVaultTagRequest; //

const { status, data } = await apiInstance.vaultServiceAddVaultTag(
    vaultId,
    vaultServiceAddVaultTagRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultServiceAddVaultTagRequest** | **VaultServiceAddVaultTagRequest**|  | |
| **vaultId** | [**string**] | The vault ID | defaults to undefined|


### Return type

**Array<V2VaultTag>**

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

# **vaultServiceDeleteVaultTag**
> object vaultServiceDeleteVaultTag()

Delete a vault tag from a vault

### Example

```typescript
import {
    VaultTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)
let tag: string; //The tag (default to undefined)

const { status, data } = await apiInstance.vaultServiceDeleteVaultTag(
    vaultId,
    tag
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|
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

# **vaultServiceListGlobalVaultTags**
> Array<V2VaultTag> vaultServiceListGlobalVaultTags()

List all vault tags for the organization

### Example

```typescript
import {
    VaultTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultTagsApi(configuration);

const { status, data } = await apiInstance.vaultServiceListGlobalVaultTags();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2VaultTag>**

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

# **vaultServiceListVaultTags**
> Array<V2VaultTag> vaultServiceListVaultTags()

List all tags for the vault

### Example

```typescript
import {
    VaultTagsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new VaultTagsApi(configuration);

let vaultId: string; //The vault ID (default to undefined)

const { status, data } = await apiInstance.vaultServiceListVaultTags(
    vaultId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **vaultId** | [**string**] | The vault ID | defaults to undefined|


### Return type

**Array<V2VaultTag>**

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

