# ReindexProgress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** |  | [optional] [default to undefined]
**embedding_model** | **string** |  | [default to undefined]
**status** | [**ReindexStatus**](ReindexStatus.md) |  | [default to undefined]
**data_source** | [**ReindexDataSource**](ReindexDataSource.md) |  | [default to undefined]
**total_items** | **number** |  | [optional] [default to 0]
**processed_items** | **number** |  | [optional] [default to 0]
**failed_items** | **number** |  | [optional] [default to 0]
**started_at** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]
**completed_at** | **string** |  | [optional] [default to undefined]
**error_message** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ReindexProgress } from 'flowhunt';

const instance: ReindexProgress = {
    workspace_id,
    embedding_model,
    status,
    data_source,
    total_items,
    processed_items,
    failed_items,
    started_at,
    updated_at,
    completed_at,
    error_message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
