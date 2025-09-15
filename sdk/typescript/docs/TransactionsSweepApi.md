# TransactionsSweepApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**transactionsServiceListSweepInstanceTransactions**](#transactionsservicelistsweepinstancetransactions) | **GET** /v2/transactions/sweep/{sweepId} | List transactions for a sweep instance|

# **transactionsServiceListSweepInstanceTransactions**
> V2ListSweepInstanceTransactionsResponse transactionsServiceListSweepInstanceTransactions()

List all transactions for a given sweep instance

### Example

```typescript
import {
    TransactionsSweepApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new TransactionsSweepApi(configuration);

let sweepId: string; // (default to undefined)
let correlationId: string; //Correlation ID for this request, used to correlate multiple actions (optional) (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.transactionsServiceListSweepInstanceTransactions(
    sweepId,
    correlationId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sweepId** | [**string**] |  | defaults to undefined|
| **correlationId** | [**string**] | Correlation ID for this request, used to correlate multiple actions | (optional) defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListSweepInstanceTransactionsResponse**

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

