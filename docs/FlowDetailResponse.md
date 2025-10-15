# FlowDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Flow ID | [default to undefined]
**name** | **string** | Flow name | [default to undefined]
**description** | **string** | Flow description | [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**config** | [**FlowConfig**](FlowConfig.md) | Flow configuration | [default to undefined]
**flow_type** | [**FlowType**](FlowType.md) | Flow type | [default to undefined]
**executed_at** | **string** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**branch** | **string** | Flow branch | [default to undefined]
**enable_cache** | **boolean** | Enable cache | [default to undefined]
**draft_version_nr** | **number** |  | [optional] [default to undefined]
**prod_version_nr** | **number** |  | [optional] [default to undefined]
**last_modified** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowDetailResponse } from 'flowhunt';

const instance: FlowDetailResponse = {
    id,
    name,
    description,
    detailed_description,
    config,
    flow_type,
    executed_at,
    category_id,
    branch,
    enable_cache,
    draft_version_nr,
    prod_version_nr,
    last_modified,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
