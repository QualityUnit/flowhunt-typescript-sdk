# AgentGridSearchRequest

Schema for searching rows in an agent grid.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **string** |  | [optional] [default to undefined]
**filters** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**limit** | **number** | Maximum number of rows to return | [optional] [default to 50]
**offset** | **number** | Number of rows to skip | [optional] [default to 0]

## Example

```typescript
import { AgentGridSearchRequest } from 'flowhunt';

const instance: AgentGridSearchRequest = {
    query,
    filters,
    limit,
    offset,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
