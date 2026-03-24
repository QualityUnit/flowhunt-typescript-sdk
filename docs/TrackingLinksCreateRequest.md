# TrackingLinksCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**Array&lt;TrackingLinkCreateRequest&gt;**](TrackingLinkCreateRequest.md) | The list of links to be created | [default to undefined]
**with_address** | **boolean** |  | [optional] [default to undefined]
**unique_id** | **string** |  | [optional] [default to undefined]
**fp** | **string** |  | [optional] [default to undefined]
**session_id** | **string** |  | [optional] [default to undefined]
**ga** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { TrackingLinksCreateRequest } from 'flowhunt';

const instance: TrackingLinksCreateRequest = {
    links,
    with_address,
    unique_id,
    fp,
    session_id,
    ga,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
