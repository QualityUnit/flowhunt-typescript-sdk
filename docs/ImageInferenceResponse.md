# ImageInferenceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inference_id** | **string** | The ID of the inference | [default to undefined]
**image_url_outputs** | **Array&lt;string&gt;** | The URL of the image | [default to undefined]
**date_created** | **string** | The date the image was created | [default to undefined]
**prompt** | **string** | The prompt used for the inference | [default to undefined]
**styles** | **Array&lt;string&gt;** | The styles used for the inference | [default to undefined]
**effects** | **Array&lt;string&gt;** | The effects used for the inference | [default to undefined]
**aspect_ratio** | **string** | The aspect ratio of the output images | [default to undefined]
**ai_model** | **string** | The AI model used for the inference | [default to undefined]
**status** | **string** | The status of the inference | [default to undefined]

## Example

```typescript
import { ImageInferenceResponse } from 'flowhunt';

const instance: ImageInferenceResponse = {
    inference_id,
    image_url_outputs,
    date_created,
    prompt,
    styles,
    effects,
    aspect_ratio,
    ai_model,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
