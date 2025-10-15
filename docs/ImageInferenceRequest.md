# ImageInferenceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**base_model** | [**BaseFoundationModel**](BaseFoundationModel.md) | The base model to use for inference | [default to undefined]
**prompt** | **string** | The prompt to use for inference | [default to undefined]
**image_fts** | **Array&lt;string&gt;** | The list of image FTs to use for inference | [default to undefined]
**number_of_outputs** | **number** | The number of outputs to generate | [optional] [default to 1]
**aspect_ratio** | [**AspecRatio**](AspecRatio.md) | The aspect ratio of the output images | [optional] [default to undefined]
**steps** | **number** |  | [optional] [default to undefined]
**guidance_scale** | **number** |  | [optional] [default to undefined]
**styles** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**effects** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**use_ai_agent** | **boolean** |  | [optional] [default to undefined]
**reference_images** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**reference_videos** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**duration** | **number** |  | [optional] [default to undefined]
**resolution** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ImageInferenceRequest } from 'flowhunt';

const instance: ImageInferenceRequest = {
    base_model,
    prompt,
    image_fts,
    number_of_outputs,
    aspect_ratio,
    steps,
    guidance_scale,
    styles,
    effects,
    use_ai_agent,
    reference_images,
    reference_videos,
    duration,
    resolution,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
