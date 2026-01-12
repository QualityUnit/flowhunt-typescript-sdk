# FlowUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The agent name | [default to undefined]
**description** | **string** | The agent description | [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**config** | [**FlowConfig**](FlowConfig.md) | The agent configuration | [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**branch** | [**FlowBranch**](FlowBranch.md) | The agent branch | [optional] [default to undefined]
**enable_cache** | **boolean** |  | [optional] [default to undefined]
**version_nr** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowUpdate } from 'flowhunt';

const instance: FlowUpdate = {
    name,
    description,
    detailed_description,
    config,
    category_id,
    branch,
    enable_cache,
    version_nr,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
