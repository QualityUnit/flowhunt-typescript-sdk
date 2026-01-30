# ComponentValidateRequest

Request to validate a V3 component configuration.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template** | **{ [key: string]: { [key: string]: any; }; }** | Component template with parameter values. Format: {param_name: {value: any, ...}, ...} | [default to undefined]

## Example

```typescript
import { ComponentValidateRequest } from 'flowhunt';

const instance: ComponentValidateRequest = {
    template,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
