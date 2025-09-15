# AuditApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**auditServiceGetFirehoseConfiguration**](#auditservicegetfirehoseconfiguration) | **GET** /v2/audit/firehose/configuration | Get the Firehose configuration for streaming audit events|
|[**auditServiceSetFirehoseConfiguration**](#auditservicesetfirehoseconfiguration) | **PUT** /v2/audit/firehose/configuration | Set the Firehose configuration for streaming audit events|

# **auditServiceGetFirehoseConfiguration**
> V2FirehoseConfiguration auditServiceGetFirehoseConfiguration()

Get the Firehose configuration for streaming audit events

### Example

```typescript
import {
    AuditApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AuditApi(configuration);

const { status, data } = await apiInstance.auditServiceGetFirehoseConfiguration();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2FirehoseConfiguration**

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

# **auditServiceSetFirehoseConfiguration**
> V2FirehoseConfiguration auditServiceSetFirehoseConfiguration(v2FirehoseConfiguration)

Set the Firehose configuration for streaming audit events

### Example

```typescript
import {
    AuditApi,
    Configuration,
    V2FirehoseConfiguration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new AuditApi(configuration);

let v2FirehoseConfiguration: V2FirehoseConfiguration; //

const { status, data } = await apiInstance.auditServiceSetFirehoseConfiguration(
    v2FirehoseConfiguration
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2FirehoseConfiguration** | **V2FirehoseConfiguration**|  | |


### Return type

**V2FirehoseConfiguration**

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

