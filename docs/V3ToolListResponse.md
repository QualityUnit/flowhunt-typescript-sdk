# V3ToolListResponse

Response schema for list of tools grouped by category.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tools** | **{ [key: string]: { [key: string]: V3ToolResponse; }; }** | Tools grouped by category: {category: {step_name: tool}} | [optional] [default to undefined]
**count** | **number** | Total number of tools | [default to undefined]

## Example

```typescript
import { V3ToolListResponse } from 'flowhunt';

const instance: V3ToolListResponse = {
    tools,
    count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
