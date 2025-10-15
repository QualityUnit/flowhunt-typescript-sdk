# FlowCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The flow name | [default to undefined]
**description** | **string** | The flow description | [default to undefined]
**detailed_description** | **string** |  | [optional] [default to undefined]
**config** | [**FlowConfig**](FlowConfig.md) | The flow configuration | [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowCreate } from 'flowhunt';

const instance: FlowCreate = {
    name,
    description,
    detailed_description,
    config,
    category_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
