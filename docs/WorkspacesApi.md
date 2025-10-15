# WorkspacesApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addWorkspaceUser**](#addworkspaceuser) | **POST** /v2/workspaces/{workspace_id}/add-member | Add Workspace User|
|[**createWorkspace**](#createworkspace) | **POST** /v2/workspaces/create | Create Workspace|
|[**deleteWorkspace**](#deleteworkspace) | **DELETE** /v2/workspaces/{workspace_id} | Delete Workspace|
|[**deleteWorkspaceUser**](#deleteworkspaceuser) | **DELETE** /v2/workspaces/{workspace_id}/{user_id} | Delete Workspace User|
|[**getWorkspace**](#getworkspace) | **POST** /v2/workspaces/{workspace_id} | Get Workspace|
|[**searchMyWorkspaces**](#searchmyworkspaces) | **POST** /v2/workspaces/me/my_workspaces | Search My Workspaces|
|[**searchWorkspaceUsers**](#searchworkspaceusers) | **POST** /v2/workspaces/{workspace_id}/users | Search Workspace Users|
|[**updateWorkspace**](#updateworkspace) | **PUT** /v2/workspaces/{workspace_id} | Update Workspace|
|[**updateWorkspaceUser**](#updateworkspaceuser) | **PUT** /v2/workspaces/{workspace_id}/{user_id} | Update Workspace User|

# **addWorkspaceUser**
> Completed addWorkspaceUser(workspaceUserCreateRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceUserCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)
let workspaceUserCreateRequest: WorkspaceUserCreateRequest; //

const { status, data } = await apiInstance.addWorkspaceUser(
    workspaceId,
    workspaceUserCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceUserCreateRequest** | **WorkspaceUserCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **createWorkspace**
> WorkspaceResponse createWorkspace(workspaceCreateRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceCreateRequest: WorkspaceCreateRequest; //

const { status, data } = await apiInstance.createWorkspace(
    workspaceCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceCreateRequest** | **WorkspaceCreateRequest**|  | |


### Return type

**WorkspaceResponse**

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

# **deleteWorkspace**
> Completed deleteWorkspace()


### Example

```typescript
import {
    WorkspacesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteWorkspace(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


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

# **deleteWorkspaceUser**
> Completed deleteWorkspaceUser()


### Example

```typescript
import {
    WorkspacesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)
let userId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteWorkspaceUser(
    workspaceId,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **userId** | [**string**] |  | defaults to undefined|


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

# **getWorkspace**
> WorkspaceResponse getWorkspace()


### Example

```typescript
import {
    WorkspacesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWorkspace(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceResponse**

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

# **searchMyWorkspaces**
> Array<WorkspaceRole> searchMyWorkspaces(workspaceSearchRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceSearchRequest: WorkspaceSearchRequest; //

const { status, data } = await apiInstance.searchMyWorkspaces(
    workspaceSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceSearchRequest** | **WorkspaceSearchRequest**|  | |


### Return type

**Array<WorkspaceRole>**

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

# **searchWorkspaceUsers**
> Array<WorkspaceUserResponse> searchWorkspaceUsers(workspaceUsersSearchRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceUsersSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)
let workspaceUsersSearchRequest: WorkspaceUsersSearchRequest; //

const { status, data } = await apiInstance.searchWorkspaceUsers(
    workspaceId,
    workspaceUsersSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceUsersSearchRequest** | **WorkspaceUsersSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WorkspaceUserResponse>**

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

# **updateWorkspace**
> Completed updateWorkspace(workspaceUpdateRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)
let workspaceUpdateRequest: WorkspaceUpdateRequest; //

const { status, data } = await apiInstance.updateWorkspace(
    workspaceId,
    workspaceUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceUpdateRequest** | **WorkspaceUpdateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **updateWorkspaceUser**
> Completed updateWorkspaceUser(workspaceUserUpdateRequest)


### Example

```typescript
import {
    WorkspacesApi,
    Configuration,
    WorkspaceUserUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesApi(configuration);

let workspaceId: string; // (default to undefined)
let userId: string; // (default to undefined)
let workspaceUserUpdateRequest: WorkspaceUserUpdateRequest; //

const { status, data } = await apiInstance.updateWorkspaceUser(
    workspaceId,
    userId,
    workspaceUserUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceUserUpdateRequest** | **WorkspaceUserUpdateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|
| **userId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

