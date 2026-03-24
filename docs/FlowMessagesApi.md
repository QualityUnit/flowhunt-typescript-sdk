# FlowMessagesApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchFlowMessages**](#searchflowmessages) | **POST** /v2/chatbots/search/{session_id} | Search Flow Messages|

# **searchFlowMessages**
> Array<FlowSessionEvent> searchFlowMessages()


### Example

```typescript
import {
    FlowMessagesApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowMessagesApi(configuration);

let sessionId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.searchFlowMessages(
    sessionId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowSessionEvent>**

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

