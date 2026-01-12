# WorkspaceUserResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **string** | User ID | [default to undefined]
**email** | **string** | Email of the user | [default to undefined]
**name** | **string** | Name of the user | [default to undefined]
**avatar_url** | **string** |  | [optional] [default to undefined]
**role** | [**Role**](Role.md) | Role of the user (A - Admin, E - Editor, M - member, G - Guest) | [default to undefined]

## Example

```typescript
import { WorkspaceUserResponse } from 'flowhunt';

const instance: WorkspaceUserResponse = {
    user_id,
    email,
    name,
    avatar_url,
    role,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
