# FlowVersionHistoryResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Agent ID | [default to undefined]
**name** | **string** | Agent name | [default to undefined]
**description** | **string** | Agent description | [default to undefined]
**version_nr** | **number** |  | [optional] [default to undefined]
**flow_type** | [**FlowType**](FlowType.md) | Agent type | [default to undefined]
**executed_at** | **string** |  | [optional] [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**enable_cache** | **boolean** | Enable cache | [default to undefined]
**user** | [**UserResponse**](UserResponse.md) |  | [optional] [default to undefined]
**branch** | **string** | Agent branch | [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**commit_title** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FlowVersionHistoryResponse } from 'flowhunt';

const instance: FlowVersionHistoryResponse = {
    id,
    name,
    description,
    version_nr,
    flow_type,
    executed_at,
    category_id,
    enable_cache,
    user,
    branch,
    created_at,
    commit_title,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
