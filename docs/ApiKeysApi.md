# ApiKeysApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createApiKey**](#createapikey) | **POST** /v2/api_keys/create | Create Api Key|
|[**deleteApiKey**](#deleteapikey) | **DELETE** /v2/api_keys/{api_key_id} | Delete Api Key|
|[**searchApiKey**](#searchapikey) | **POST** /v2/api_keys/search | Search Api Key|
|[**updateApiKey**](#updateapikey) | **PUT** /v2/api_keys/{api_key_id} | Update Api Key|

# **createApiKey**
> ApiKeyResponse createApiKey(apiKeyCreateRequest)


### Example

```typescript
import {
    ApiKeysApi,
    Configuration,
    ApiKeyCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let workspaceId: string; // (default to undefined)
let apiKeyCreateRequest: ApiKeyCreateRequest; //

const { status, data } = await apiInstance.createApiKey(
    workspaceId,
    apiKeyCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeyCreateRequest** | **ApiKeyCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ApiKeyResponse**

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

# **deleteApiKey**
> Completed deleteApiKey()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let apiKeyId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteApiKey(
    apiKeyId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeyId** | [**string**] |  | defaults to undefined|
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

# **searchApiKey**
> Array<ApiKeyResponse> searchApiKey(apiKeySearchRequest)


### Example

```typescript
import {
    ApiKeysApi,
    Configuration,
    ApiKeySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let workspaceId: string; // (default to undefined)
let apiKeySearchRequest: ApiKeySearchRequest; //

const { status, data } = await apiInstance.searchApiKey(
    workspaceId,
    apiKeySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeySearchRequest** | **ApiKeySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ApiKeyResponse>**

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

# **updateApiKey**
> ApiKeyResponse updateApiKey(apiKeyUpdateRequest)


### Example

```typescript
import {
    ApiKeysApi,
    Configuration,
    ApiKeyUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let apiKeyId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let apiKeyUpdateRequest: ApiKeyUpdateRequest; //

const { status, data } = await apiInstance.updateApiKey(
    apiKeyId,
    workspaceId,
    apiKeyUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeyUpdateRequest** | **ApiKeyUpdateRequest**|  | |
| **apiKeyId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ApiKeyResponse**

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

