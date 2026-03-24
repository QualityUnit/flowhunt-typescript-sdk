# FlowSessionEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**session_id** | **string** | Session ID | [default to undefined]
**event_id** | **string** | Event ID | [default to undefined]
**event_type** | [**MessageType**](MessageType.md) | Event type | [default to undefined]
**created_at_timestamp** | **string** | Created at | [default to undefined]
**action_type** | [**FlowEventActionType**](FlowEventActionType.md) | Action type | [default to undefined]
**credits** | **number** | Credits | [default to undefined]
**metadata** | [**Metadata**](Metadata.md) |  | [optional] [default to undefined]
**component_name** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionEvent } from 'flowhunt';

const instance: FlowSessionEvent = {
    workspace_id,
    session_id,
    event_id,
    event_type,
    created_at_timestamp,
    action_type,
    credits,
    metadata,
    component_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
