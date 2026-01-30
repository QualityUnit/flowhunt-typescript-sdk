# ScreenshotResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Task ID | [default to undefined]
**status** | [**TaskStatus**](TaskStatus.md) | Task status | [default to undefined]
**result** | **string** |  | [optional] [default to undefined]
**error_message** | **string** |  | [optional] [default to undefined]
**original_size_url** | [**AppUrlOutput**](AppUrlOutput.md) |  | [optional] [default to undefined]
**thumbnail_url** | [**AppUrlOutput**](AppUrlOutput.md) |  | [optional] [default to undefined]
**original_size_url_full_page** | [**AppUrlOutput**](AppUrlOutput.md) |  | [optional] [default to undefined]
**thumbnail_url_full_page** | [**AppUrlOutput**](AppUrlOutput.md) |  | [optional] [default to undefined]
**timestamp** | **number** |  | [optional] [default to undefined]
**domain_id** | **string** |  | [optional] [default to undefined]
**url_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ScreenshotResponse } from 'flowhunt';

const instance: ScreenshotResponse = {
    id,
    status,
    result,
    error_message,
    original_size_url,
    thumbnail_url,
    original_size_url_full_page,
    thumbnail_url_full_page,
    timestamp,
    domain_id,
    url_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
