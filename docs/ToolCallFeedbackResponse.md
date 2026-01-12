# ToolCallFeedbackResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date** | **string** | Date in YYYY-MM-DD format | [default to undefined]
**tool_calling_count** | **number** | Tool call count | [optional] [default to 0]
**tools** | [**Array&lt;ToolFeedback&gt;**](ToolFeedback.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ToolCallFeedbackResponse } from 'flowhunt';

const instance: ToolCallFeedbackResponse = {
    date,
    tool_calling_count,
    tools,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
