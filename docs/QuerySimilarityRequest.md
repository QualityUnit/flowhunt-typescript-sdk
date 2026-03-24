# QuerySimilarityRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | [**VectorDocumentType**](VectorDocumentType.md) |  | [optional] [default to undefined]
**pointer_type** | [**PointerType**](PointerType.md) |  | [optional] [default to undefined]
**schema_type** | **string** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**score_trheshold** | **number** |  | [optional] [default to undefined]
**with_vectors** | **boolean** |  | [optional] [default to undefined]
**pointer_position_from** | **number** |  | [optional] [default to undefined]
**pointer_position_to** | **number** |  | [optional] [default to undefined]
**vector_id_from** | **number** |  | [optional] [default to undefined]
**vector_id_to** | **number** |  | [optional] [default to undefined]
**filter_url** | **string** |  | [optional] [default to undefined]
**filter_domains** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**query** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { QuerySimilarityRequest } from 'flowhunt';

const instance: QuerySimilarityRequest = {
    document_type,
    pointer_type,
    schema_type,
    limit,
    score_trheshold,
    with_vectors,
    pointer_position_from,
    pointer_position_to,
    vector_id_from,
    vector_id_to,
    filter_url,
    filter_domains,
    query,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
