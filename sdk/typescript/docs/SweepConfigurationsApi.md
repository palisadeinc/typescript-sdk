# SweepConfigurationsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sweepServiceCreateSweepConfiguration**](#sweepservicecreatesweepconfiguration) | **POST** /v2/workflows/sweep | Create sweep configuration|
|[**sweepServiceDeleteSweepConfiguration**](#sweepservicedeletesweepconfiguration) | **DELETE** /v2/workflows/sweep/{id} | Delete sweep configuration|
|[**sweepServiceDisableSweepConfiguration**](#sweepservicedisablesweepconfiguration) | **POST** /v2/workflows/sweep/{id}/disable | Disable sweep configuration|
|[**sweepServiceEnableSweepConfiguration**](#sweepserviceenablesweepconfiguration) | **POST** /v2/workflows/sweep/{id}/enable | Enable sweep configuration|
|[**sweepServiceGetSweepConfiguration**](#sweepservicegetsweepconfiguration) | **GET** /v2/workflows/sweep/{id} | Get sweep configuration|
|[**sweepServiceListSweepConfigurations**](#sweepservicelistsweepconfigurations) | **GET** /v2/workflows/sweep | List sweep configurations|
|[**sweepServiceTriggerSweepConfiguration**](#sweepservicetriggersweepconfiguration) | **POST** /v2/workflows/sweep/{id}/trigger | Trigger a sweep configuration|

# **sweepServiceCreateSweepConfiguration**
> V2SweepConfiguration sweepServiceCreateSweepConfiguration(v2CreateSweepConfigurationRequest)

Create a new sweep configuration

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration,
    V2CreateSweepConfigurationRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let v2CreateSweepConfigurationRequest: V2CreateSweepConfigurationRequest; //

const { status, data } = await apiInstance.sweepServiceCreateSweepConfiguration(
    v2CreateSweepConfigurationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateSweepConfigurationRequest** | **V2CreateSweepConfigurationRequest**|  | |


### Return type

**V2SweepConfiguration**

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

# **sweepServiceDeleteSweepConfiguration**
> object sweepServiceDeleteSweepConfiguration()

Delete a single sweep configuration based on its ID

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let id: string; //The ID of the sweep configuration (default to undefined)

const { status, data } = await apiInstance.sweepServiceDeleteSweepConfiguration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep configuration | defaults to undefined|


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

# **sweepServiceDisableSweepConfiguration**
> V2SweepConfiguration sweepServiceDisableSweepConfiguration()

Disable a single sweep configuration based on its ID

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let id: string; //The ID of the sweep configuration (default to undefined)

const { status, data } = await apiInstance.sweepServiceDisableSweepConfiguration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep configuration | defaults to undefined|


### Return type

**V2SweepConfiguration**

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

# **sweepServiceEnableSweepConfiguration**
> V2SweepConfiguration sweepServiceEnableSweepConfiguration()

Enable a single sweep configuration based on its ID

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let id: string; //The ID of the sweep configuration (default to undefined)

const { status, data } = await apiInstance.sweepServiceEnableSweepConfiguration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep configuration | defaults to undefined|


### Return type

**V2SweepConfiguration**

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

# **sweepServiceGetSweepConfiguration**
> V2SweepConfiguration sweepServiceGetSweepConfiguration()

Get a single sweep configuration based on its ID

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let id: string; //The ID of the sweep configuration (default to undefined)

const { status, data } = await apiInstance.sweepServiceGetSweepConfiguration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep configuration | defaults to undefined|


### Return type

**V2SweepConfiguration**

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

# **sweepServiceListSweepConfigurations**
> V2ListSweepConfigurationsResponse sweepServiceListSweepConfigurations()

List sweep configurations

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 100) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.sweepServiceListSweepConfigurations(
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 100) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListSweepConfigurationsResponse**

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

# **sweepServiceTriggerSweepConfiguration**
> object sweepServiceTriggerSweepConfiguration()

Manually trigger a single sweep configuration based on its ID

### Example

```typescript
import {
    SweepConfigurationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new SweepConfigurationsApi(configuration);

let id: string; //The ID of the sweep configuration (default to undefined)

const { status, data } = await apiInstance.sweepServiceTriggerSweepConfiguration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The ID of the sweep configuration | defaults to undefined|


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

