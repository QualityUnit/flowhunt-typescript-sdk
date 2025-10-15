# TrackingSourceCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** |  | [optional] [default to undefined]
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
**links** | **Array&lt;string&gt;** | The links of the traffic source | [optional] [default to undefined]
**valid_days** | **number** |  | [optional] [default to undefined]
**with_address** | **boolean** |  | [optional] [default to undefined]
**event_data** | [**Array&lt;TrackingEventData&gt;**](TrackingEventData.md) |  | [optional] [default to undefined]
**unique_id** | **string** |  | [optional] [default to undefined]
**fp** | **string** |  | [optional] [default to undefined]
**session_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingSourceCreateRequest } from 'flowhunt';

const instance: TrackingSourceCreateRequest = {
    customer_id,
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
    links,
    valid_days,
    with_address,
    event_data,
    unique_id,
    fp,
    session_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
