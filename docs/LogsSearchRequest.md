# LogsSearchRequest

Request model for searching logs.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**log_types** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**log_levels** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**from_date** | **string** |  | [optional] [default to undefined]
**to_date** | **string** |  | [optional] [default to undefined]
**search_text** | **string** |  | [optional] [default to undefined]
**page** | **number** | Page number for pagination | [optional] [default to 1]
**page_size** | **number** | Number of results per page | [optional] [default to 50]
**sort_by** | **string** | Field to sort results by | [optional] [default to 'created_at']
**sort_direction** | [**SortDirection**](SortDirection.md) | Sort direction (asc or desc) | [optional] [default to undefined]

## Example

```typescript
import { LogsSearchRequest } from 'flowhunt';

const instance: LogsSearchRequest = {
    log_types,
    log_levels,
    category_id,
    from_date,
    to_date,
    search_text,
    page,
    page_size,
    sort_by,
    sort_direction,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
