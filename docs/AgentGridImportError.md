# AgentGridImportError

Schema for a single import error.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**row** | **number** | Row number where the error occurred (1-indexed) | [default to undefined]
**field** | **string** | Field name that caused the error | [default to undefined]
**error** | **string** | Error message | [default to undefined]

## Example

```typescript
import { AgentGridImportError } from 'flowhunt';

const instance: AgentGridImportError = {
    row,
    field,
    error,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
