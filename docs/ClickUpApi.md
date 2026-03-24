# ClickUpApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getClickupSpaces**](#getclickupspaces) | **GET** /v2/integrations/clickup/{integration_id}/spaces | Get Clickup Spaces|
|[**getClickupWorkspaces**](#getclickupworkspaces) | **GET** /v2/integrations/clickup/ | Get Clickup Workspaces|

# **getClickupSpaces**
> Array<ClickUpSpaceResponse> getClickupSpaces()


### Example

```typescript
import {
    ClickUpApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ClickUpApi(configuration);

let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getClickupSpaces(
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ClickUpSpaceResponse>**

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

# **getClickupWorkspaces**
> Array<ClickUpWorkspaceResponse> getClickupWorkspaces()


### Example

```typescript
import {
    ClickUpApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ClickUpApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getClickupWorkspaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ClickUpWorkspaceResponse>**

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

