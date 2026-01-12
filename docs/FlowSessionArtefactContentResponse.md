# FlowSessionArtefactContentResponse

Response containing artefact file content.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique artefact identifier | [default to undefined]
**name** | **string** | File name | [default to undefined]
**path** | **string** | Relative path within workspace | [default to undefined]
**size** | **number** | File size in bytes | [default to undefined]
**modified_at** | **string** | Last modification timestamp (ISO format) | [default to undefined]
**content** | **string** | File content | [default to undefined]

## Example

```typescript
import { FlowSessionArtefactContentResponse } from 'flowhunt';

const instance: FlowSessionArtefactContentResponse = {
    id,
    name,
    path,
    size,
    modified_at,
    content,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
