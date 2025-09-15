# InformationApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**balanceServiceListSupportedAssets**](#balanceservicelistsupportedassets) | **GET** /v2/info/supported-assets | List Supported Assets|
|[**balanceServiceListSupportedCurrencies**](#balanceservicelistsupportedcurrencies) | **GET** /v2/info/supported-currencies | List Supported Currencies|

# **balanceServiceListSupportedAssets**
> Array<Commonv2Asset> balanceServiceListSupportedAssets()

Get the list of supported assets

### Example

```typescript
import {
    InformationApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new InformationApi(configuration);

let blockchain: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; // (optional) (default to undefined)

const { status, data } = await apiInstance.balanceServiceListSupportedAssets(
    blockchain
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **blockchain** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** |  | (optional) defaults to undefined|


### Return type

**Array<Commonv2Asset>**

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

# **balanceServiceListSupportedCurrencies**
> Array<V2Currency> balanceServiceListSupportedCurrencies()

Get the list of supported currencies

### Example

```typescript
import {
    InformationApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new InformationApi(configuration);

const { status, data } = await apiInstance.balanceServiceListSupportedCurrencies();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2Currency>**

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

