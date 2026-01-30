# FlowResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Agent ID | [default to undefined]
**name** | **string** | Agent name | [default to undefined]
**description** | **string** | Agent description | [default to undefined]
**flow_type** | [**FlowType**](FlowType.md) | Agent type | [default to undefined]
**component_count** | **number** | Component count | [default to undefined]
**executed_at** | **string** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**enable_cache** | **boolean** | Enable cache | [default to undefined]
**last_modified** | **string** |  | [optional] [default to undefined]
**engine_version** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowResponse } from 'flowhunt';

const instance: FlowResponse = {
    id,
    name,
    description,
    flow_type,
    component_count,
    executed_at,
    category_id,
    enable_cache,
    last_modified,
    engine_version,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
