# FlowSessionV3FlowAssistantInitMetadata

Metadata for V3 Flow Assistant initialization events.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stage** | **string** | Initialization stage (e.g., \&#39;starting\&#39;, \&#39;creating_agent\&#39;, \&#39;ready\&#39;) | [default to undefined]
**message** | **string** | User-friendly message describing the current stage | [default to undefined]

## Example

```typescript
import { FlowSessionV3FlowAssistantInitMetadata } from 'flowhunt';

const instance: FlowSessionV3FlowAssistantInitMetadata = {
    stage,
    message,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
