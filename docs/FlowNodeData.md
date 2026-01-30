# FlowNodeData

Node data structure for flow validation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **string** | Component type (e.g., \&#39;AgentGridSearch\&#39;) | [default to undefined]
**node** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowNodeData } from 'flowhunt';

const instance: FlowNodeData = {
    type,
    node,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
