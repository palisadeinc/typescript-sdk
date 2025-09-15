# OrganizationsApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**accountServiceDeleteOrganizationAuthMethod**](#accountservicedeleteorganizationauthmethod) | **DELETE** /v2/organizations/auth-methods/{id} | Delete an authentication method|
|[**accountServiceGenerateSelfServiceSSOTicket**](#accountservicegenerateselfservicessoticket) | **POST** /v2/organizations/self-service-sso-ticket | Generate a self service SSO ticket|
|[**accountServiceGetOrganization**](#accountservicegetorganization) | **GET** /v2/organizations | Get organization|
|[**accountServiceGetOrganizationAuthMethod**](#accountservicegetorganizationauthmethod) | **GET** /v2/organizations/auth-methods/{id} | Get an authentication method|
|[**accountServiceListOrganizationAuthMethods**](#accountservicelistorganizationauthmethods) | **GET** /v2/organizations/auth-methods | List authentication methods|
|[**accountServiceSetDefaultOrganizationAuthMethod**](#accountservicesetdefaultorganizationauthmethod) | **PUT** /v2/organizations/auth-methods/{id}/default | Set default authentication method|
|[**accountServiceUpdateOrganizationAuthMethodIdpSettings**](#accountserviceupdateorganizationauthmethodidpsettings) | **PUT** /v2/organizations/auth-methods/{id}/idp | Update authentication method IDP settings|

# **accountServiceDeleteOrganizationAuthMethod**
> object accountServiceDeleteOrganizationAuthMethod()

Delete a specific organization authentication method

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

let id: string; //The auth method ID (default to undefined)

const { status, data } = await apiInstance.accountServiceDeleteOrganizationAuthMethod(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The auth method ID | defaults to undefined|


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

# **accountServiceGenerateSelfServiceSSOTicket**
> V2GenerateSelfServiceSSOTicketResponse accountServiceGenerateSelfServiceSSOTicket()

Generate a self service ticket to setup SSO

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

const { status, data } = await apiInstance.accountServiceGenerateSelfServiceSSOTicket();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2GenerateSelfServiceSSOTicketResponse**

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

# **accountServiceGetOrganization**
> Accountv2Organization accountServiceGetOrganization()

Get an organization

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

const { status, data } = await apiInstance.accountServiceGetOrganization();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Accountv2Organization**

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

# **accountServiceGetOrganizationAuthMethod**
> V2OrganizationAuthMethod accountServiceGetOrganizationAuthMethod()

Get a specific organization authentication method

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

let id: string; //The auth method ID (default to undefined)

const { status, data } = await apiInstance.accountServiceGetOrganizationAuthMethod(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The auth method ID | defaults to undefined|


### Return type

**V2OrganizationAuthMethod**

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

# **accountServiceListOrganizationAuthMethods**
> Array<V2OrganizationAuthMethod> accountServiceListOrganizationAuthMethods()

List an organizations authentication methods

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

const { status, data } = await apiInstance.accountServiceListOrganizationAuthMethods();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<V2OrganizationAuthMethod>**

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

# **accountServiceSetDefaultOrganizationAuthMethod**
> V2OrganizationAuthMethod accountServiceSetDefaultOrganizationAuthMethod()

Set the default authentication method for an organization

### Example

```typescript
import {
    OrganizationsApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

let id: string; //The auth method ID (default to undefined)

const { status, data } = await apiInstance.accountServiceSetDefaultOrganizationAuthMethod(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The auth method ID | defaults to undefined|


### Return type

**V2OrganizationAuthMethod**

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

# **accountServiceUpdateOrganizationAuthMethodIdpSettings**
> V2OrganizationAuthMethodIdpSettings accountServiceUpdateOrganizationAuthMethodIdpSettings(v2OrganizationAuthMethodIdpSettings)

Update the IDP settings for an authentication method

### Example

```typescript
import {
    OrganizationsApi,
    Configuration,
    V2OrganizationAuthMethodIdpSettings
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new OrganizationsApi(configuration);

let id: string; //The auth method ID (default to undefined)
let v2OrganizationAuthMethodIdpSettings: V2OrganizationAuthMethodIdpSettings; //

const { status, data } = await apiInstance.accountServiceUpdateOrganizationAuthMethodIdpSettings(
    id,
    v2OrganizationAuthMethodIdpSettings
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2OrganizationAuthMethodIdpSettings** | **V2OrganizationAuthMethodIdpSettings**|  | |
| **id** | [**string**] | The auth method ID | defaults to undefined|


### Return type

**V2OrganizationAuthMethodIdpSettings**

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

