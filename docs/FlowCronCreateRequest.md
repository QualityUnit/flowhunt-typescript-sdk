# FlowCronCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**flow_id** | **string** |  | [default to undefined]
**status** | [**FlowCronStatus**](FlowCronStatus.md) |  | [default to undefined]
**input_text** | **string** |  | [optional] [default to undefined]
**variables** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**interval_settings** | **string** |  | [default to undefined]
**cron_name** | **string** |  | [default to undefined]

## Example

```typescript
import { FlowCronCreateRequest } from 'flowhunt';

const instance: FlowCronCreateRequest = {
    flow_id,
    status,
    input_text,
    variables,
    interval_settings,
    cron_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
