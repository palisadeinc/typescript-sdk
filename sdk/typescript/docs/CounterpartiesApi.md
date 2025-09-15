# CounterpartiesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**counterpartyServiceCreateCounterparty**](#counterpartyservicecreatecounterparty) | **POST** /v2/counterparties | Create counterparties|
|[**counterpartyServiceDeleteCounterparty**](#counterpartyservicedeletecounterparty) | **DELETE** /v2/counterparties/{id} | Delete counterparties|
|[**counterpartyServiceGetCounterparty**](#counterpartyservicegetcounterparty) | **GET** /v2/counterparties/{id} | Get counterparties|
|[**counterpartyServiceListCounterparties**](#counterpartyservicelistcounterparties) | **GET** /v2/counterparties | List counterparties|
|[**counterpartyServiceUpdateCounterparty**](#counterpartyserviceupdatecounterparty) | **PUT** /v2/counterparties/{id} | Update counterparties|

# **counterpartyServiceCreateCounterparty**
> V2Counterparty counterpartyServiceCreateCounterparty(v2CreateCounterpartyRequest)

Create a new counterparty

### Example

```typescript
import {
    CounterpartiesApi,
    Configuration,
    V2CreateCounterpartyRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CounterpartiesApi(configuration);

let v2CreateCounterpartyRequest: V2CreateCounterpartyRequest; //

const { status, data } = await apiInstance.counterpartyServiceCreateCounterparty(
    v2CreateCounterpartyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateCounterpartyRequest** | **V2CreateCounterpartyRequest**|  | |


### Return type

**V2Counterparty**

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

# **counterpartyServiceDeleteCounterparty**
> object counterpartyServiceDeleteCounterparty()

Delete a counterparty

### Example

```typescript
import {
    CounterpartiesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CounterpartiesApi(configuration);

let id: string; //The counterparty ID (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceDeleteCounterparty(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The counterparty ID | defaults to undefined|


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

# **counterpartyServiceGetCounterparty**
> V2Counterparty counterpartyServiceGetCounterparty()

Get a counterparty

### Example

```typescript
import {
    CounterpartiesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CounterpartiesApi(configuration);

let id: string; //The counterparty ID (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceGetCounterparty(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The counterparty ID | defaults to undefined|


### Return type

**V2Counterparty**

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

# **counterpartyServiceListCounterparties**
> V2ListCounterpartiesResponse counterpartyServiceListCounterparties()

List counterparties

### Example

```typescript
import {
    CounterpartiesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CounterpartiesApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceListCounterparties(
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

**V2ListCounterpartiesResponse**

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

# **counterpartyServiceUpdateCounterparty**
> V2Counterparty counterpartyServiceUpdateCounterparty(counterpartyServiceUpdateCounterpartyRequest)

Update a counterparty

### Example

```typescript
import {
    CounterpartiesApi,
    Configuration,
    CounterpartyServiceUpdateCounterpartyRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new CounterpartiesApi(configuration);

let id: string; //The counterparty ID (default to undefined)
let counterpartyServiceUpdateCounterpartyRequest: CounterpartyServiceUpdateCounterpartyRequest; //

const { status, data } = await apiInstance.counterpartyServiceUpdateCounterparty(
    id,
    counterpartyServiceUpdateCounterpartyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **counterpartyServiceUpdateCounterpartyRequest** | **CounterpartyServiceUpdateCounterpartyRequest**|  | |
| **id** | [**string**] | The counterparty ID | defaults to undefined|


### Return type

**V2Counterparty**

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

