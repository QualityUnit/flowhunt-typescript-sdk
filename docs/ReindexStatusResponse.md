# ReindexStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scope** | [**ReindexScope**](ReindexScope.md) |  | [default to undefined]
**workspace_id** | **string** |  | [optional] [default to undefined]
**embedding_model** | **string** |  | [default to undefined]
**overall_status** | [**ReindexStatus**](ReindexStatus.md) |  | [default to undefined]
**sources** | [**{ [key: string]: ReindexProgress; }**](ReindexProgress.md) |  | [default to undefined]
**collection_name** | **string** |  | [default to undefined]
**new_collection_name** | **string** |  | [optional] [default to undefined]
**started_at** | **string** |  | [default to undefined]
**completed_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ReindexStatusResponse } from 'flowhunt';

const instance: ReindexStatusResponse = {
    scope,
    workspace_id,
    embedding_model,
    overall_status,
    sources,
    collection_name,
    new_collection_name,
    started_at,
    completed_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
