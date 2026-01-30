# FlowValidationError

Single flow validation error with node context.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**node_id** | **string** | ID of the node with the error | [default to undefined]
**component_type** | **string** |  | [optional] [default to undefined]
**param_name** | **string** | The parameter that failed validation | [default to undefined]
**error_level** | **string** | Severity level of the validation issue | [optional] [default to ErrorLevelEnum_Error]
**message** | **string** | Human-readable error message | [default to undefined]

## Example

```typescript
import { FlowValidationError } from 'flowhunt';

const instance: FlowValidationError = {
    node_id,
    component_type,
    param_name,
    error_level,
    message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
