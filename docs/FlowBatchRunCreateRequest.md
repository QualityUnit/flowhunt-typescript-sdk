# FlowBatchRunCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Batch run name | [default to undefined]
**columns** | [**Array&lt;FlowBatchColumnDefinition&gt;**](FlowBatchColumnDefinition.md) |  | [optional] [default to undefined]
**max_parallel** | **number** | Max concurrent row executions | [optional] [default to 10]

## Example

```typescript
import { FlowBatchRunCreateRequest } from 'flowhunt';

const instance: FlowBatchRunCreateRequest = {
    name,
    columns,
    max_parallel,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
