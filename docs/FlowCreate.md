# FlowCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The agent name | [default to undefined]
**description** | **string** | The agent description | [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**config** | [**FlowConfig**](FlowConfig.md) | The agent configuration | [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**engine_version** | [**FlowEngineVersion**](FlowEngineVersion.md) |  | [optional] [default to undefined]
**try_flow_input_placeholder** | **string** |  | [optional] [default to undefined]
**disable_text_input** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowCreate } from 'flowhunt';

const instance: FlowCreate = {
    name,
    description,
    detailed_description,
    config,
    category_id,
    engine_version,
    try_flow_input_placeholder,
    disable_text_input,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
