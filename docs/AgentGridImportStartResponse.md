# AgentGridImportStartResponse

Schema for CSV import start response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**import_id** | **string** | Unique identifier for tracking the import | [default to undefined]
**total_rows** | **number** | Total number of rows to import | [default to undefined]
**message** | **string** | Status message | [default to undefined]

## Example

```typescript
import { AgentGridImportStartResponse } from 'flowhunt';

const instance: AgentGridImportStartResponse = {
    import_id,
    total_rows,
    message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
