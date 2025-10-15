# MemorySearchResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**node_id** | **string** | Node ID | [default to undefined]
**node_type** | [**NodeType**](NodeType.md) |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**path** | **string** |  | [optional] [default to undefined]
**parent_id** | **string** |  | [optional] [default to undefined]
**children** | [**Array&lt;MemorySearchResponse&gt;**](MemorySearchResponse.md) |  | [optional] [default to undefined]

## Example

```typescript
import { MemorySearchResponse } from 'flowhunt';

const instance: MemorySearchResponse = {
    node_id,
    node_type,
    name,
    path,
    parent_id,
    children,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
