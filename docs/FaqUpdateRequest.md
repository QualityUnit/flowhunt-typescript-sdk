# FaqUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cat_id** | **string** | Category ID | [optional] [default to undefined]
**primary_question** | **string** | Question | [optional] [default to undefined]
**answer** | **string** | Answer formatted as markdow | [optional] [default to undefined]
**secondary_questions** | **Array&lt;string&gt;** | Parent FAQ ID if current question points to other answer | [optional] [default to undefined]

## Example

```typescript
import { FaqUpdateRequest } from 'flowhunt';

const instance: FaqUpdateRequest = {
    cat_id,
    primary_question,
    answer,
    secondary_questions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
