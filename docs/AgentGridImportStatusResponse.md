# AgentGridImportStatusResponse

Schema for CSV import status response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**import_id** | **string** | Import identifier | [default to undefined]
**status** | **string** | Import status: processing, completed, or failed | [default to undefined]
**total_rows** | **number** | Total number of rows being imported | [default to undefined]
**processed_batches** | **number** | Number of batches processed so far | [default to undefined]
**total_batches** | **number** | Total number of batches | [default to undefined]
**successful_rows** | **number** | Number of rows successfully imported | [default to undefined]
**failed_rows** | **number** | Number of rows that failed to import | [default to undefined]
**progress_percentage** | **number** | Import progress as a percentage (0-100) | [default to undefined]
**errors** | [**Array&lt;AgentGridImportError&gt;**](AgentGridImportError.md) | List of import errors (max 1000) | [optional] [default to undefined]
**started_at** | **string** |  | [optional] [default to undefined]
**completed_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { AgentGridImportStatusResponse } from 'flowhunt';

const instance: AgentGridImportStatusResponse = {
    import_id,
    status,
    total_rows,
    processed_batches,
    total_batches,
    successful_rows,
    failed_rows,
    progress_percentage,
    errors,
    started_at,
    completed_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
