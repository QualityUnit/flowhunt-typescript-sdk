# FlowBatchRunResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**batch_run_id** | **string** |  | [default to undefined]
**flow_id** | **string** |  | [default to undefined]
**workspace_id** | **string** |  | [default to undefined]
**user_id** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [default to undefined]
**columns** | [**Array&lt;FlowBatchColumnDefinition&gt;**](FlowBatchColumnDefinition.md) |  | [optional] [default to undefined]
**max_parallel** | **number** |  | [default to undefined]
**status** | [**FlowBatchRunStatus**](FlowBatchRunStatus.md) |  | [default to undefined]
**total_rows** | **number** |  | [default to undefined]
**completed_rows** | **number** |  | [default to undefined]
**failed_rows** | **number** |  | [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowBatchRunResponse } from 'flowhunt';

const instance: FlowBatchRunResponse = {
    batch_run_id,
    flow_id,
    workspace_id,
    user_id,
    name,
    columns,
    max_parallel,
    status,
    total_rows,
    completed_rows,
    failed_rows,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
