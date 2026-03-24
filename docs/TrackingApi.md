# TrackingApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchEvents**](#searchevents) | **POST** /v2/tracking/events | Search Events|
|[**searchLinks**](#searchlinks) | **POST** /v2/tracking/links | Search Links|
|[**searchSources**](#searchsources) | **POST** /v2/tracking/sources | Search Sources|
|[**trackClick**](#trackclick) | **POST** /v2/tracking/clk | Track Click|
|[**trackEvent**](#trackevent) | **POST** /v2/tracking/evnt | Track Event|
|[**trackLink**](#tracklink) | **POST** /v2/tracking/lnk | Track Link|

# **searchEvents**
> TrackingEventsResponse searchEvents(trackingEventSearchRequest)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingEventSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingEventSearchRequest: TrackingEventSearchRequest; //

const { status, data } = await apiInstance.searchEvents(
    workspaceId,
    trackingEventSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingEventSearchRequest** | **TrackingEventSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TrackingEventsResponse**

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

# **searchLinks**
> TrackingLinksResponse searchLinks(trackingLinkSearchRequest)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingLinkSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingLinkSearchRequest: TrackingLinkSearchRequest; //

const { status, data } = await apiInstance.searchLinks(
    workspaceId,
    trackingLinkSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingLinkSearchRequest** | **TrackingLinkSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TrackingLinksResponse**

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

# **searchSources**
> TrackingSourcesResponse searchSources(trackingSourceSearchRequest)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingSourceSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingSourceSearchRequest: TrackingSourceSearchRequest; //

const { status, data } = await apiInstance.searchSources(
    workspaceId,
    trackingSourceSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingSourceSearchRequest** | **TrackingSourceSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TrackingSourcesResponse**

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

# **trackClick**
> Completed trackClick(trackingSourceCreateRequest)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingSourceCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingSourceCreateRequest: TrackingSourceCreateRequest; //

const { status, data } = await apiInstance.trackClick(
    workspaceId,
    trackingSourceCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingSourceCreateRequest** | **TrackingSourceCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trackEvent**
> Completed trackEvent(trackingEventCreateRequests)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingEventCreateRequests
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingEventCreateRequests: TrackingEventCreateRequests; //

const { status, data } = await apiInstance.trackEvent(
    workspaceId,
    trackingEventCreateRequests
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingEventCreateRequests** | **TrackingEventCreateRequests**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trackLink**
> Completed trackLink(trackingLinksCreateRequest)


### Example

```typescript
import {
    TrackingApi,
    Configuration,
    TrackingLinksCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TrackingApi(configuration);

let workspaceId: string; // (default to undefined)
let trackingLinksCreateRequest: TrackingLinksCreateRequest; //

const { status, data } = await apiInstance.trackLink(
    workspaceId,
    trackingLinksCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackingLinksCreateRequest** | **TrackingLinksCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

