# FlowCronUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**FlowCronStatus**](FlowCronStatus.md) |  | [optional] [default to undefined]
**input_text** | **string** |  | [optional] [default to undefined]
**variables** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**interval_settings** | **string** |  | [optional] [default to undefined]
**cron_name** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowCronUpdateRequest } from 'flowhunt';

const instance: FlowCronUpdateRequest = {
    status,
    input_text,
    variables,
    interval_settings,
    cron_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
