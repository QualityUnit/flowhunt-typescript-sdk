# FlowCronResponse

Agent cron response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**flow_id** | **string** |  | [default to undefined]
**cron_id** | **string** |  | [default to undefined]
**last_run** | **string** |  | [optional] [default to undefined]
**next_run** | **string** |  | [optional] [default to undefined]
**status** | [**FlowCronStatus**](FlowCronStatus.md) |  | [default to undefined]
**input_text** | **string** |  | [optional] [default to undefined]
**interval_settings** | **string** |  | [default to undefined]
**variables** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**cron_name** | **string** |  | [default to undefined]

## Example

```typescript
import { FlowCronResponse } from 'flowhunt';

const instance: FlowCronResponse = {
    flow_id,
    cron_id,
    last_run,
    next_run,
    status,
    input_text,
    interval_settings,
    variables,
    cron_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
