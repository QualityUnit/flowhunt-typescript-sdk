# FlowCronSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**FlowCronStatus**](FlowCronStatus.md) |  | [optional] [default to undefined]
**next_run_to** | **string** |  | [optional] [default to undefined]
**next_run_from** | **string** |  | [optional] [default to undefined]
**last_run_to** | **string** |  | [optional] [default to undefined]
**last_run_from** | **string** |  | [optional] [default to undefined]
**flow_id** | **string** |  | [optional] [default to undefined]
**cron_name** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowCronSearchRequest } from 'flowhunt';

const instance: FlowCronSearchRequest = {
    status,
    next_run_to,
    next_run_from,
    last_run_to,
    last_run_from,
    flow_id,
    cron_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
