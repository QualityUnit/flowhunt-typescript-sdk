# ImageFTResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ft_type** | [**FTType**](FTType.md) | Fine tuning type | [default to undefined]
**ft_id** | **string** | Fine tuning id | [default to undefined]
**name** | **string** | Fine tuning name | [default to undefined]
**steps** | **number** | Number of steps | [default to undefined]
**lora_rank** | **number** | Lora rank | [default to undefined]
**trigger_word** | **string** | Trigger word | [default to undefined]
**training_images** | **Array&lt;string&gt;** | Training images | [default to undefined]
**status** | [**FTStatus**](FTStatus.md) | Status | [default to undefined]
**cover_image** | **string** |  | [default to undefined]

## Example

```typescript
import { ImageFTResponse } from 'flowhunt';

const instance: ImageFTResponse = {
    ft_type,
    ft_id,
    name,
    steps,
    lora_rank,
    trigger_word,
    training_images,
    status,
    cover_image,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
