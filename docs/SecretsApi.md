# SecretsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createSecret**](#createsecret) | **POST** /v2/secrets/create | Create Secret|
|[**deleteSecret**](#deletesecret) | **DELETE** /v2/secrets/{secret_id} | Delete Secret|
|[**getSecret**](#getsecret) | **GET** /v2/secrets/{secret_id} | Get Secret|
|[**searchSecret**](#searchsecret) | **POST** /v2/secrets/search | Search Secret|
|[**updateSecret**](#updatesecret) | **PUT** /v2/secrets/{secret_id} | Update Secret|

# **createSecret**
> SecretResponse createSecret(secretCreateRequest)


### Example

```typescript
import {
    SecretsApi,
    Configuration,
    SecretCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SecretsApi(configuration);

let workspaceId: string; // (default to undefined)
let secretCreateRequest: SecretCreateRequest; //

const { status, data } = await apiInstance.createSecret(
    workspaceId,
    secretCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **secretCreateRequest** | **SecretCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**SecretResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteSecret**
> Completed deleteSecret()


### Example

```typescript
import {
    SecretsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SecretsApi(configuration);

let secretId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteSecret(
    secretId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **secretId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSecret**
> SecretResponse getSecret()


### Example

```typescript
import {
    SecretsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SecretsApi(configuration);

let secretId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSecret(
    secretId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **secretId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**SecretResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchSecret**
> Array<SecretResponse> searchSecret(secretSearchRequest)


### Example

```typescript
import {
    SecretsApi,
    Configuration,
    SecretSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SecretsApi(configuration);

let workspaceId: string; // (default to undefined)
let secretSearchRequest: SecretSearchRequest; //

const { status, data } = await apiInstance.searchSecret(
    workspaceId,
    secretSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **secretSearchRequest** | **SecretSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SecretResponse>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateSecret**
> SecretResponse updateSecret(secretUpdateRequest)


### Example

```typescript
import {
    SecretsApi,
    Configuration,
    SecretUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SecretsApi(configuration);

let secretId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let secretUpdateRequest: SecretUpdateRequest; //

const { status, data } = await apiInstance.updateSecret(
    secretId,
    workspaceId,
    secretUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **secretUpdateRequest** | **SecretUpdateRequest**|  | |
| **secretId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**SecretResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

