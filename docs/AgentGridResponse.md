# AgentGridResponse

Schema for an agent grid (Flow Table) response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**agent_grid_id** | **string** | Agent Grid ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**name** | **string** | Name of the Flow Table | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**schema_fields** | [**Array&lt;AgentGridFieldResponse&gt;**](AgentGridFieldResponse.md) | List of fields defining the table schema | [default to undefined]
**semantic_search_enabled** | **boolean** | Whether semantic search is enabled | [default to undefined]
**row_count** | **number** | Number of rows in the table | [default to undefined]
**created_at** | **string** | Creation timestamp | [default to undefined]
**updated_at** | **string** | Last update timestamp | [default to undefined]

## Example

```typescript
import { AgentGridResponse } from 'flowhunt';

const instance: AgentGridResponse = {
    agent_grid_id,
    workspace_id,
    name,
    description,
    schema_fields,
    semantic_search_enabled,
    row_count,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
