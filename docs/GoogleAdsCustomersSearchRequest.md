# GoogleAdsCustomersSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
**customer_name** | **string** |  | [optional] [default to undefined]
**language_code** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**min_queries** | **number** |  | [optional] [default to undefined]
**min_clicks** | **number** |  | [optional] [default to undefined]
**process_negative_keywords** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**min_impressions** | **number** |  | [optional] [default to undefined]
**cluster_strength** | **number** |  | [optional] [default to undefined]
**last_update** | **string** |  | [optional] [default to undefined]
**next_update** | **string** |  | [optional] [default to undefined]
**action_type** | [**GoogleAdsActionType**](GoogleAdsActionType.md) |  | [optional] [default to undefined]
**ga_measurement_id** | **string** |  | [optional] [default to undefined]
**ga_api_secret** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { GoogleAdsCustomersSearchRequest } from 'flowhunt';

const instance: GoogleAdsCustomersSearchRequest = {
    customer_id,
    customer_name,
    language_code,
    country,
    min_queries,
    min_clicks,
    process_negative_keywords,
    min_impressions,
    cluster_strength,
    last_update,
    next_update,
    action_type,
    ga_measurement_id,
    ga_api_secret,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
