# LogResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**log_id** | **string** | Unique identifier for the log entry | [default to undefined]
**log_type** | [**LogEntryType**](LogEntryType.md) | Type of log (e.g., \&#39;system\&#39;, \&#39;application\&#39;, \&#39;user\&#39;) | [default to undefined]
**category_id** | **string** |  | [optional] [default to undefined]
**log_level** | [**LogEntryLevel**](LogEntryLevel.md) | Log level (e.g., \&#39;info\&#39;, \&#39;warning\&#39;, \&#39;error\&#39;, \&#39;debug\&#39;) | [default to undefined]
**message** | **string** | Log message content | [default to undefined]
**created_at** | **string** | Timestamp when the log was created | [default to undefined]
**metadata** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { LogResponse } from 'flowhunt';

const instance: LogResponse = {
    log_id,
    log_type,
    category_id,
    log_level,
    message,
    created_at,
    metadata,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
