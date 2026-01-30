# FlowSessionV3ToolCallStartMetadata

Metadata for V3 tool call start events.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tool_name** | **string** | Tool name | [default to undefined]
**agent_query** | **string** | Tool input arguments | [default to undefined]
**action_description** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionV3ToolCallStartMetadata } from 'flowhunt';

const instance: FlowSessionV3ToolCallStartMetadata = {
    tool_name,
    agent_query,
    action_description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
