# AgentGridPreviewResponse

Schema for agent grid preview response (first N rows).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rows** | **Array&lt;{ [key: string]: any; }&gt;** | Preview rows | [default to undefined]
**total_count** | **number** | Total number of rows in the table | [default to undefined]

## Example

```typescript
import { AgentGridPreviewResponse } from 'flowhunt';

const instance: AgentGridPreviewResponse = {
    rows,
    total_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
