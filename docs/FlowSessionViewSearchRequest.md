# FlowSessionViewSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**chatbot_id** | **string** |  | [optional] [default to undefined]
**flow_id** | **string** |  | [optional] [default to undefined]
**tags** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**created_at_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**last_message_at_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**duration_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**msg_count_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**credits_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**chatbot_name** | **string** |  | [optional] [default to undefined]
**flow_name** | **string** |  | [optional] [default to undefined]
**ipaddress_filter** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]
**positive_feedback** | **number** |  | [optional] [default to undefined]
**negative_feedback** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionViewSearchRequest } from 'flowhunt';

const instance: FlowSessionViewSearchRequest = {
    chatbot_id,
    flow_id,
    tags,
    limit,
    created_at_filter,
    last_message_at_filter,
    duration_filter,
    msg_count_filter,
    credits_filter,
    chatbot_name,
    flow_name,
    ipaddress_filter,
    pagination,
    positive_feedback,
    negative_feedback,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
