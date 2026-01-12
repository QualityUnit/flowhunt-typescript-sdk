# GoogleAdsCustomerUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**min_queries** | **number** |  | [optional] [default to undefined]
**cluster_strength** | **number** |  | [optional] [default to undefined]
**min_impressions** | **number** |  | [optional] [default to undefined]
**min_clicks** | **number** |  | [optional] [default to undefined]
**process_negative_keywords** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**cron_settings** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) |  | [optional] [default to undefined]
**ga_measurement_id** | **string** |  | [optional] [default to undefined]
**ga_api_secret** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsCustomerUpdateRequest } from 'flowhunt';

const instance: GoogleAdsCustomerUpdateRequest = {
    language_code,
    country,
    min_queries,
    cluster_strength,
    min_impressions,
    min_clicks,
    process_negative_keywords,
    cron_settings,
    action_type,
    ga_measurement_id,
    ga_api_secret,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
