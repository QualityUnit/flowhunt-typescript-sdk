# ComponentValidationResponse

Response from component validation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_valid** | **boolean** | Whether the component config is valid | [default to undefined]
**errors** | [**Array&lt;ComponentValidationError&gt;**](ComponentValidationError.md) | List of validation errors/warnings | [optional] [default to undefined]

## Example

```typescript
import { ComponentValidationResponse } from 'flowhunt';

const instance: ComponentValidationResponse = {
    is_valid,
    errors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
