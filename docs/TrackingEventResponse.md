# TrackingEventResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_id** | **string** |  | [default to undefined]
**unique_id** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**event_name** | **string** |  | [optional] [default to undefined]
**event_value** | **number** |  | [optional] [default to undefined]
**currency** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**valid_until** | **string** |  | [optional] [default to undefined]
**include_in_conversions_metric** | **boolean** |  | [optional] [default to undefined]
**event_data** | [**Array&lt;TrackingEventData&gt;**](TrackingEventData.md) |  | [optional] [default to undefined]
**link_ids** | **Array&lt;any&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingEventResponse } from 'flowhunt';

const instance: TrackingEventResponse = {
    event_id,
    unique_id,
    url,
    event_name,
    event_value,
    currency,
    created_at,
    valid_until,
    include_in_conversions_metric,
    event_data,
    link_ids,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
