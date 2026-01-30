# FlowValidationResponse

Response from flow-wide validation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_valid** | **boolean** | Whether the entire flow is valid | [default to undefined]
**errors** | [**Array&lt;FlowValidationError&gt;**](FlowValidationError.md) | List of validation errors across all nodes | [optional] [default to undefined]

## Example

```typescript
import { FlowValidationResponse } from 'flowhunt';

const instance: FlowValidationResponse = {
    is_valid,
    errors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
