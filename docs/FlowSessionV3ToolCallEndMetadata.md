# FlowSessionV3ToolCallEndMetadata

Metadata for V3 tool call end events.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tool_name** | **string** | Tool name | [default to undefined]
**agent_query** | **string** | Tool input arguments | [default to undefined]
**tool_response** | **string** | Tool response | [default to undefined]
**duration_ms** | **number** |  | [optional] [default to undefined]
**action_description** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionV3ToolCallEndMetadata } from 'flowhunt';

const instance: FlowSessionV3ToolCallEndMetadata = {
    tool_name,
    agent_query,
    tool_response,
    duration_ms,
    action_description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
