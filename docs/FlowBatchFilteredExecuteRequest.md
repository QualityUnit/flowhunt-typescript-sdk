# FlowBatchFilteredExecuteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rerun_all** | **boolean** | If True, reset matching completed/failed rows to pending before running | [optional] [default to false]
**max_concurrency** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowBatchFilteredExecuteRequest } from 'flowhunt';

const instance: FlowBatchFilteredExecuteRequest = {
    rerun_all,
    max_concurrency,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
