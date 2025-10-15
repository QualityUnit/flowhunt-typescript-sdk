# WorkspacesSSOApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createWorkspaceSsoSettings**](#createworkspacessosettings) | **POST** /v2/workspaces/{workspace_id}/sso | Create Workspace Sso Settings|
|[**deleteWorkspaceSsoSettings**](#deleteworkspacessosettings) | **DELETE** /v2/workspaces/{workspace_id}/sso/{provider} | Delete Workspace Sso Settings|
|[**getWorkspaceSsoSettings**](#getworkspacessosettings) | **GET** /v2/workspaces/{workspace_id}/sso/{provider} | Get Workspace Sso Settings|
|[**listWorkspaceSsoSettings**](#listworkspacessosettings) | **GET** /v2/workspaces/{workspace_id}/sso | List Workspace Sso Settings|
|[**updateWorkspaceSsoSettings**](#updateworkspacessosettings) | **PUT** /v2/workspaces/{workspace_id}/sso/{provider} | Update Workspace Sso Settings|

# **createWorkspaceSsoSettings**
> WorkspaceSSOResponse createWorkspaceSsoSettings(workspaceSSOCreateRequest)

Create SSO settings for a workspace. Admin endpoint - requires workspace admin permissions.

### Example

```typescript
import {
    WorkspacesSSOApi,
    Configuration,
    WorkspaceSSOCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSOApi(configuration);

let workspaceId: string; // (default to undefined)
let workspaceSSOCreateRequest: WorkspaceSSOCreateRequest; //

const { status, data } = await apiInstance.createWorkspaceSsoSettings(
    workspaceId,
    workspaceSSOCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceSSOCreateRequest** | **WorkspaceSSOCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSOResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteWorkspaceSsoSettings**
> Completed deleteWorkspaceSsoSettings()

Delete SSO settings for a workspace and provider. Admin endpoint - requires workspace admin permissions.

### Example

```typescript
import {
    WorkspacesSSOApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSOApi(configuration);

let workspaceId: string; // (default to undefined)
let provider: string; // (default to undefined)

const { status, data } = await apiInstance.deleteWorkspaceSsoSettings(
    workspaceId,
    provider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **provider** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getWorkspaceSsoSettings**
> WorkspaceSSOResponse getWorkspaceSsoSettings()

Get SSO settings for a specific workspace and provider. Admin endpoint - requires workspace admin permissions.

### Example

```typescript
import {
    WorkspacesSSOApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSOApi(configuration);

let workspaceId: string; // (default to undefined)
let provider: string; // (default to undefined)

const { status, data } = await apiInstance.getWorkspaceSsoSettings(
    workspaceId,
    provider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **provider** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSOResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listWorkspaceSsoSettings**
> WorkspaceSSOListResponse listWorkspaceSsoSettings()

List all SSO settings for a workspace. Admin endpoint - requires workspace admin permissions.

### Example

```typescript
import {
    WorkspacesSSOApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSOApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listWorkspaceSsoSettings(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSOListResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateWorkspaceSsoSettings**
> WorkspaceSSOResponse updateWorkspaceSsoSettings(workspaceSSOUpdateRequest)

Update SSO settings for a workspace and provider. Admin endpoint - requires workspace admin permissions.

### Example

```typescript
import {
    WorkspacesSSOApi,
    Configuration,
    WorkspaceSSOUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSOApi(configuration);

let workspaceId: string; // (default to undefined)
let provider: string; // (default to undefined)
let workspaceSSOUpdateRequest: WorkspaceSSOUpdateRequest; //

const { status, data } = await apiInstance.updateWorkspaceSsoSettings(
    workspaceId,
    provider,
    workspaceSSOUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceSSOUpdateRequest** | **WorkspaceSSOUpdateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|
| **provider** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSOResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

