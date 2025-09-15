# WebhooksApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**webhookServiceCreateSubscriptions**](#webhookservicecreatesubscriptions) | **POST** /v2/webhooks/{webhookId}/subscriptions | Create webhook subscriptions|
|[**webhookServiceCreateWebhook**](#webhookservicecreatewebhook) | **POST** /v2/webhooks | Create webhooks|
|[**webhookServiceDeleteSubscription**](#webhookservicedeletesubscription) | **DELETE** /v2/webhooks/{webhookId}/subscriptions/{subscriptionId} | Delete subscriptions|
|[**webhookServiceDeleteWebhook**](#webhookservicedeletewebhook) | **DELETE** /v2/webhooks/{id} | Delete webhooks|
|[**webhookServiceGetSubscription**](#webhookservicegetsubscription) | **GET** /v2/webhooks/{webhookId}/subscriptions/{subscriptionId} | Get subscriptions|
|[**webhookServiceGetWebhook**](#webhookservicegetwebhook) | **GET** /v2/webhooks/{id} | Get webhooks|
|[**webhookServiceListSubscriptions**](#webhookservicelistsubscriptions) | **GET** /v2/webhooks/{webhookId}/subscriptions | List subscriptions|
|[**webhookServiceListWebhooks**](#webhookservicelistwebhooks) | **GET** /v2/webhooks | List webhooks|

# **webhookServiceCreateSubscriptions**
> Array<V2Subscription> webhookServiceCreateSubscriptions(v2SubscriptionConfig)

Create one or more new webhook subscription

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let webhookId: string; //The webhook ID (default to undefined)
let v2SubscriptionConfig: Array<V2SubscriptionConfig>; //

const { status, data } = await apiInstance.webhookServiceCreateSubscriptions(
    webhookId,
    v2SubscriptionConfig
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2SubscriptionConfig** | **Array<V2SubscriptionConfig>**|  | |
| **webhookId** | [**string**] | The webhook ID | defaults to undefined|


### Return type

**Array<V2Subscription>**

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

# **webhookServiceCreateWebhook**
> V2Webhook webhookServiceCreateWebhook(v2CreateWebhookRequest)

Create a new webhook

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    V2CreateWebhookRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let v2CreateWebhookRequest: V2CreateWebhookRequest; //

const { status, data } = await apiInstance.webhookServiceCreateWebhook(
    v2CreateWebhookRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateWebhookRequest** | **V2CreateWebhookRequest**|  | |


### Return type

**V2Webhook**

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

# **webhookServiceDeleteSubscription**
> object webhookServiceDeleteSubscription()

Delete a single subscription based on its ID

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let webhookId: string; //The webhook ID (default to undefined)
let subscriptionId: string; //The subscription ID (default to undefined)

const { status, data } = await apiInstance.webhookServiceDeleteSubscription(
    webhookId,
    subscriptionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhookId** | [**string**] | The webhook ID | defaults to undefined|
| **subscriptionId** | [**string**] | The subscription ID | defaults to undefined|


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

# **webhookServiceDeleteWebhook**
> object webhookServiceDeleteWebhook()

Delete a single webhook based on its ID

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //The webhook ID (default to undefined)

const { status, data } = await apiInstance.webhookServiceDeleteWebhook(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The webhook ID | defaults to undefined|


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

# **webhookServiceGetSubscription**
> V2Subscription webhookServiceGetSubscription()

Get a single subscription based on its ID

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let webhookId: string; //The webhook ID (default to undefined)
let subscriptionId: string; //The subscription ID (default to undefined)

const { status, data } = await apiInstance.webhookServiceGetSubscription(
    webhookId,
    subscriptionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhookId** | [**string**] | The webhook ID | defaults to undefined|
| **subscriptionId** | [**string**] | The subscription ID | defaults to undefined|


### Return type

**V2Subscription**

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

# **webhookServiceGetWebhook**
> V2Webhook webhookServiceGetWebhook()

Get a single webhook based on its ID

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //The webhook ID (default to undefined)

const { status, data } = await apiInstance.webhookServiceGetWebhook(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The webhook ID | defaults to undefined|


### Return type

**V2Webhook**

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

# **webhookServiceListSubscriptions**
> V2ListSubscriptionsResponse webhookServiceListSubscriptions()

List subscriptions

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let webhookId: string; //The webhook ID (default to undefined)
let pageSize: number; //The number of results to return per page (default 50, max 100) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.webhookServiceListSubscriptions(
    webhookId,
    pageSize,
    pageToken
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhookId** | [**string**] | The webhook ID | defaults to undefined|
| **pageSize** | [**number**] | The number of results to return per page (default 50, max 100) | (optional) defaults to undefined|
| **pageToken** | [**string**] | The token to retrieve the next page of results | (optional) defaults to undefined|


### Return type

**V2ListSubscriptionsResponse**

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

# **webhookServiceListWebhooks**
> V2ListWebhooksResponse webhookServiceListWebhooks()

List webhooks

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let pageSize: number; //The number of results to return per page (default 50, max 100) (optional) (default to undefined)
let pageToken: string; //The token to retrieve the next page of results (optional) (default to undefined)

const { status, data } = await apiInstance.webhookServiceListWebhooks(
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

**V2ListWebhooksResponse**

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

