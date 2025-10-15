# ReindexRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** |  | [optional] [default to undefined]
**embedding_model** | **string** | Name of the embedding model to use | [default to undefined]
**batch_size** | **number** | Number of items to process in each batch | [optional] [default to 100]
**force_reindex** | **boolean** | Force reindex even if the embedding model is already up-to-date | [optional] [default to false]

## Example

```typescript
import { ReindexRequest } from 'flowhunt';

const instance: ReindexRequest = {
    workspace_id,
    embedding_model,
    batch_size,
    force_reindex,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
