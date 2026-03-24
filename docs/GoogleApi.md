# GoogleApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCalendars**](#getcalendars) | **GET** /v2/integrations/google/calendar | Get Calendars|
|[**getPickerToken**](#getpickertoken) | **GET** /v2/integrations/google/picker_token | Get Picker Token|
|[**getSheets**](#getsheets) | **GET** /v2/integrations/google/sheets/{document_id} | Get Sheets|

# **getCalendars**
> GoogleCalendarsResponse getCalendars()


### Example

```typescript
import {
    GoogleApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getCalendars(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleCalendarsResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getPickerToken**
> GooglePickerTokenResponse getPickerToken()


### Example

```typescript
import {
    GoogleApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getPickerToken(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GooglePickerTokenResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSheets**
> GoogleSheetsResponse getSheets()


### Example

```typescript
import {
    GoogleApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleApi(configuration);

let documentId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSheets(
    documentId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleSheetsResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

