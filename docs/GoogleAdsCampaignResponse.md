# GoogleAdsCampaignResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**customer_id** | **string** | Google Ads Customer ID | [default to undefined]
**campaign_id** | **string** | Google Ads Campaign ID | [default to undefined]
**campaign_name** | **string** | Google Ads Campaign Name | [default to undefined]
**campaign_status** | [**GoogleAdsCampaignStatus**](GoogleAdsCampaignStatus.md) | Campaign Status | [default to undefined]
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**last_update** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) | Action Type | [default to undefined]

## Example

```typescript
import { GoogleAdsCampaignResponse } from 'flowhunt';

const instance: GoogleAdsCampaignResponse = {
    workspace_id,
    customer_id,
    campaign_id,
    campaign_name,
    campaign_status,
    language_code,
    country,
    last_update,
    action_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
