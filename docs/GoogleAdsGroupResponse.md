# GoogleAdsGroupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**customer_id** | **string** | Google Ads Customer ID | [default to undefined]
**campaign_id** | **string** | Google Ads Campaign ID | [default to undefined]
**group_id** | **string** | Google Ads Group | [default to undefined]
**group_name** | **string** | Google Ads Group Name | [default to undefined]
**group_status** | [**GoogleAdsGroupStatus**](GoogleAdsGroupStatus.md) | Group Status | [default to undefined]
**last_update** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) | Action Type | [default to undefined]
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsGroupResponse } from 'flowhunt';

const instance: GoogleAdsGroupResponse = {
    workspace_id,
    customer_id,
    campaign_id,
    group_id,
    group_name,
    group_status,
    last_update,
    action_type,
    language_code,
    country,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
