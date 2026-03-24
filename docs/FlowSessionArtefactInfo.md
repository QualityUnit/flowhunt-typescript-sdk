# FlowSessionArtefactInfo

Information about a single artefact file.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique artefact identifier | [default to undefined]
**name** | **string** | File name | [default to undefined]
**path** | **string** | Relative path within workspace | [default to undefined]
**size** | **number** | File size in bytes | [default to undefined]
**modified_at** | **string** | Last modification timestamp (ISO format) | [default to undefined]
**download_url** | **string** | Public S3 URL for downloading the file | [default to undefined]

## Example

```typescript
import { FlowSessionArtefactInfo } from 'flowhunt';

const instance: FlowSessionArtefactInfo = {
    id,
    name,
    path,
    size,
    modified_at,
    download_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
