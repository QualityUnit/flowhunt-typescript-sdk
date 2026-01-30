# AirtableTableResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**primary_field_id** | **string** |  | [optional] [default to undefined]
**fields** | [**Array&lt;AirtableFieldResponse&gt;**](AirtableFieldResponse.md) |  | [optional] [default to undefined]
**views** | [**Array&lt;AirtableViewResponse&gt;**](AirtableViewResponse.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AirtableTableResponse } from 'flowhunt';

const instance: AirtableTableResponse = {
    id,
    name,
    description,
    primary_field_id,
    fields,
    views,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
