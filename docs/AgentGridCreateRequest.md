# AgentGridCreateRequest

Schema for creating a new agent grid (Flow Table).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the Agent Grid (must be snake_case: lowercase letters, numbers, underscores only) | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**schema_fields** | [**Array&lt;AgentGridFieldRequest&gt;**](AgentGridFieldRequest.md) | List of fields defining the table schema | [default to undefined]
**semantic_search_enabled** | **boolean** | Whether semantic search is enabled (not yet available) | [optional] [default to false]

## Example

```typescript
import { AgentGridCreateRequest } from 'flowhunt';

const instance: AgentGridCreateRequest = {
    name,
    description,
    schema_fields,
    semantic_search_enabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
