# V3ToolResponse

Response schema for a single tool.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**step_name** | **string** | Internal step name (e.g., \&#39;Separator\&#39;) | [default to undefined]
**tool_name** | **string** | Tool name for AI agents (e.g., \&#39;split_text\&#39;) | [default to undefined]
**tool_description** | **string** | Tool description for AI agents | [default to undefined]
**display_name** | **string** | Display name for UI | [default to undefined]
**category** | **string** | Tool category (e.g., \&#39;data_processing\&#39;, \&#39;airtable\&#39;) | [default to undefined]
**icon** | **string** | Icon identifier | [default to undefined]
**beta** | **boolean** | Whether this tool is in beta | [optional] [default to false]
**available_plans** | **Array&lt;string&gt;** | List of subscription plans this tool is available on | [optional] [default to undefined]
**is_hitl** | **boolean** | Whether this tool requires human-in-the-loop approval | [optional] [default to false]
**parameters** | [**Array&lt;V3ToolParameterResponse&gt;**](V3ToolParameterResponse.md) | Tool parameters | [optional] [default to undefined]
**exclusive_groups** | [**{ [key: string]: V3ExclusiveGroupResponse; }**](V3ExclusiveGroupResponse.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V3ToolResponse } from 'flowhunt';

const instance: V3ToolResponse = {
    step_name,
    tool_name,
    tool_description,
    display_name,
    category,
    icon,
    beta,
    available_plans,
    is_hitl,
    parameters,
    exclusive_groups,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
