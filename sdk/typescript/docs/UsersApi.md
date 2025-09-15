# UsersApi

All URIs are relative to *https://api.sandbox.palisade.co*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**accountServiceCreateUser**](#accountservicecreateuser) | **POST** /v2/users | Create a user|
|[**accountServiceDeleteUser**](#accountservicedeleteuser) | **DELETE** /v2/users/{id} | Delete users|
|[**accountServiceDeleteUserAuthMethods**](#accountservicedeleteuserauthmethods) | **DELETE** /v2/users/{id}/mfa | Delete authentication methods|
|[**accountServiceGetUser**](#accountservicegetuser) | **GET** /v2/users/{id} | Get user|
|[**accountServiceGetUserInfo**](#accountservicegetuserinfo) | **GET** /v2/users/{id}/info | Get user info|
|[**accountServiceListUserAuthMethods**](#accountservicelistuserauthmethods) | **GET** /v2/users/{id}/mfa | List authentication methods|
|[**accountServiceListUserInfo**](#accountservicelistuserinfo) | **GET** /v2/users/info | List user info|
|[**accountServiceListUsers**](#accountservicelistusers) | **GET** /v2/users | List users|
|[**accountServiceTriggerPasswordReset**](#accountservicetriggerpasswordreset) | **POST** /v2/users/{id}/password | Trigger password reset|
|[**accountServiceUpdateUser**](#accountserviceupdateuser) | **PUT** /v2/users/{id} | Update users|
|[**accountServiceUpdateUserRole**](#accountserviceupdateuserrole) | **PUT** /v2/users/{id}/role | Update user role|
|[**accountServiceUpdateUserStatus**](#accountserviceupdateuserstatus) | **PUT** /v2/users/{id}/status | Update user status|

# **accountServiceCreateUser**
> V2User accountServiceCreateUser(v2CreateUserRequest)

Create a new user

### Example

```typescript
import {
    UsersApi,
    Configuration,
    V2CreateUserRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let v2CreateUserRequest: V2CreateUserRequest; //

const { status, data } = await apiInstance.accountServiceCreateUser(
    v2CreateUserRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **v2CreateUserRequest** | **V2CreateUserRequest**|  | |


### Return type

**V2User**

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

# **accountServiceDeleteUser**
> object accountServiceDeleteUser()

Delete a user

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceDeleteUser(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


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

# **accountServiceDeleteUserAuthMethods**
> object accountServiceDeleteUserAuthMethods()

Delete all authentication methods for a user

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceDeleteUserAuthMethods(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


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

# **accountServiceGetUser**
> V2User accountServiceGetUser()

Get a user

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceGetUser(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**V2User**

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

# **accountServiceGetUserInfo**
> V2UserInfo accountServiceGetUserInfo()

Get a users info

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceGetUserInfo(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**V2UserInfo**

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

# **accountServiceListUserAuthMethods**
> Array<V2UserAuthMethod> accountServiceListUserAuthMethods()

List a users authentication methods

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceListUserAuthMethods(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**Array<V2UserAuthMethod>**

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

# **accountServiceListUserInfo**
> V2ListUserInfoResponse accountServiceListUserInfo()

List user info

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

const { status, data } = await apiInstance.accountServiceListUserInfo();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**V2ListUserInfoResponse**

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

# **accountServiceListUsers**
> V2ListUsersResponse accountServiceListUsers()

List users

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let role: 'ADMINISTRATOR' | 'APPROVER' | 'AUDITOR' | 'OWNER' | 'PROPOSER' | 'VIEWER'; //The role to filter by (optional) (default to undefined)

const { status, data } = await apiInstance.accountServiceListUsers(
    role
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **role** | [**&#39;ADMINISTRATOR&#39; | &#39;APPROVER&#39; | &#39;AUDITOR&#39; | &#39;OWNER&#39; | &#39;PROPOSER&#39; | &#39;VIEWER&#39;**]**Array<&#39;ADMINISTRATOR&#39; &#124; &#39;APPROVER&#39; &#124; &#39;AUDITOR&#39; &#124; &#39;OWNER&#39; &#124; &#39;PROPOSER&#39; &#124; &#39;VIEWER&#39;>** | The role to filter by | (optional) defaults to undefined|


### Return type

**V2ListUsersResponse**

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

# **accountServiceTriggerPasswordReset**
> object accountServiceTriggerPasswordReset()

Triggers a password reset and sends an email to the user

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)

const { status, data } = await apiInstance.accountServiceTriggerPasswordReset(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The user ID | defaults to undefined|


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

# **accountServiceUpdateUser**
> V2User accountServiceUpdateUser(accountServiceUpdateUserRequest)

Update a user

### Example

```typescript
import {
    UsersApi,
    Configuration,
    AccountServiceUpdateUserRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)
let accountServiceUpdateUserRequest: AccountServiceUpdateUserRequest; //

const { status, data } = await apiInstance.accountServiceUpdateUser(
    id,
    accountServiceUpdateUserRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accountServiceUpdateUserRequest** | **AccountServiceUpdateUserRequest**|  | |
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**V2User**

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

# **accountServiceUpdateUserRole**
> V2User accountServiceUpdateUserRole(accountServiceUpdateUserRoleRequest)

Update a users role

### Example

```typescript
import {
    UsersApi,
    Configuration,
    AccountServiceUpdateUserRoleRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)
let accountServiceUpdateUserRoleRequest: AccountServiceUpdateUserRoleRequest; //

const { status, data } = await apiInstance.accountServiceUpdateUserRole(
    id,
    accountServiceUpdateUserRoleRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accountServiceUpdateUserRoleRequest** | **AccountServiceUpdateUserRoleRequest**|  | |
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**V2User**

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

# **accountServiceUpdateUserStatus**
> V2User accountServiceUpdateUserStatus(accountServiceUpdateUserStatusRequest)

Update a users status

### Example

```typescript
import {
    UsersApi,
    Configuration,
    AccountServiceUpdateUserStatusRequest
} from '@palisade-inc/typescript-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: string; //The user ID (default to undefined)
let accountServiceUpdateUserStatusRequest: AccountServiceUpdateUserStatusRequest; //

const { status, data } = await apiInstance.accountServiceUpdateUserStatus(
    id,
    accountServiceUpdateUserStatusRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accountServiceUpdateUserStatusRequest** | **AccountServiceUpdateUserStatusRequest**|  | |
| **id** | [**string**] | The user ID | defaults to undefined|


### Return type

**V2User**

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

