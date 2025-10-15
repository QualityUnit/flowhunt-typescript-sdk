# FlowSessionViewResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**session_id** | **string** | Session ID | [default to undefined]
**chatbot_id** | **string** |  | [optional] [default to undefined]
**flow_id** | **string** | Flow ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**created_at** | **string** | Created at | [default to undefined]
**last_msg_at** | **string** |  | [optional] [default to undefined]
**msg_count** | **number** |  | [optional] [default to undefined]
**credits** | **number** |  | [optional] [default to undefined]
**chatbot_name** | **string** |  | [optional] [default to undefined]
**flow_name** | **string** |  | [optional] [default to undefined]
**tags** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**duration** | **number** |  | [optional] [default to undefined]
**ipaddress** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**positive_feedback_count** | **number** |  | [optional] [default to undefined]
**negative_feedback_count** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionViewResponse } from 'flowhunt';

const instance: FlowSessionViewResponse = {
    session_id,
    chatbot_id,
    flow_id,
    workspace_id,
    created_at,
    last_msg_at,
    msg_count,
    credits,
    chatbot_name,
    flow_name,
    tags,
    duration,
    ipaddress,
    url,
    positive_feedback_count,
    negative_feedback_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
