# ScheduleUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**frequency** | [**ScheduleFrequency**](ScheduleFrequency.md) |  | [optional] [default to undefined]
**status** | [**ScheduleStatus**](ScheduleStatus.md) |  | [optional] [default to undefined]
**with_screenshot** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**with_browser** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**follow_links** | [**BoolChar**](BoolChar.md) |  | [optional] [default to undefined]
**with_proxy_rotation** | **string** |  | [optional] [default to undefined]
**disallow_urls** | **string** |  | [optional] [default to undefined]
**filter_urls** | **string** |  | [optional] [default to undefined]
**custom_headers** | **string** |  | [optional] [default to undefined]
**urls_extra_config** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ScheduleUpdateRequest } from 'flowhunt';

const instance: ScheduleUpdateRequest = {
    frequency,
    status,
    with_screenshot,
    with_browser,
    follow_links,
    with_proxy_rotation,
    disallow_urls,
    filter_urls,
    custom_headers,
    urls_extra_config,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
