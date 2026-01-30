# LogsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchLogs**](#searchlogs) | **POST** /v2/logs/search | Search logs|

# **searchLogs**
> Array<LogResponse> searchLogs(logsSearchRequest)

Search for logs based on various criteria

### Example

```typescript
import {
    LogsApi,
    Configuration,
    LogsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new LogsApi(configuration);

let workspaceId: string; // (default to undefined)
let logsSearchRequest: LogsSearchRequest; //

const { status, data } = await apiInstance.searchLogs(
    workspaceId,
    logsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **logsSearchRequest** | **LogsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<LogResponse>**

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

