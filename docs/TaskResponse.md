# TaskResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Task ID | [default to undefined]
**status** | [**TaskStatus**](TaskStatus.md) | Task status | [default to undefined]
**result** | **string** |  | [optional] [default to undefined]
**error_message** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { TaskResponse } from 'flowhunt';

const instance: TaskResponse = {
    id,
    status,
    result,
    error_message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
