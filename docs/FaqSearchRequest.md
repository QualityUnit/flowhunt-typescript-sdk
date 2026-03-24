# FaqSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**faq_id** | **string** |  | [optional] [default to undefined]
**status** | [**FaqStatus**](FaqStatus.md) |  | [optional] [default to undefined]
**cat_id** | **string** |  | [optional] [default to undefined]
**question** | **string** |  | [optional] [default to undefined]
**answer** | **string** |  | [optional] [default to undefined]
**parent_faq_id** | **string** |  | [optional] [default to undefined]
**faq_type** | [**FaqType**](FaqType.md) |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FaqSearchRequest } from 'flowhunt';

const instance: FaqSearchRequest = {
    faq_id,
    status,
    cat_id,
    question,
    answer,
    parent_faq_id,
    faq_type,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
