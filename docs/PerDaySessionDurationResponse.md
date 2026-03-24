# PerDaySessionDurationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date** | **string** | Date in YYYY-MM-DD format | [default to undefined]
**average_duration** | **number** | Average session duration in seconds | [optional] [default to 0.0]
**session_count** | **number** | Count of unique sessions (visitor count) | [optional] [default to 0]

## Example

```typescript
import { PerDaySessionDurationResponse } from 'flowhunt';

const instance: PerDaySessionDurationResponse = {
    date,
    average_duration,
    session_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
