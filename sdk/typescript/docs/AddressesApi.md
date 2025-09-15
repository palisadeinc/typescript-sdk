# AddressesApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**counterpartyServiceCreateAddress**](#counterpartyservicecreateaddress) | **POST** /v2/counterparties/{counterpartyId}/addresses | Create addresses|
|[**counterpartyServiceDeleteAddress**](#counterpartyservicedeleteaddress) | **DELETE** /v2/counterparties/{counterpartyId}/addresses/{addressId} | Delete addresses|
|[**counterpartyServiceGetAddress**](#counterpartyservicegetaddress) | **GET** /v2/counterparties/{counterpartyId}/addresses/{addressId} | Get addresses|
|[**counterpartyServiceListAddresses**](#counterpartyservicelistaddresses) | **GET** /v2/counterparties/{counterpartyId}/addresses | List counterparty addresses|
|[**counterpartyServiceListGlobalAddresses**](#counterpartyservicelistglobaladdresses) | **GET** /v2/addresses | List organization addresses|

# **counterpartyServiceCreateAddress**
> Counterpartyv2Address counterpartyServiceCreateAddress(counterpartyServiceCreateAddressRequest)

Create a new address

### Example

```typescript
import {
    AddressesApi,
    Configuration,
    CounterpartyServiceCreateAddressRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AddressesApi(configuration);

let counterpartyId: string; //The counterparty ID (default to undefined)
let counterpartyServiceCreateAddressRequest: CounterpartyServiceCreateAddressRequest; //

const { status, data } = await apiInstance.counterpartyServiceCreateAddress(
    counterpartyId,
    counterpartyServiceCreateAddressRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **counterpartyServiceCreateAddressRequest** | **CounterpartyServiceCreateAddressRequest**|  | |
| **counterpartyId** | [**string**] | The counterparty ID | defaults to undefined|


### Return type

**Counterpartyv2Address**

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

# **counterpartyServiceDeleteAddress**
> object counterpartyServiceDeleteAddress()

Delete an address

### Example

```typescript
import {
    AddressesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AddressesApi(configuration);

let counterpartyId: string; //The counterparty ID (default to undefined)
let addressId: string; //The address ID (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceDeleteAddress(
    counterpartyId,
    addressId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **counterpartyId** | [**string**] | The counterparty ID | defaults to undefined|
| **addressId** | [**string**] | The address ID | defaults to undefined|


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

# **counterpartyServiceGetAddress**
> Counterpartyv2Address counterpartyServiceGetAddress()

Get an address

### Example

```typescript
import {
    AddressesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AddressesApi(configuration);

let counterpartyId: string; //The counterparty ID (default to undefined)
let addressId: string; //The address ID (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceGetAddress(
    counterpartyId,
    addressId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **counterpartyId** | [**string**] | The counterparty ID | defaults to undefined|
| **addressId** | [**string**] | The address ID | defaults to undefined|


### Return type

**Counterpartyv2Address**

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

# **counterpartyServiceListAddresses**
> V2ListAddressesResponse counterpartyServiceListAddresses()

List all addresses within a counterparty

### Example

```typescript
import {
    AddressesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AddressesApi(configuration);

let counterpartyId: string; //The counterparty ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 100) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceListAddresses(
    counterpartyId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **counterpartyId** | [**string**] | The counterparty ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 100) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListAddressesResponse**

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

# **counterpartyServiceListGlobalAddresses**
> V2ListGlobalAddressesResponse counterpartyServiceListGlobalAddresses()

List all addresses within the organization

### Example

```typescript
import {
    AddressesApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AddressesApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 1000) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)
let address: string; //The on-chain address to search for (optional) (default to undefined)

const { status, data } = await apiInstance.counterpartyServiceListGlobalAddresses(
    pageSize,
    pageToken,
    address
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 1000) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|
| **address** | [**string**] | The on-chain address to search for | (optional) defaults to undefined|


### Return type

**V2ListGlobalAddressesResponse**

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

