# GoogleAdsRecommendationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** | Customer id to get recommendations for | [default to undefined]
**campaign_id** | **string** |  | [optional] [default to undefined]
**group_id** | **string** |  | [optional] [default to undefined]
**limit** | **number** | Limit of the search | [optional] [default to 50]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsRecommendationsRequest } from 'flowhunt';

const instance: GoogleAdsRecommendationsRequest = {
    customer_id,
    campaign_id,
    group_id,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
