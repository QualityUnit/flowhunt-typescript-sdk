# NodeDetailRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cat_id** | **string** |  | [optional] [default to undefined]
**parent_node_id** | **string** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**body** | **string** |  | [optional] [default to undefined]
**node_type** | [**NodeType**](NodeType.md) |  | [optional] [default to undefined]
**position** | **number** |  | [optional] [default to undefined]
**sources** | [**Array&lt;Source&gt;**](Source.md) |  | [optional] [default to undefined]

## Example

```typescript
import { NodeDetailRequest } from 'flowhunt';

const instance: NodeDetailRequest = {
    cat_id,
    parent_node_id,
    title,
    body,
    node_type,
    position,
    sources,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
