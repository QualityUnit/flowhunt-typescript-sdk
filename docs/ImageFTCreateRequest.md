# ImageFTCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Fine tuning name | [default to undefined]
**trigger_word** | **string** | Trigger word | [default to undefined]
**steps** | **number** |  | [optional] [default to undefined]
**lora_rank** | **number** |  | [optional] [default to undefined]
**training_images** | **Array&lt;string&gt;** | Training images | [default to undefined]
**cover_image** | **string** | Cover image | [default to undefined]

## Example

```typescript
import { ImageFTCreateRequest } from 'flowhunt';

const instance: ImageFTCreateRequest = {
    name,
    trigger_word,
    steps,
    lora_rank,
    training_images,
    cover_image,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
