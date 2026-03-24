# ComponentValidationError

Single component validation error.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**param_name** | **string** | The parameter that failed validation | [default to undefined]
**error_level** | **string** | Severity level of the validation issue | [optional] [default to ErrorLevelEnum_Error]
**message** | **string** | Human-readable error message | [default to undefined]

## Example

```typescript
import { ComponentValidationError } from 'flowhunt';

const instance: ComponentValidationError = {
    param_name,
    error_level,
    message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
