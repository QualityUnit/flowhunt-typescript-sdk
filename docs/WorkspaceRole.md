# WorkspaceRole


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**workspace_name** | **string** | Workspace Name | [default to undefined]
**owner_name** | **string** | Name of the owner of the workspace | [default to undefined]
**owner_email** | **string** | Email of the owner of the workspace | [default to undefined]
**role** | **string** | Role of the user in the workspace (A - Admin, E - Editor, M - Member, G - Guest) | [default to undefined]

## Example

```typescript
import { WorkspaceRole } from 'flowhunt';

const instance: WorkspaceRole = {
    workspace_id,
    workspace_name,
    owner_name,
    owner_email,
    role,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
