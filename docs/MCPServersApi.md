# MCPServersApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMcpServer**](#createmcpserver) | **POST** /v2/mcp_servers/create | Create Mcp Server|
|[**deleteMcpServer**](#deletemcpserver) | **DELETE** /v2/mcp_servers/{mcp_server_id} | Delete Mcp Server|
|[**getAllMcpSubservers**](#getallmcpsubservers) | **GET** /v2/mcp_servers/all | Get All Mcp Subservers|
|[**getMcpServer**](#getmcpserver) | **GET** /v2/mcp_servers/{mcp_server_id} | Get Mcp Server|
|[**searchMcpServers**](#searchmcpservers) | **POST** /v2/mcp_servers/ | Search Mcp Servers|
|[**updateMcpServer**](#updatemcpserver) | **PUT** /v2/mcp_servers/{mcp_server_id} | Update Mcp Server|

# **createMcpServer**
> MCPServerResponse createMcpServer(mCPServerCreateRequest)

Create a new MCP server.  Args:     main_request: The main request object for rate limiting.     workspace_id: The workspace ID.     request: The MCP server creation request.     user: The authenticated user.     controller: The MCP server controller.  Returns:     MCPServerCreateResponse: The created MCP server with the raw API key.

### Example

```typescript
import {
    MCPServersApi,
    Configuration,
    MCPServerCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

let workspaceId: string; // (default to undefined)
let mCPServerCreateRequest: MCPServerCreateRequest; //

const { status, data } = await apiInstance.createMcpServer(
    workspaceId,
    mCPServerCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mCPServerCreateRequest** | **MCPServerCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MCPServerResponse**

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

# **deleteMcpServer**
> Completed deleteMcpServer()

Delete an MCP server.  Args:     main_request: The main request object for rate limiting.     workspace_id: The workspace ID.     mcp_server_id: The MCP server ID.     user: The authenticated user.     controller: The MCP server controller.

### Example

```typescript
import {
    MCPServersApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

let mcpServerId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteMcpServer(
    mcpServerId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mcpServerId** | [**string**] |  | defaults to undefined|
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

# **getAllMcpSubservers**
> Array<GeneralMCPSubserverResponse> getAllMcpSubservers()

Get all MCP subservers available in the system.  Args:     user: The authenticated user.     controller: The MCP server controller.  Returns:     List[MCPSubServerBinding]: List of all MCP subservers.

### Example

```typescript
import {
    MCPServersApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

const { status, data } = await apiInstance.getAllMcpSubservers();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<GeneralMCPSubserverResponse>**

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

# **getMcpServer**
> MCPServerResponse getMcpServer()

Get an MCP server by ID.  Args:     workspace_id: The workspace ID.     mcp_server_id: The MCP server ID.     user: The authenticated user.     controller: The MCP server controller.  Returns:     MCPServerResponse: The MCP server.

### Example

```typescript
import {
    MCPServersApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

let mcpServerId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getMcpServer(
    mcpServerId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mcpServerId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MCPServerResponse**

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

# **searchMcpServers**
> Array<MCPServerResponse> searchMcpServers(mCPServerSearchRequest)

List MCP servers in a workspace.  Args:     workspace_id: The workspace ID.     user: The authenticated user.     controller: The MCP server controller.  Returns:     List[MCPServerResponse]: List of MCP servers.

### Example

```typescript
import {
    MCPServersApi,
    Configuration,
    MCPServerSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

let workspaceId: string; // (default to undefined)
let mCPServerSearchRequest: MCPServerSearchRequest; //

const { status, data } = await apiInstance.searchMcpServers(
    workspaceId,
    mCPServerSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mCPServerSearchRequest** | **MCPServerSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<MCPServerResponse>**

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

# **updateMcpServer**
> MCPServerResponse updateMcpServer(mCPServerCreateRequest)

Update an MCP server.  Args:     main_request: The main request object for rate limiting.     workspace_id: The workspace ID.     mcp_server_id: The MCP server ID.     request: The update request.     user: The authenticated user.     controller: The MCP server controller.  Returns:     MCPServerResponse: The updated MCP server.

### Example

```typescript
import {
    MCPServersApi,
    Configuration,
    MCPServerCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MCPServersApi(configuration);

let mcpServerId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let mCPServerCreateRequest: MCPServerCreateRequest; //

const { status, data } = await apiInstance.updateMcpServer(
    mcpServerId,
    workspaceId,
    mCPServerCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mCPServerCreateRequest** | **MCPServerCreateRequest**|  | |
| **mcpServerId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MCPServerResponse**

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

