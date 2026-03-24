# ScheduleUrlSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schedule_id** | **string** |  | [optional] [default to undefined]
**domain_id** | **string** |  | [optional] [default to undefined]
**url_id** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**text_timestamp_from** | **string** |  | [optional] [default to undefined]
**text_timestamp_to** | **string** |  | [optional] [default to undefined]
**url_title** | **string** |  | [optional] [default to undefined]
**is_original_url** | **boolean** |  | [optional] [default to undefined]
**created_at_from** | **string** |  | [optional] [default to undefined]
**created_at_to** | **string** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ScheduleUrlSearchRequest } from 'flowhunt';

const instance: ScheduleUrlSearchRequest = {
    schedule_id,
    domain_id,
    url_id,
    url,
    text_timestamp_from,
    text_timestamp_to,
    url_title,
    is_original_url,
    created_at_from,
    created_at_to,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
