# TotalFeedback


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**positive** | **number** | Total count of positive feedback | [optional] [default to 0]
**negative** | **number** | Total count of negative feedback | [optional] [default to 0]
**session_count** | **number** | Total count of unique sessions (visitor count) | [optional] [default to 0]
**human_message_count** | **number** | Average human messages per session | [optional] [default to 0.0]
**tool_calling_count** | **number** | Average tool calls per session | [optional] [default to 0.0]

## Example

```typescript
import { TotalFeedback } from 'flowhunt';

const instance: TotalFeedback = {
    positive,
    negative,
    session_count,
    human_message_count,
    tool_calling_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
