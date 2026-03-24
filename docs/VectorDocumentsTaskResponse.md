# VectorDocumentsTaskResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Task ID | [default to undefined]
**status** | [**TaskStatus**](TaskStatus.md) | Task status | [default to undefined]
**result** | [**Array&lt;VectorDocumentResponse&gt;**](VectorDocumentResponse.md) |  | [optional] [default to undefined]
**error_message** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { VectorDocumentsTaskResponse } from 'flowhunt';

const instance: VectorDocumentsTaskResponse = {
    id,
    status,
    result,
    error_message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
