# GitLabApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getBranches**](#getbranches) | **GET** /v2/integrations/gitlab/branches | Get Branches|
|[**getProjects**](#getprojects) | **GET** /v2/integrations/gitlab/projects | Get Projects|

# **getBranches**
> GitLabBranchesResponse getBranches()


### Example

```typescript
import {
    GitLabApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GitLabApi(configuration);

let workspaceId: string; // (default to undefined)
let projectId: string; // (default to undefined)

const { status, data } = await apiInstance.getBranches(
    workspaceId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **projectId** | [**string**] |  | defaults to undefined|


### Return type

**GitLabBranchesResponse**

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

# **getProjects**
> GitLabProjectsResponse getProjects()


### Example

```typescript
import {
    GitLabApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GitLabApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getProjects(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GitLabProjectsResponse**

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

