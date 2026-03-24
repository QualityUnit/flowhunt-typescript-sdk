# GoogleAdsGroupsSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
**campaign_id** | **string** |  | [optional] [default to undefined]
**group_id** | **string** |  | [optional] [default to undefined]
**group_name** | **string** |  | [optional] [default to undefined]
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) |  | [optional] [default to undefined]
**group_status** | [**GoogleAdsGroupStatus**](GoogleAdsGroupStatus.md) |  | [optional] [default to undefined]
**limit** | **number** | Limit of the search | [optional] [default to 50]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsGroupsSearchRequest } from 'flowhunt';

const instance: GoogleAdsGroupsSearchRequest = {
    customer_id,
    campaign_id,
    group_id,
    group_name,
    language_code,
    country,
    action_type,
    group_status,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
