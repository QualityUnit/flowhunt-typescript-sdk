# TrackingSourceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
**link_id** | **string** |  | [optional] [default to undefined]
**source_type** | [**TrackingSourceTypes**](TrackingSourceTypes.md) |  | [default to undefined]
**click_id** | **string** |  | [optional] [default to undefined]
**click_id_name** | [**TrackingClickIdNames**](TrackingClickIdNames.md) |  | [optional] [default to undefined]
**utm_source** | **string** |  | [optional] [default to undefined]
**utm_medium** | **string** |  | [optional] [default to undefined]
**utm_campaign** | **string** |  | [optional] [default to undefined]
**utm_term** | **string** |  | [optional] [default to undefined]
**utm_content** | **string** |  | [optional] [default to undefined]
**utm_channel** | **string** |  | [optional] [default to undefined]
**ga** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**valid_until** | **string** |  | [optional] [default to undefined]
**event_data** | [**Array&lt;TrackingEventData&gt;**](TrackingEventData.md) |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingSourceResponse } from 'flowhunt';

const instance: TrackingSourceResponse = {
    customer_id,
    link_id,
    source_type,
    click_id,
    click_id_name,
    utm_source,
    utm_medium,
    utm_campaign,
    utm_term,
    utm_content,
    utm_channel,
    ga,
    url,
    created_at,
    valid_until,
    event_data,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
