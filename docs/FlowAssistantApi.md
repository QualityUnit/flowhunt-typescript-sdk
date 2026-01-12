# FlowAssistantApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**applyFlowAssistantChanges**](#applyflowassistantchanges) | **POST** /v2/flow_assistants/apply_changes | Apply Flow Assistant Changes|
|[**createFlowAssistantSession**](#createflowassistantsession) | **POST** /v2/flow_assistants/create | Create Flow Assistant Session|
|[**invokeFlowAssistantResponse**](#invokeflowassistantresponse) | **POST** /v2/flow_assistants/{session_id}/invoke | Invoke Flow Assistant Response|
|[**pollFlowAssistantResponse**](#pollflowassistantresponse) | **POST** /v2/flow_assistants/{session_id}/invocation_response/{from_timestamp} | Poll Flow Assistant Response|
|[**rejectFlowAssistantChanges**](#rejectflowassistantchanges) | **POST** /v2/flow_assistants/reject_changes | Reject Flow Assistant Changes|

# **applyFlowAssistantChanges**
> FlowDetailResponse applyFlowAssistantChanges(flowAssistantApplyRejectChangesRequest)


### Example

```typescript
import {
    FlowAssistantApi,
    Configuration,
    FlowAssistantApplyRejectChangesRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantApi(configuration);

let workspaceId: string; // (default to undefined)
let flowAssistantApplyRejectChangesRequest: FlowAssistantApplyRejectChangesRequest; //

const { status, data } = await apiInstance.applyFlowAssistantChanges(
    workspaceId,
    flowAssistantApplyRejectChangesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowAssistantApplyRejectChangesRequest** | **FlowAssistantApplyRejectChangesRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createFlowAssistantSession**
> FlowSessionResponse createFlowAssistantSession(flowAssistantSessionCreateRequest)


### Example

```typescript
import {
    FlowAssistantApi,
    Configuration,
    FlowAssistantSessionCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantApi(configuration);

let workspaceId: string; // (default to undefined)
let flowAssistantSessionCreateRequest: FlowAssistantSessionCreateRequest; //

const { status, data } = await apiInstance.createFlowAssistantSession(
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

# **invokeFlowAssistantResponse**
> FlowSessionInvocationResponse invokeFlowAssistantResponse(flowAssistantInvokeRequest)


### Example

```typescript
import {
    FlowAssistantApi,
    Configuration,
    FlowAssistantInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantApi(configuration);

let sessionId: string; // (default to undefined)
let flowAssistantInvokeRequest: FlowAssistantInvokeRequest; //

const { status, data } = await apiInstance.invokeFlowAssistantResponse(
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

# **pollFlowAssistantResponse**
> Array<FlowSessionEvent> pollFlowAssistantResponse()


### Example

```typescript
import {
    FlowAssistantApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantApi(configuration);

let sessionId: string; // (default to undefined)
let fromTimestamp: string; // (default to undefined)

const { status, data } = await apiInstance.pollFlowAssistantResponse(
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

# **rejectFlowAssistantChanges**
> FlowDetailResponse rejectFlowAssistantChanges(flowAssistantApplyRejectChangesRequest)


### Example

```typescript
import {
    FlowAssistantApi,
    Configuration,
    FlowAssistantApplyRejectChangesRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowAssistantApi(configuration);

let workspaceId: string; // (default to undefined)
let flowAssistantApplyRejectChangesRequest: FlowAssistantApplyRejectChangesRequest; //

const { status, data } = await apiInstance.rejectFlowAssistantChanges(
    workspaceId,
    flowAssistantApplyRejectChangesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowAssistantApplyRejectChangesRequest** | **FlowAssistantApplyRejectChangesRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

