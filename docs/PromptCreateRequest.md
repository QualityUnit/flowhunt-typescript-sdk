# PromptCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cat_id** | **string** | Category ID | [default to undefined]
**name** | **string** | Document name | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**prompt_text** | **string** | Prompt text | [default to undefined]
**prompt_url** | [**AppUrlInput**](AppUrlInput.md) |  | [optional] [default to undefined]

## Example

```typescript
import { PromptCreateRequest } from 'flowhunt';

const instance: PromptCreateRequest = {
    cat_id,
    name,
    description,
    prompt_text,
    prompt_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
