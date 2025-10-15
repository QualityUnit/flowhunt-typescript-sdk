# DocumentSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**doc_id** | **string** |  | [optional] [default to undefined]
**cat_id** | **string** |  | [optional] [default to undefined]
**doc_name** | **string** |  | [optional] [default to undefined]
**doc_type** | [**DocumentType**](DocumentType.md) |  | [optional] [default to undefined]
**status** | [**DocumentStatus**](DocumentStatus.md) |  | [optional] [default to undefined]
**user_status** | [**UserDocumentStatus**](UserDocumentStatus.md) |  | [optional] [default to undefined]
**updated_at_from** | **string** |  | [optional] [default to undefined]
**updated_at_to** | **string** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { DocumentSearchRequest } from 'flowhunt';

const instance: DocumentSearchRequest = {
    doc_id,
    cat_id,
    doc_name,
    doc_type,
    status,
    user_status,
    updated_at_from,
    updated_at_to,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
