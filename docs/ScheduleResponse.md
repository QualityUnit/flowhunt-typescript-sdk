# ScheduleResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** | Workspace ID | [default to undefined]
**schedule_id** | **string** | Schedule ID | [default to undefined]
**url** | **string** | URL to be scheduled | [default to undefined]
**frequency** | [**ScheduleFrequency**](ScheduleFrequency.md) | Frequency of the schedule D - Daily, W - Weekly, M - Monthly, Y - Yearly | [default to undefined]
**schedule_type** | [**ScheduleType**](ScheduleType.md) | Type of the schedule (U - URL, D - Domain, S - Sitemap) | [default to undefined]
**start_time** | **string** |  | [optional] [default to undefined]
**end_time** | **string** |  | [optional] [default to undefined]
**status** | [**ScheduleStatus**](ScheduleStatus.md) | Status of the schedule (N - New, F - Finished, P - Pending, E - Error, C - Cancelled | [default to undefined]
**status_message** | **string** |  | [optional] [default to undefined]
**cnt_scheduled** | **number** |  | [default to undefined]
**cnt_completed** | **number** |  | [default to undefined]
**cnt_failed** | **number** |  | [default to undefined]
**with_screenshot** | [**BoolChar**](BoolChar.md) |  | [default to undefined]
**with_browser** | [**BoolChar**](BoolChar.md) |  | [default to undefined]
**follow_links** | [**BoolChar**](BoolChar.md) |  | [default to undefined]
**with_proxy_rotation** | **string** |  | [optional] [default to undefined]
**disallow_urls** | **string** |  | [optional] [default to undefined]
**filter_urls** | **string** |  | [optional] [default to undefined]
**custom_headers** | **string** |  | [optional] [default to undefined]
**urls_extra_config** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ScheduleResponse } from 'flowhunt';

const instance: ScheduleResponse = {
    workspace_id,
    schedule_id,
    url,
    frequency,
    schedule_type,
    start_time,
    end_time,
    status,
    status_message,
    cnt_scheduled,
    cnt_completed,
    cnt_failed,
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
