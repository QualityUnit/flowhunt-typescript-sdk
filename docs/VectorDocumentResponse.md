# VectorDocumentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_id** | **string** | Document ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**document_type** | [**VectorDocumentType**](VectorDocumentType.md) | Document type | [default to undefined]
**point_id** | **string** | Point ID | [default to undefined]
**pointer_position** | **number** | Pointer position | [default to undefined]
**pointer_type** | [**PointerType**](PointerType.md) | Pointer type | [default to undefined]
**schema_type** | **string** |  | [optional] [default to undefined]
**kb_key** | **string** | Knowledge key - schedule id or category id | [default to undefined]
**vector** | **Array&lt;number&gt;** |  | [default to undefined]
**vector_id** | **number** | Vector ID | [default to undefined]
**data** | [**Data**](Data.md) |  | [optional] [default to undefined]

## Example

```typescript
import { VectorDocumentResponse } from 'flowhunt';

const instance: VectorDocumentResponse = {
    document_id,
    workspace_id,
    document_type,
    point_id,
    pointer_position,
    pointer_type,
    schema_type,
    kb_key,
    vector,
    vector_id,
    data,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
