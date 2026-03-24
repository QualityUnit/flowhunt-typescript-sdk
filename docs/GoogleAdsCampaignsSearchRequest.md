# GoogleAdsCampaignsSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
**campaign_id** | **string** |  | [optional] [default to undefined]
**campaign_name** | **string** |  | [optional] [default to undefined]
**campaign_status** | [**GoogleAdsCampaignStatus**](GoogleAdsCampaignStatus.md) |  | [optional] [default to undefined]
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) |  | [optional] [default to undefined]
**limit** | **number** | Limit of the search | [optional] [default to 50]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsCampaignsSearchRequest } from 'flowhunt';

const instance: GoogleAdsCampaignsSearchRequest = {
    customer_id,
    campaign_id,
    campaign_name,
    campaign_status,
    language_code,
    country,
    action_type,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
