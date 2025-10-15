# OAuthApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**oauthAuthorize**](#oauthauthorize) | **GET** /v2/auth/oauth/authorize | Oauth Authorize|
|[**oauthAuthorizePost**](#oauthauthorizepost) | **POST** /v2/auth/oauth/authorize | Oauth Authorize Post|
|[**oauthCallback**](#oauthcallback) | **GET** /v2/auth/oauth/callback | Oauth Callback|
|[**oauthLogin**](#oauthlogin) | **GET** /v2/auth/oauth/login | Oauth Login|
|[**oauthLoginGithub**](#oauthlogingithub) | **GET** /v2/auth/oauth/login/github | Oauth Login Github|
|[**oauthLoginGoogle**](#oauthlogingoogle) | **GET** /v2/auth/oauth/login/google | Oauth Login Google|
|[**oauthLoginPost**](#oauthloginpost) | **POST** /v2/auth/oauth/login | Oauth Login Post|
|[**oauthLoginShopify**](#oauthloginshopify) | **GET** /v2/auth/oauth/login/shopify | Oauth Login Shopify|
|[**oauthLogout**](#oauthlogout) | **GET** /v2/auth/oauth/logout | Oauth Logout|
|[**oauthRevoke**](#oauthrevoke) | **POST** /v2/auth/oauth/revoke | Oauth Revoke|
|[**oauthToken**](#oauthtoken) | **POST** /v2/auth/oauth/token | Oauth Token|
|[**oauthUserinfo**](#oauthuserinfo) | **GET** /v2/auth/oauth/userinfo | Oauth Userinfo|
|[**samlCallback**](#samlcallback) | **POST** /v2/auth/oauth/callback/saml/{random_id} | Saml Callback|

# **oauthAuthorize**
> any oauthAuthorize()

OAuth authorization endpoint

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthAuthorize();
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

# **oauthAuthorizePost**
> any oauthAuthorizePost()

OAuth authorization endpoint (consent form submission)

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthAuthorizePost();
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

# **oauthCallback**
> any oauthCallback()

OAuth callback endpoint for third-party providers

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthCallback();
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

# **oauthLogin**
> any oauthLogin()

OAuth login page

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLogin();
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

# **oauthLoginGithub**
> any oauthLoginGithub()

OAuth login with GitHub

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLoginGithub();
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

# **oauthLoginGoogle**
> any oauthLoginGoogle()

OAuth login with Google

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLoginGoogle();
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

# **oauthLoginPost**
> any oauthLoginPost()

OAuth login form submission

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLoginPost();
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

# **oauthLoginShopify**
> any oauthLoginShopify()

OAuth login with Shopify for app installation

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLoginShopify();
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

# **oauthLogout**
> any oauthLogout()

OAuth logout endpoint - revokes tokens, clears session and redirects to specified URL

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthLogout();
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

# **oauthRevoke**
> any oauthRevoke()

OAuth token revocation endpoint

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthRevoke();
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

# **oauthToken**
> any oauthToken()

OAuth token endpoint

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthToken();
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

# **oauthUserinfo**
> any oauthUserinfo()

OpenID Connect userinfo endpoint

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

const { status, data } = await apiInstance.oauthUserinfo();
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

# **samlCallback**
> any samlCallback()

SAML callback endpoint (Assertion Consumer Service) Handles the SAML response from the Identity Provider after successful authentication

### Example

```typescript
import {
    OAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new OAuthApi(configuration);

let randomId: string; // (default to undefined)
let workspaceId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.samlCallback(
    randomId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **randomId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | (optional) defaults to undefined|


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

