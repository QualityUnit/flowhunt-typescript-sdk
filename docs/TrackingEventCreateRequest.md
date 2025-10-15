# TrackingEventCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_name** | **string** | The name of the event | [default to undefined]
**unique_id** | **string** |  | [optional] [default to undefined]
**event_value** | **number** |  | [optional] [default to undefined]
**currency** | **string** |  | [optional] [default to undefined]
**event_data** | [**Array&lt;TrackingEventData&gt;**](TrackingEventData.md) |  | [optional] [default to undefined]
**link_ids** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**valid_until** | **string** |  | [optional] [default to undefined]
**conversion_action_id** | **string** |  | [optional] [default to undefined]
**include_in_conversions_metric** | **boolean** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingEventCreateRequest } from 'flowhunt';

const instance: TrackingEventCreateRequest = {
    event_name,
    unique_id,
    event_value,
    currency,
    event_data,
    link_ids,
    valid_until,
    conversion_action_id,
    include_in_conversions_metric,
    url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
