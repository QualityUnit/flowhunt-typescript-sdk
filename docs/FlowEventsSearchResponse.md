# FlowEventsSearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **string** | Session ID | [default to undefined]
**event_id** | **string** | Event ID | [default to undefined]
**event_type** | [**MessageType**](MessageType.md) | Event type | [default to undefined]
**action_type** | [**FlowEventActionType**](FlowEventActionType.md) | Action type | [default to undefined]
**date** | **string** |  | [optional] [default to undefined]
**message_id** | **string** |  | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowEventsSearchResponse } from 'flowhunt';

const instance: FlowEventsSearchResponse = {
    session_id,
    event_id,
    event_type,
    action_type,
    date,
    message_id,
    message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
