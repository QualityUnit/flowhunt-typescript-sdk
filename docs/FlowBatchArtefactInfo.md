# FlowBatchArtefactInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique artefact identifier | [default to undefined]
**name** | **string** | File name | [default to undefined]
**size** | **number** | File size in bytes | [optional] [default to 0]
**mime_type** | **string** |  | [optional] [default to undefined]
**download_url** | **string** | Download URL | [optional] [default to '']

## Example

```typescript
import { FlowBatchArtefactInfo } from 'flowhunt';

const instance: FlowBatchArtefactInfo = {
    id,
    name,
    size,
    mime_type,
    download_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
