# AgentGridFieldRequest

Schema for a single field in an agent grid schema.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Field name (must be snake_case: lowercase letters, numbers, underscores only) | [default to undefined]
**field_type** | [**AgentGridFieldType**](AgentGridFieldType.md) | Field type | [default to undefined]
**required** | **boolean** | Whether the field is required | [optional] [default to false]

## Example

```typescript
import { AgentGridFieldRequest } from 'flowhunt';

const instance: AgentGridFieldRequest = {
    name,
    field_type,
    required,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
