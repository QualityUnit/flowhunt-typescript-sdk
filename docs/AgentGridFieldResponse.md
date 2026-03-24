# AgentGridFieldResponse

Schema for a single field in an agent grid schema.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Field name | [default to undefined]
**field_type** | [**AgentGridFieldType**](AgentGridFieldType.md) | Field type | [default to undefined]
**required** | **boolean** | Whether the field is required | [default to undefined]

## Example

```typescript
import { AgentGridFieldResponse } from 'flowhunt';

const instance: AgentGridFieldResponse = {
    name,
    field_type,
    required,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
