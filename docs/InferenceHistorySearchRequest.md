# InferenceHistorySearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_date** | **string** |  | [optional] [default to undefined]
**to_date** | **string** |  | [optional] [default to undefined]
**limit** | **number** | The number of results to return | [optional] [default to 10]
**search_after** | **Array&lt;any&gt;** |  | [optional] [default to undefined]
**base_model** | [**BaseFoundationModel**](BaseFoundationModel.md) |  | [optional] [default to undefined]
**style** | **string** |  | [optional] [default to undefined]
**effect** | **string** |  | [optional] [default to undefined]
**aspect_ratio** | [**AspecRatio**](AspecRatio.md) |  | [optional] [default to undefined]

## Example

```typescript
import { InferenceHistorySearchRequest } from 'flowhunt';

const instance: InferenceHistorySearchRequest = {
    from_date,
    to_date,
    limit,
    search_after,
    base_model,
    style,
    effect,
    aspect_ratio,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
