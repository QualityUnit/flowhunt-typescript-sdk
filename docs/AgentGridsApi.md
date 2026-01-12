# AgentGridsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAgentGrid**](#createagentgrid) | **POST** /v2/agent_grids/ | Create a Flow Table|
|[**deleteAgentGrid**](#deleteagentgrid) | **DELETE** /v2/agent_grids/{agent_grid_id} | Delete a Flow Table|
|[**deleteRow**](#deleterow) | **DELETE** /v2/agent_grids/{agent_grid_id}/rows/{row_id} | Delete a row|
|[**getAgentGrid**](#getagentgrid) | **GET** /v2/agent_grids/{agent_grid_id} | Get a Flow Table|
|[**getAgentGridPreview**](#getagentgridpreview) | **GET** /v2/agent_grids/{agent_grid_id}/preview | Get Flow Table preview|
|[**getImportStatus**](#getimportstatus) | **GET** /v2/agent_grids/{agent_grid_id}/import-status/{import_id} | Get import status|
|[**importCsv**](#importcsv) | **POST** /v2/agent_grids/{agent_grid_id}/import-csv | Import CSV|
|[**insertRow**](#insertrow) | **POST** /v2/agent_grids/{agent_grid_id}/rows | Insert a row|
|[**insertRowsBulk**](#insertrowsbulk) | **POST** /v2/agent_grids/{agent_grid_id}/rows/bulk | Bulk insert rows|
|[**listAgentGrids**](#listagentgrids) | **GET** /v2/agent_grids/ | List all Flow Tables|
|[**searchRows**](#searchrows) | **POST** /v2/agent_grids/{agent_grid_id}/search | Search rows|

# **createAgentGrid**
> AgentGridResponse createAgentGrid(agentGridCreateRequest)

Creates a new Flow Table with the specified schema.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration,
    AgentGridCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let workspaceId: string; // (default to undefined)
let agentGridCreateRequest: AgentGridCreateRequest; //

const { status, data } = await apiInstance.createAgentGrid(
    workspaceId,
    agentGridCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridCreateRequest** | **AgentGridCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteAgentGrid**
> Completed deleteAgentGrid()

Deletes a Flow Table and all its data.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAgentGrid(
    agentGridId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
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

# **deleteRow**
> Completed deleteRow()

Deletes a single row from the Flow Table.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteRow(
    agentGridId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
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

# **getAgentGrid**
> AgentGridResponse getAgentGrid()

Returns details of a specific Flow Table by ID.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAgentGrid(
    agentGridId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridResponse**

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

# **getAgentGridPreview**
> AgentGridPreviewResponse getAgentGridPreview()

Returns the first N rows of a Flow Table.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let limit: number; //Number of rows to return (optional) (default to 50)

const { status, data } = await apiInstance.getAgentGridPreview(
    agentGridId,
    workspaceId,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] | Number of rows to return | (optional) defaults to 50|


### Return type

**AgentGridPreviewResponse**

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

# **getImportStatus**
> AgentGridImportStatusResponse getImportStatus()

Poll for the status of a CSV import. Returns progress, errors, and completion status.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let importId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getImportStatus(
    agentGridId,
    importId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
| **importId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridImportStatusResponse**

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

# **importCsv**
> AgentGridImportStartResponse importCsv()

Start importing rows from a CSV file. The import runs asynchronously. Use the returned import_id to poll for status.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: File; //CSV file to import (default to undefined)

const { status, data } = await apiInstance.importCsv(
    agentGridId,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] | CSV file to import | defaults to undefined|


### Return type

**AgentGridImportStartResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**202** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **insertRow**
> AgentGridRowInsertResponse insertRow(agentGridRowInsertRequest)

Inserts a single row into the Flow Table.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration,
    AgentGridRowInsertRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let agentGridRowInsertRequest: AgentGridRowInsertRequest; //

const { status, data } = await apiInstance.insertRow(
    agentGridId,
    workspaceId,
    agentGridRowInsertRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridRowInsertRequest** | **AgentGridRowInsertRequest**|  | |
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridRowInsertResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **insertRowsBulk**
> AgentGridBulkInsertResponse insertRowsBulk(agentGridRowsBulkInsertRequest)

Inserts multiple rows into the Flow Table.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration,
    AgentGridRowsBulkInsertRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let agentGridRowsBulkInsertRequest: AgentGridRowsBulkInsertRequest; //

const { status, data } = await apiInstance.insertRowsBulk(
    agentGridId,
    workspaceId,
    agentGridRowsBulkInsertRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridRowsBulkInsertRequest** | **AgentGridRowsBulkInsertRequest**|  | |
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridBulkInsertResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listAgentGrids**
> Array<AgentGridResponse> listAgentGrids()

Returns a list of all Flow Tables (Agent Grids) for the workspace.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listAgentGrids(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AgentGridResponse>**

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

# **searchRows**
> AgentGridSearchResponse searchRows(agentGridSearchRequest)

Search rows in the Flow Table using full-text search.

### Example

```typescript
import {
    AgentGridsApi,
    Configuration,
    AgentGridSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AgentGridsApi(configuration);

let agentGridId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let agentGridSearchRequest: AgentGridSearchRequest; //

const { status, data } = await apiInstance.searchRows(
    agentGridId,
    workspaceId,
    agentGridSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **agentGridSearchRequest** | **AgentGridSearchRequest**|  | |
| **agentGridId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AgentGridSearchResponse**

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

