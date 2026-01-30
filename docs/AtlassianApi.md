# AtlassianApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getConfluencePages**](#getconfluencepages) | **GET** /v2/integrations/atlassian/confluence/spaces/{space_key}/pages | Get Confluence Pages|
|[**getConfluenceSpaces**](#getconfluencespaces) | **GET** /v2/integrations/atlassian/confluence/spaces | Get Confluence Spaces|
|[**getJiraAssignees**](#getjiraassignees) | **GET** /v2/integrations/atlassian/jira/projects/{project_key}/assignees | Get Jira Assignees|
|[**getJiraIssues**](#getjiraissues) | **GET** /v2/integrations/atlassian/jira/projects/{project_key}/issues | Get Jira Issues|
|[**getJiraProjects**](#getjiraprojects) | **GET** /v2/integrations/atlassian/jira/projects | Get Jira Projects|
|[**getJiraTransitions**](#getjiratransitions) | **GET** /v2/integrations/atlassian/jira/issues/{issue_key}/transitions | Get Jira Transitions|

# **getConfluencePages**
> ConfluencePagesResponse getConfluencePages()

Get all pages in a Confluence space.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let spaceKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getConfluencePages(
    spaceKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **spaceKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ConfluencePagesResponse**

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

# **getConfluenceSpaces**
> ConfluenceSpacesResponse getConfluenceSpaces()

Get all Confluence spaces accessible through the workspace\'s Atlassian integration.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getConfluenceSpaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ConfluenceSpacesResponse**

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

# **getJiraAssignees**
> JiraAssigneesResponse getJiraAssignees()

Get assignable users for a Jira project.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let projectKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraAssignees(
    projectKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraAssigneesResponse**

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

# **getJiraIssues**
> JiraIssuesResponse getJiraIssues()

Get issues for a Jira project.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let projectKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraIssues(
    projectKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraIssuesResponse**

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

# **getJiraProjects**
> JiraProjectsResponse getJiraProjects()

Get all Jira projects accessible through the workspace\'s Atlassian integration.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraProjects(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraProjectsResponse**

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

# **getJiraTransitions**
> JiraTransitionsResponse getJiraTransitions()

Get available transitions for a Jira issue.

### Example

```typescript
import {
    AtlassianApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AtlassianApi(configuration);

let issueKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraTransitions(
    issueKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **issueKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraTransitionsResponse**

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

