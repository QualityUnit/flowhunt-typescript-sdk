# TrackingSourceSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
**source_type** | [**TrackingSourceTypes**](TrackingSourceTypes.md) |  | [optional] [default to undefined]
**click_id** | **string** |  | [optional] [default to undefined]
**click_id_name** | [**TrackingClickIdNames**](TrackingClickIdNames.md) |  | [optional] [default to undefined]
**utm_source** | **string** |  | [optional] [default to undefined]
**utm_medium** | **string** |  | [optional] [default to undefined]
**utm_campaign** | **string** |  | [optional] [default to undefined]
**utm_channel** | **string** |  | [optional] [default to undefined]
**from_date** | **string** |  | [optional] [default to undefined]
**to_date** | **string** |  | [optional] [default to undefined]
**include_expired** | **boolean** |  | [optional] [default to undefined]
**page** | **number** |  | [optional] [default to undefined]
**page_size** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingSourceSearchRequest } from 'flowhunt';

const instance: TrackingSourceSearchRequest = {
    customer_id,
    source_type,
    click_id,
    click_id_name,
    utm_source,
    utm_medium,
    utm_campaign,
    utm_channel,
    from_date,
    to_date,
    include_expired,
    page,
    page_size,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
