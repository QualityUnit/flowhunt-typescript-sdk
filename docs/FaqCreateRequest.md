# FaqCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cat_id** | **string** | Category ID | [default to undefined]
**primary_question** | **string** | Question | [default to undefined]
**answer** | **string** |  | [optional] [default to undefined]
**secondary_questions** | **Array&lt;string&gt;** | Parent FAQ ID if current question points to other answer | [optional] [default to undefined]

## Example

```typescript
import { FaqCreateRequest } from 'flowhunt';

const instance: FaqCreateRequest = {
    cat_id,
    primary_question,
    answer,
    secondary_questions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
