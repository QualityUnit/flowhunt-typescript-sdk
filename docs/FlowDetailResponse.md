# FlowDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Agent ID | [default to undefined]
**name** | **string** | Agent name | [default to undefined]
**description** | **string** | Agent description | [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**config** | [**FlowConfig**](FlowConfig.md) | Agent configuration | [default to undefined]
**flow_type** | [**FlowType**](FlowType.md) | Agent type | [default to undefined]
**executed_at** | **string** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**branch** | **string** | Agent branch | [default to undefined]
**enable_cache** | **boolean** | Enable cache | [default to undefined]
**draft_version_nr** | **number** |  | [optional] [default to undefined]
**prod_version_nr** | **number** |  | [optional] [default to undefined]
**engine_version** | **string** |  | [optional] [default to undefined]
**last_modified** | **string** |  | [optional] [default to undefined]
**integration_slugs** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**webhook_base_url** | **string** |  | [optional] [default to undefined]
**try_flow_input_placeholder** | **string** |  | [optional] [default to undefined]
**disable_text_input** | **boolean** |  | [optional] [default to undefined]

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
    engine_version,
    last_modified,
    integration_slugs,
    webhook_base_url,
    try_flow_input_placeholder,
    disable_text_input,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
