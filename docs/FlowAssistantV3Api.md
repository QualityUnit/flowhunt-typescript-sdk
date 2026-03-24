# FlowAssistantV3Api

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createV3FlowAssistantSession**](#createv3flowassistantsession) | **POST** /v3/flow-assistants/create | Create V3 Flow Assistant Session|
|[**invokeV3FlowAssistantResponse**](#invokev3flowassistantresponse) | **POST** /v3/flow-assistants/{session_id}/invoke | Invoke V3 Flow Assistant Response|
|[**pollV3FlowAssistantResponse**](#pollv3flowassistantresponse) | **POST** /v3/flow-assistants/{session_id}/invocation_response/{from_timestamp} | Poll V3 Flow Assistant Response|

# **createV3FlowAssistantSession**
> FlowSessionResponse createV3FlowAssistantSession(flowAssistantSessionCreateRequest)

Create a new assistant session.  Returns session_id and created_at for the new session.

### Example

```typescript
import {
    FlowAssistantV3Api,
    Configuration,
    FlowAssistantSessionCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantV3Api(configuration);

let workspaceId: string; // (default to undefined)
let flowAssistantSessionCreateRequest: FlowAssistantSessionCreateRequest; //

const { status, data } = await apiInstance.createV3FlowAssistantSession(
    workspaceId,
    flowAssistantSessionCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowAssistantSessionCreateRequest** | **FlowAssistantSessionCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowSessionResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **invokeV3FlowAssistantResponse**
> FlowSessionInvocationResponse invokeV3FlowAssistantResponse(flowAssistantInvokeRequest)

Start an assistant invocation.  Returns immediately - client polls for events via invocation_response endpoint.

### Example

```typescript
import {
    FlowAssistantV3Api,
    Configuration,
    FlowAssistantInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantV3Api(configuration);

let sessionId: string; // (default to undefined)
let flowAssistantInvokeRequest: FlowAssistantInvokeRequest; //

const { status, data } = await apiInstance.invokeV3FlowAssistantResponse(
    sessionId,
    flowAssistantInvokeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowAssistantInvokeRequest** | **FlowAssistantInvokeRequest**|  | |
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**FlowSessionInvocationResponse**

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

# **pollV3FlowAssistantResponse**
> Array<FlowSessionEvent> pollV3FlowAssistantResponse()

Poll for events after the given timestamp.  Used by client to receive streamed responses from the assistant.

### Example

```typescript
import {
    FlowAssistantV3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantV3Api(configuration);

let sessionId: string; // (default to undefined)
let fromTimestamp: string; // (default to undefined)

const { status, data } = await apiInstance.pollV3FlowAssistantResponse(
    sessionId,
    fromTimestamp
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|
| **fromTimestamp** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowSessionEvent>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

