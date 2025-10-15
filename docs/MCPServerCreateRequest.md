# MCPServerCreateRequest

Request schema for creating a new MCP server

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the MCP server | [default to undefined]
**is_active** | **boolean** | Whether the MCP server is active | [optional] [default to true]
**server_configuration** | [**Array&lt;MCPSubServerBinding&gt;**](MCPSubServerBinding.md) | List of subserver bindings for the MCP server configuration | [default to undefined]

## Example

```typescript
import { MCPServerCreateRequest } from 'flowhunt';

const instance: MCPServerCreateRequest = {
    name,
    is_active,
    server_configuration,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
