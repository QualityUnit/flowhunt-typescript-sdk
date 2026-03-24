# FlowSessionTodoListMetadata

Metadata for agent todo list updates.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**todo_id** | **string** | Unique todo list identifier for updates | [default to undefined]
**todos** | [**Array&lt;TodoItem&gt;**](TodoItem.md) | List of todo items | [default to undefined]

## Example

```typescript
import { FlowSessionTodoListMetadata } from 'flowhunt';

const instance: FlowSessionTodoListMetadata = {
    todo_id,
    todos,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
