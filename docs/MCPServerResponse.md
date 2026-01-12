# MCPServerResponse

Response schema for MCP server

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**mcp_server_id** | **string** | MCP Server ID | [default to undefined]
**name** | **string** | Name of the MCP server | [default to undefined]
**server_configuration** | [**Array&lt;MCPSubServerBinding&gt;**](MCPSubServerBinding.md) | List of subserver bindings for the MCP server configuration | [default to undefined]
**is_active** | **boolean** | Whether the MCP server is active | [default to undefined]
**created_at** | **string** | Creation timestamp | [default to undefined]
**updated_at** | **string** | Last update timestamp | [default to undefined]
**remote_mcp_url** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { MCPServerResponse } from 'flowhunt';

const instance: MCPServerResponse = {
    workspace_id,
    mcp_server_id,
    name,
    server_configuration,
    is_active,
    created_at,
    updated_at,
    remote_mcp_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
