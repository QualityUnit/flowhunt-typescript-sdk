# GoogleAdsCustomerResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**customer_id** | **string** | Google Ads Customer ID | [default to undefined]
**customer_name** | **string** | Google Ads Customer Name | [default to undefined]
**language_code** | **string** | Language Code | [default to undefined]
**country** | **string** | Country Code | [default to undefined]
**min_queries** | **number** | Minimum Queries | [default to undefined]
**cluster_strength** | **number** | Cluster Strength | [default to undefined]
**min_impressions** | **number** | Minimum Impressions | [default to undefined]
**min_clicks** | **number** | Minimum Clicks | [default to undefined]
**process_negative_keywords** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**last_update** | **string** |  | [optional] [default to undefined]
**next_update** | **string** |  | [optional] [default to undefined]
**cron_settings** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) | Action Type | [default to undefined]
**ga_measurement_id** | **string** |  | [optional] [default to undefined]
**ga_api_secret** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsCustomerResponse } from 'flowhunt';

const instance: GoogleAdsCustomerResponse = {
    workspace_id,
    customer_id,
    customer_name,
    language_code,
    country,
    min_queries,
    cluster_strength,
    min_impressions,
    min_clicks,
    process_negative_keywords,
    last_update,
    next_update,
    cron_settings,
    action_type,
    ga_measurement_id,
    ga_api_secret,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
