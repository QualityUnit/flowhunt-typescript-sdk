# PerDayFeedback


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date** | **string** | Date in YYYY-MM-DD format | [default to undefined]
**positive** | **number** | Count of positive feedback | [optional] [default to 0]
**negative** | **number** | Count of negative feedback | [optional] [default to 0]
**session_count** | **number** | Count of unique sessions (visitor count) | [optional] [default to 0]
**human_message_count** | **number** | Count of human messages | [optional] [default to 0]
**tool_calling_count** | **number** | Count of tool calls | [optional] [default to undefined]

## Example

```typescript
import { PerDayFeedback } from 'flowhunt';

const instance: PerDayFeedback = {
    date,
    positive,
    negative,
    session_count,
    human_message_count,
    tool_calling_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
