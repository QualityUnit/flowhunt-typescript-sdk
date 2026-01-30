# FaqResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**faq_id** | **string** | FAQ ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**cat_id** | **string** | Category ID | [default to undefined]
**question** | **string** | Question | [default to undefined]
**answer** | **string** |  | [optional] [default to undefined]
**parent_faq_id** | **string** |  | [optional] [default to undefined]
**status** | [**FaqStatus**](FaqStatus.md) | FAQ status | [default to undefined]
**updated_at** | **string** | FAQ updated at | [default to undefined]
**indexed_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FaqResponse } from 'flowhunt';

const instance: FaqResponse = {
    faq_id,
    workspace_id,
    cat_id,
    question,
    answer,
    parent_faq_id,
    status,
    updated_at,
    indexed_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
