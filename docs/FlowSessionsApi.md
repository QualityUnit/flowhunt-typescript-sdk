# FlowSessionsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteChatbotSessionView**](#deletechatbotsessionview) | **DELETE** /v2/chatbots/sessions/{session_id} | Delete Chatbot Session View|
|[**getChartFeedback**](#getchartfeedback) | **POST** /v2/chatbots/sessions/charts | Get Chart Feedback|
|[**getChartSessionDuration**](#getchartsessionduration) | **POST** /v2/chatbots/sessions/chart_session_duration | Get Chart Session Duration|
|[**getChatbotSessionView**](#getchatbotsessionview) | **GET** /v2/chatbots/sessions/{session_id} | Get Chatbot Session View|
|[**getToolCallsChartFeedback**](#gettoolcallschartfeedback) | **POST** /v2/chatbots/sessions/chart_tool_calls | Get Tool Calls Chart Feedback|
|[**searchChatbotSessionsView**](#searchchatbotsessionsview) | **POST** /v2/chatbots/sessions/search | Search Chatbot Sessions View|
|[**updateChatbotSessionView**](#updatechatbotsessionview) | **PUT** /v2/chatbots/sessions/{session_id} | Update Chatbot Session View|

# **deleteChatbotSessionView**
> Completed deleteChatbotSessionView()


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let sessionId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteChatbotSessionView(
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

# **getChartFeedback**
> FeedbackChartResponse getChartFeedback(chartsFeedbackRequest)


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration,
    ChartsFeedbackRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let workspaceId: string; // (default to undefined)
let chartsFeedbackRequest: ChartsFeedbackRequest; //

const { status, data } = await apiInstance.getChartFeedback(
    workspaceId,
    chartsFeedbackRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chartsFeedbackRequest** | **ChartsFeedbackRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FeedbackChartResponse**

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

# **getChartSessionDuration**
> ChartSessionDurationResponse getChartSessionDuration(chartsFeedbackRequest)


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration,
    ChartsFeedbackRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let workspaceId: string; // (default to undefined)
let chartsFeedbackRequest: ChartsFeedbackRequest; //

const { status, data } = await apiInstance.getChartSessionDuration(
    workspaceId,
    chartsFeedbackRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chartsFeedbackRequest** | **ChartsFeedbackRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ChartSessionDurationResponse**

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

# **getChatbotSessionView**
> FlowSessionViewResponse getChatbotSessionView()


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let sessionId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getChatbotSessionView(
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

**FlowSessionViewResponse**

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

# **getToolCallsChartFeedback**
> Array<ToolCallFeedbackResponse> getToolCallsChartFeedback(chartsFeedbackRequest)


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration,
    ChartsFeedbackRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let workspaceId: string; // (default to undefined)
let chartsFeedbackRequest: ChartsFeedbackRequest; //

const { status, data } = await apiInstance.getToolCallsChartFeedback(
    workspaceId,
    chartsFeedbackRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chartsFeedbackRequest** | **ChartsFeedbackRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ToolCallFeedbackResponse>**

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

# **searchChatbotSessionsView**
> Array<FlowSessionViewResponse> searchChatbotSessionsView(flowSessionViewSearchRequest)


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration,
    FlowSessionViewSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowSessionViewSearchRequest: FlowSessionViewSearchRequest; //

const { status, data } = await apiInstance.searchChatbotSessionsView(
    workspaceId,
    flowSessionViewSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSessionViewSearchRequest** | **FlowSessionViewSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowSessionViewResponse>**

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

# **updateChatbotSessionView**
> FlowSessionViewResponse updateChatbotSessionView(flowSessionViewUpdateRequest)


### Example

```typescript
import {
    FlowSessionsApi,
    Configuration,
    FlowSessionViewUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowSessionsApi(configuration);

let sessionId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowSessionViewUpdateRequest: FlowSessionViewUpdateRequest; //

const { status, data } = await apiInstance.updateChatbotSessionView(
    sessionId,
    workspaceId,
    flowSessionViewUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSessionViewUpdateRequest** | **FlowSessionViewUpdateRequest**|  | |
| **sessionId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowSessionViewResponse**

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

