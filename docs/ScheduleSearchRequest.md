# ScheduleSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain_id** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**status** | [**ScheduleStatus**](ScheduleStatus.md) |  | [optional] [default to undefined]
**schedule_type** | [**ScheduleType**](ScheduleType.md) |  | [optional] [default to undefined]
**limit** | **number** | Limit of the search | [optional] [default to 100]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ScheduleSearchRequest } from 'flowhunt';

const instance: ScheduleSearchRequest = {
    domain_id,
    url,
    status,
    schedule_type,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
