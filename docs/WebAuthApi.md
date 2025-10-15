# WebAuthApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**activateAccount**](#activateaccount) | **GET** /v2/auth/activate | Activate Account|
|[**getUser**](#getuser) | **GET** /v2/auth/me | Get User|
|[**passwordRecoveryPage**](#passwordrecoverypage) | **GET** /v2/auth/recover-password | Password Recovery Page|
|[**passwordRecoverySubmit**](#passwordrecoverysubmit) | **POST** /v2/auth/recover-password | Password Recovery Submit|
|[**registerPage**](#registerpage) | **GET** /v2/auth/register | Register Page|
|[**registerSubmit**](#registersubmit) | **POST** /v2/auth/register | Register Submit|
|[**resetPasswordPage**](#resetpasswordpage) | **GET** /v2/auth/reset-password | Reset Password Page|
|[**resetPasswordSubmit**](#resetpasswordsubmit) | **POST** /v2/auth/reset-password | Reset Password Submit|
|[**ssoLoginPage**](#ssologinpage) | **GET** /v2/auth/oauth/sso | Sso Login Page|
|[**ssoLoginSubmit**](#ssologinsubmit) | **POST** /v2/auth/oauth/sso | Sso Login Submit|

# **activateAccount**
> any activateAccount()

Activate user account

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let token: string; // (default to undefined)

const { status, data } = await apiInstance.activateAccount(
    token
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUser**
> UserResponse getUser()

Get current authenticated user details.  This endpoint returns the current user\'s details including their product plans and API key workspace information. It follows DDD principles by delegating the business logic to the application service layer.  Args:     user: The current authenticated user (injected by dependency)     request: The HTTP request object     user_service: The user application service (injected by dependency)  Returns:     UserResponse: The user details response

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

const { status, data } = await apiInstance.getUser();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **passwordRecoveryPage**
> any passwordRecoveryPage()

Password recovery page

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

const { status, data } = await apiInstance.passwordRecoveryPage();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **passwordRecoverySubmit**
> any passwordRecoverySubmit()

Handle password recovery form submission

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let email: string; // (default to undefined)

const { status, data } = await apiInstance.passwordRecoverySubmit(
    email
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **email** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registerPage**
> any registerPage()

Registration page

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let next: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.registerPage(
    next
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **next** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registerSubmit**
> any registerSubmit()

Handle registration form submission

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let name: string; // (default to undefined)
let email: string; // (default to undefined)
let password: string; // (default to undefined)
let next: string; // (optional) (default to '/')

const { status, data } = await apiInstance.registerSubmit(
    name,
    email,
    password,
    next
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] |  | defaults to undefined|
| **email** | [**string**] |  | defaults to undefined|
| **password** | [**string**] |  | defaults to undefined|
| **next** | [**string**] |  | (optional) defaults to '/'|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetPasswordPage**
> any resetPasswordPage()

Reset password page

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let token: string; // (default to undefined)

const { status, data } = await apiInstance.resetPasswordPage(
    token
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetPasswordSubmit**
> any resetPasswordSubmit()

Handle reset password form submission

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let token: string; // (default to undefined)
let password: string; // (default to undefined)
let confirmPassword: string; // (default to undefined)

const { status, data } = await apiInstance.resetPasswordSubmit(
    token,
    password,
    confirmPassword
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] |  | defaults to undefined|
| **password** | [**string**] |  | defaults to undefined|
| **confirmPassword** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ssoLoginPage**
> any ssoLoginPage()

SSO login page

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let next: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.ssoLoginPage(
    next
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **next** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ssoLoginSubmit**
> any ssoLoginSubmit()

Handle SSO login form submission

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

let email: string; // (default to undefined)
let next: string; // (optional) (default to '/')

const { status, data } = await apiInstance.ssoLoginSubmit(
    email,
    next
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **email** | [**string**] |  | defaults to undefined|
| **next** | [**string**] |  | (optional) defaults to '/'|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

