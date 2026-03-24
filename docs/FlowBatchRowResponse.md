# FlowBatchRowResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**row_id** | **string** |  | [default to undefined]
**batch_run_id** | **string** |  | [default to undefined]
**row_index** | **number** |  | [default to undefined]
**input_data** | **{ [key: string]: any; }** |  | [default to undefined]
**status** | [**FlowBatchRowStatus**](FlowBatchRowStatus.md) |  | [default to undefined]
**output** | **string** |  | [optional] [default to undefined]
**output_artefacts** | [**Array&lt;FlowBatchArtefactInfo&gt;**](FlowBatchArtefactInfo.md) |  | [optional] [default to undefined]
**error** | **string** |  | [optional] [default to undefined]
**session_id** | **string** |  | [optional] [default to undefined]
**credits_used** | **number** |  | [optional] [default to undefined]
**started_at** | **string** |  | [optional] [default to undefined]
**completed_at** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowBatchRowResponse } from 'flowhunt';

const instance: FlowBatchRowResponse = {
    row_id,
    batch_run_id,
    row_index,
    input_data,
    status,
    output,
    output_artefacts,
    error,
    session_id,
    credits_used,
    started_at,
    completed_at,
    created_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
