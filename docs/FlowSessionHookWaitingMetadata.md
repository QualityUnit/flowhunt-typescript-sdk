# FlowSessionHookWaitingMetadata

Metadata for hook waiting for input events.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**hook_id** | **string** | Hook ID for resuming the hook | [default to undefined]
**hook_name** | **string** | Hook name (e.g., \&#39;wait_for_user_input\&#39;) | [default to undefined]
**prompt_message** | **string** | Message to show the user | [default to undefined]

## Example

```typescript
import { FlowSessionHookWaitingMetadata } from 'flowhunt';

const instance: FlowSessionHookWaitingMetadata = {
    hook_id,
    hook_name,
    prompt_message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
