# MemoryDocumentProcessRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cat_id** | **string** | Category ID | [default to undefined]
**flow_id** | **string** | Flow ID to process the documents | [default to undefined]
**doc_ids** | **Array&lt;string&gt;** | List of document IDs to process | [default to undefined]
**parent_node_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { MemoryDocumentProcessRequest } from 'flowhunt';

const instance: MemoryDocumentProcessRequest = {
    cat_id,
    flow_id,
    doc_ids,
    parent_node_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
