# RatesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**balanceServiceGetRate**](#balanceservicegetrate) | **GET** /v2/rates | Get rates|

# **balanceServiceGetRate**
> V2GetRateResponse balanceServiceGetRate()

Get the rate of a currency pair

### Example

```typescript
import {
    RatesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new RatesApi(configuration);

let blockchain: 'AVALANCHE' | 'ETHEREUM' | 'XRP_LEDGER' | 'POLYGON' | 'BNBCHAIN' | 'BASE' | 'HEDERA' | 'ARBITRUM' | 'ONE_MONEY' | 'SOLANA' | 'TRON' | 'BITCOIN'; // (default to undefined)
let symbol: string; //The asset symbol (default to undefined)
let currency: string; //The currency (must be USD) (default to undefined)
let contract: string; //The contract/issuing address (optional) (default to undefined)

const { status, data } = await apiInstance.balanceServiceGetRate(
    blockchain,
    symbol,
    currency,
    contract
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **blockchain** | [**&#39;AVALANCHE&#39; | &#39;ETHEREUM&#39; | &#39;XRP_LEDGER&#39; | &#39;POLYGON&#39; | &#39;BNBCHAIN&#39; | &#39;BASE&#39; | &#39;HEDERA&#39; | &#39;ARBITRUM&#39; | &#39;ONE_MONEY&#39; | &#39;SOLANA&#39; | &#39;TRON&#39; | &#39;BITCOIN&#39;**]**Array<&#39;AVALANCHE&#39; &#124; &#39;ETHEREUM&#39; &#124; &#39;XRP_LEDGER&#39; &#124; &#39;POLYGON&#39; &#124; &#39;BNBCHAIN&#39; &#124; &#39;BASE&#39; &#124; &#39;HEDERA&#39; &#124; &#39;ARBITRUM&#39; &#124; &#39;ONE_MONEY&#39; &#124; &#39;SOLANA&#39; &#124; &#39;TRON&#39; &#124; &#39;BITCOIN&#39;>** |  | defaults to undefined|
| **symbol** | [**string**] | The asset symbol | defaults to undefined|
| **currency** | [**string**] | The currency (must be USD) | defaults to undefined|
| **contract** | [**string**] | The contract/issuing address | (optional) defaults to undefined|


### Return type

**V2GetRateResponse**

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

