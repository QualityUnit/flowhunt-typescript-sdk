# FlowSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**flow_type** | [**FlowType**](FlowType.md) |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FlowSearchRequest } from 'flowhunt';

const instance: FlowSearchRequest = {
    flow_type,
    name,
    category_id,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
