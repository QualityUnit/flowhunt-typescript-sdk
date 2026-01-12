# SchedulesApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createSchedules**](#createschedules) | **POST** /v2/schedules/create | Create Schedules|
|[**deleteSchedule**](#deleteschedule) | **DELETE** /v2/schedules/{schedule_id} | Delete Schedule|
|[**deleteScheduleUrl**](#deletescheduleurl) | **DELETE** /v2/schedules/{schedule_id}/urls/{domain_id}/{url_id} | Delete Schedule Url|
|[**getSchedule**](#getschedule) | **GET** /v2/schedules/{schedule_id} | Get Schedule|
|[**getScheduleUrlDetails**](#getscheduleurldetails) | **GET** /v2/schedules/{schedule_id}/urls/{domain_id}/{url_id} | Get Schedule Url Details|
|[**getSchedules**](#getschedules) | **POST** /v2/schedules/ | Get Schedules|
|[**runSchedule**](#runschedule) | **POST** /v2/schedules/run/{schedule_id} | Run Schedule|
|[**searchScheduleUrls**](#searchscheduleurls) | **POST** /v2/schedules/urls/ | Search Schedule Urls|
|[**updateSchedule**](#updateschedule) | **PUT** /v2/schedules/{schedule_id} | Update Schedule|

# **createSchedules**
> Array<ScheduleResponse> createSchedules(scheduleCreateRequest)


### Example

```typescript
import {
    SchedulesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let workspaceId: string; // (default to undefined)
let scheduleCreateRequest: Array<ScheduleCreateRequest>; //

const { status, data } = await apiInstance.createSchedules(
    workspaceId,
    scheduleCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleCreateRequest** | **Array<ScheduleCreateRequest>**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ScheduleResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteSchedule**
> Completed deleteSchedule()


### Example

```typescript
import {
    SchedulesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteSchedule(
    scheduleId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteScheduleUrl**
> Completed deleteScheduleUrl(scheduleUrlDeleteRequest)


### Example

```typescript
import {
    SchedulesApi,
    Configuration,
    ScheduleUrlDeleteRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let urlId: string; // (default to undefined)
let domainId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let scheduleUrlDeleteRequest: ScheduleUrlDeleteRequest; //

const { status, data } = await apiInstance.deleteScheduleUrl(
    scheduleId,
    urlId,
    domainId,
    workspaceId,
    scheduleUrlDeleteRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleUrlDeleteRequest** | **ScheduleUrlDeleteRequest**|  | |
| **scheduleId** | [**string**] |  | defaults to undefined|
| **urlId** | [**string**] |  | defaults to undefined|
| **domainId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSchedule**
> ScheduleResponse getSchedule()


### Example

```typescript
import {
    SchedulesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSchedule(
    scheduleId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ScheduleResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getScheduleUrlDetails**
> ScheduleUrlDetailResponse getScheduleUrlDetails()


### Example

```typescript
import {
    SchedulesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let urlId: string; // (default to undefined)
let domainId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getScheduleUrlDetails(
    scheduleId,
    urlId,
    domainId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleId** | [**string**] |  | defaults to undefined|
| **urlId** | [**string**] |  | defaults to undefined|
| **domainId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ScheduleUrlDetailResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSchedules**
> Array<ScheduleResponse> getSchedules(scheduleSearchRequest)


### Example

```typescript
import {
    SchedulesApi,
    Configuration,
    ScheduleSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let workspaceId: string; // (default to undefined)
let scheduleSearchRequest: ScheduleSearchRequest; //

const { status, data } = await apiInstance.getSchedules(
    workspaceId,
    scheduleSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleSearchRequest** | **ScheduleSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ScheduleResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **runSchedule**
> Completed runSchedule()


### Example

```typescript
import {
    SchedulesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.runSchedule(
    scheduleId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchScheduleUrls**
> Array<ScheduleUrlResponse> searchScheduleUrls(scheduleUrlSearchRequest)


### Example

```typescript
import {
    SchedulesApi,
    Configuration,
    ScheduleUrlSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let workspaceId: string; // (default to undefined)
let scheduleUrlSearchRequest: ScheduleUrlSearchRequest; //

const { status, data } = await apiInstance.searchScheduleUrls(
    workspaceId,
    scheduleUrlSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleUrlSearchRequest** | **ScheduleUrlSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ScheduleUrlResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateSchedule**
> ScheduleResponse updateSchedule(scheduleUpdateRequest)


### Example

```typescript
import {
    SchedulesApi,
    Configuration,
    ScheduleUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SchedulesApi(configuration);

let scheduleId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let scheduleUpdateRequest: ScheduleUpdateRequest; //

const { status, data } = await apiInstance.updateSchedule(
    scheduleId,
    workspaceId,
    scheduleUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **scheduleUpdateRequest** | **ScheduleUpdateRequest**|  | |
| **scheduleId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ScheduleResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

