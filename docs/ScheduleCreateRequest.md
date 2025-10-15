# ScheduleCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | [**AppUrlInput**](AppUrlInput.md) |  | [default to undefined]
**frequency** | [**ScheduleFrequency**](ScheduleFrequency.md) |  | [default to undefined]
**schedule_type** | [**ScheduleType**](ScheduleType.md) |  | [default to undefined]
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
import { ScheduleCreateRequest } from 'flowhunt';

const instance: ScheduleCreateRequest = {
    url,
    frequency,
    schedule_type,
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
