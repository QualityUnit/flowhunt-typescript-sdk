# ReindexApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getReindexStatus**](#getreindexstatus) | **GET** /v2/reindex/status | Get Reindex Status|
|[**triggerReindex**](#triggerreindex) | **POST** /v2/reindex/ | Trigger Reindex|

# **getReindexStatus**
> ReindexStatusResponse getReindexStatus()

Get the status of a reindex operation.  The task_id format is: {workspace_id}_{embedding_model} or installation_{embedding_model}

### Example

```typescript
import {
    ReindexApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ReindexApi(configuration);

let taskId: string; // (default to undefined)

const { status, data } = await apiInstance.getReindexStatus(
    taskId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **taskId** | [**string**] |  | defaults to undefined|


### Return type

**ReindexStatusResponse**

### Authorization

[sudo_api_key_header](../README.md#sudo_api_key_header)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **triggerReindex**
> ReindexStartResponse triggerReindex(reindexRequest)

Trigger a reindex operation for all data or a specific workspace.  This endpoint requires sudo API key authentication.  The reindex operation will: 1. Create a new versioned Qdrant collection 2. Reindex all documents, FAQs, and schedules 3. Support resume capability via Redis cursor 4. Be idempotent - can be called multiple times safely

### Example

```typescript
import {
    ReindexApi,
    Configuration,
    ReindexRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ReindexApi(configuration);

let reindexRequest: ReindexRequest; //

const { status, data } = await apiInstance.triggerReindex(
    reindexRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **reindexRequest** | **ReindexRequest**|  | |


### Return type

**ReindexStartResponse**

### Authorization

[sudo_api_key_header](../README.md#sudo_api_key_header)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

