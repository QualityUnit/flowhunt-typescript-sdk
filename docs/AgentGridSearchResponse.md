# AgentGridSearchResponse

Schema for agent grid search response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rows** | **Array&lt;{ [key: string]: any; }&gt;** | Search result rows | [default to undefined]
**total_count** | **number** | Total number of matching rows | [default to undefined]

## Example

```typescript
import { AgentGridSearchResponse } from 'flowhunt';

const instance: AgentGridSearchResponse = {
    rows,
    total_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
