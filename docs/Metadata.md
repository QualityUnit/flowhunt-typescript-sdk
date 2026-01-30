# Metadata

Metadata

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **string** | Message ID | [default to undefined]
**message** | **string** | Message | [default to undefined]
**sender** | [**HumanAgentSender**](HumanAgentSender.md) |  | [optional] [default to undefined]
**tool_name** | **string** | Tool name | [default to undefined]
**loading_desc** | **string** | Loading description | [default to undefined]
**icon** | **string** |  | [optional] [default to undefined]
**color** | **string** |  | [optional] [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**feedback_message_id** | **string** | Message ID | [default to undefined]
**feedback** | [**MessageFeedback**](MessageFeedback.md) |  | [optional] [default to undefined]
**agent_query** | **string** | Tool input arguments | [default to undefined]
**tool_response** | **string** | Tool response | [default to undefined]
**task_name** | **string** |  | [default to undefined]
**task_input** | **string** |  | [default to undefined]
**agent** | **string** |  | [default to undefined]
**task_response** | **string** |  | [default to undefined]
**artefacts** | [**Array&lt;FlowSessionArtefactInfo&gt;**](FlowSessionArtefactInfo.md) | List of artefact files created by agent | [default to undefined]
**cot_id** | **string** | Unique CoT identifier for updates | [default to undefined]
**content** | **string** | Chain of thought / reasoning text | [default to undefined]
**todo_id** | **string** | Unique todo list identifier for updates | [default to undefined]
**todos** | [**Array&lt;TodoItem&gt;**](TodoItem.md) | List of todo items | [default to undefined]
**action_description** | **string** |  | [optional] [default to undefined]
**duration_ms** | **number** |  | [optional] [default to undefined]
**stage** | **string** | Initialization stage (e.g., \&#39;starting\&#39;, \&#39;creating_agent\&#39;, \&#39;ready\&#39;) | [default to undefined]
**action_id** | **string** | Action ID | [default to undefined]
**component_id** | **string** | Component ID | [default to undefined]
**component_type** | **string** | Component name | [default to undefined]
**component_display_name** | **string** |  | [optional] [default to undefined]
**component_icon** | **string** |  | [optional] [default to undefined]
**parameter_values** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**source_component_id** | **string** | Source component ID | [default to undefined]
**target_component_id** | **string** | Target component ID | [default to undefined]
**source_field_name** | **string** |  | [optional] [default to undefined]
**target_field_name** | **string** |  | [optional] [default to undefined]
**flow_name** | **string** | Agent name | [default to undefined]
**flow_description** | **string** |  | [optional] [default to undefined]
**flow_id** | **string** | Agent ID | [default to undefined]
**file_id** | **string** | File ID | [default to undefined]
**file_name** | **string** | File name | [default to undefined]
**file_type** | **string** |  | [optional] [default to undefined]
**document_type** | [**DocumentType**](DocumentType.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Metadata } from 'flowhunt';

const instance: Metadata = {
    message_id,
    message,
    sender,
    tool_name,
    loading_desc,
    icon,
    color,
    detailed_description,
    feedback_message_id,
    feedback,
    agent_query,
    tool_response,
    task_name,
    task_input,
    agent,
    task_response,
    artefacts,
    cot_id,
    content,
    todo_id,
    todos,
    action_description,
    duration_ms,
    stage,
    action_id,
    component_id,
    component_type,
    component_display_name,
    component_icon,
    parameter_values,
    source_component_id,
    target_component_id,
    source_field_name,
    target_field_name,
    flow_name,
    flow_description,
    flow_id,
    file_id,
    file_name,
    file_type,
    document_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
