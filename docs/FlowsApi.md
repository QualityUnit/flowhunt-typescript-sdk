# FlowsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createChatbotSession**](#createchatbotsession) | **POST** /v2/flows/sessions/create | Create Chatbot Session|
|[**createFlow**](#createflow) | **POST** /v2/flows/create | Create Flow|
|[**createFlowCategory**](#createflowcategory) | **POST** /v2/flows/categories/create | Create Flow Category|
|[**createFlowCron**](#createflowcron) | **POST** /v2/flows/crons/create | Create Flow Cron|
|[**createFlowSession**](#createflowsession) | **POST** /v2/flows/sessions/from_flow/create | Create Flow Session|
|[**createMessageFeedback**](#createmessagefeedback) | **POST** /v2/flows/sessions/{session_id}/feedback | Create Message Feedback|
|[**deleteAttachment**](#deleteattachment) | **DELETE** /v2/flows/sessions/{session_id}/attachments/{file_id} | Delete Attachment|
|[**deleteFlow**](#deleteflow) | **DELETE** /v2/flows/{flow_id} | Delete Flow|
|[**deleteFlowCategory**](#deleteflowcategory) | **DELETE** /v2/flows/categories/{cat_id} | Delete Flow Category|
|[**deleteFlowCron**](#deleteflowcron) | **DELETE** /v2/flows/crons/{flow_id}/{cron_id} | Delete Flow Cron|
|[**executeFlowCron**](#executeflowcron) | **POST** /v2/flows/crons/{flow_id}/{cron_id}/execute | Execute Flow Cron|
|[**generateCommitMessage**](#generatecommitmessage) | **POST** /v2/flows/{flow_id}/generate-commit-msg | Generate Commit Message|
|[**get**](#get) | **GET** /v2/flows/{flow_id} | Get|
|[**getAllComponents**](#getallcomponents) | **GET** /v2/flows/components/all | Get All Components|
|[**getAttachments**](#getattachments) | **GET** /v2/flows/sessions/{session_id}/attachments | Get Attachments|
|[**getFlowVersions**](#getflowversions) | **GET** /v2/flows/{flow_id}/version_history | Get Flow Versions|
|[**getInvokedFlowResults**](#getinvokedflowresults) | **GET** /v2/flows/{flow_id}/{task_id} | Get Invoked Flow Results|
|[**getPublicFlow**](#getpublicflow) | **GET** /v2/flows/public/{flow_id} | Get Public Flow|
|[**getTriggerTypes**](#gettriggertypes) | **POST** /v2/flows/{flow_id}/triggers | Get Trigger Types|
|[**invokeFlow**](#invokeflow) | **POST** /v2/flows/{flow_id}/invoke | Invoke Flow|
|[**invokeFlowResponse**](#invokeflowresponse) | **POST** /v2/flows/sessions/{session_id}/invoke | Invoke Flow Response|
|[**invokeFlowSingleton**](#invokeflowsingleton) | **POST** /v2/flows/{flow_id}/invoke_singleton | Invoke Flow Singleton|
|[**pollFlowResponse**](#pollflowresponse) | **POST** /v2/flows/sessions/{session_id}/invocation_response/{from_timestamp} | Poll Flow Response|
|[**publishFlow**](#publishflow) | **POST** /v2/flows/{flow_id}/publish | Publish Flow|
|[**restoreFlowVersion**](#restoreflowversion) | **POST** /v2/flows/{flow_id}/version_history/{branch}/restore | Restore Flow Version|
|[**search**](#search) | **POST** /v2/flows/ | Search|
|[**searchAll**](#searchall) | **POST** /v2/flows/all | Search All|
|[**searchFlowCategories**](#searchflowcategories) | **POST** /v2/flows/categories/search | Search Flow Categories|
|[**searchFlowCrons**](#searchflowcrons) | **POST** /v2/flows/crons/search | Search Flow Crons|
|[**updateFlow**](#updateflow) | **PUT** /v2/flows/{flow_id} | Update Flow|
|[**updateFlowCategory**](#updateflowcategory) | **PUT** /v2/flows/categories/{cat_id} | Update Flow Category|
|[**updateFlowCron**](#updateflowcron) | **PUT** /v2/flows/crons/{flow_id}/{cron_id} | Update Flow Cron|
|[**uploadAttachments**](#uploadattachments) | **POST** /v2/flows/sessions/{session_id}/attachments | Upload Attachments|

# **createChatbotSession**
> FlowSessionResponse createChatbotSession(flowSessionCreateRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowSessionCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowSessionCreateRequest: FlowSessionCreateRequest; //

const { status, data } = await apiInstance.createChatbotSession(
    workspaceId,
    flowSessionCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSessionCreateRequest** | **FlowSessionCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowSessionResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createFlow**
> FlowDetailResponse createFlow(flowCreate)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCreate
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowCreate: FlowCreate; //

const { status, data } = await apiInstance.createFlow(
    workspaceId,
    flowCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCreate** | **FlowCreate**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createFlowCategory**
> FlowCategoryResponse createFlowCategory(flowCategoryCreateRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCategoryCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowCategoryCreateRequest: FlowCategoryCreateRequest; //

const { status, data } = await apiInstance.createFlowCategory(
    workspaceId,
    flowCategoryCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCategoryCreateRequest** | **FlowCategoryCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowCategoryResponse**

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

# **createFlowCron**
> FlowCronResponse createFlowCron(flowCronCreateRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCronCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowCronCreateRequest: FlowCronCreateRequest; //

const { status, data } = await apiInstance.createFlowCron(
    workspaceId,
    flowCronCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCronCreateRequest** | **FlowCronCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowCronResponse**

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

# **createFlowSession**
> FlowSessionResponse createFlowSession(flowSessionCreateFromFlowRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowSessionCreateFromFlowRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowSessionCreateFromFlowRequest: FlowSessionCreateFromFlowRequest; //

const { status, data } = await apiInstance.createFlowSession(
    workspaceId,
    flowSessionCreateFromFlowRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSessionCreateFromFlowRequest** | **FlowSessionCreateFromFlowRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowSessionResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createMessageFeedback**
> FlowMessageFeedbackResponse createMessageFeedback(flowMessageFeedbackRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowMessageFeedbackRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)
let flowMessageFeedbackRequest: FlowMessageFeedbackRequest; //

const { status, data } = await apiInstance.createMessageFeedback(
    sessionId,
    flowMessageFeedbackRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowMessageFeedbackRequest** | **FlowMessageFeedbackRequest**|  | |
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**FlowMessageFeedbackResponse**

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

# **deleteAttachment**
> Completed deleteAttachment()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)
let fileId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAttachment(
    sessionId,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|
| **fileId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **deleteFlow**
> Completed deleteFlow()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteFlow(
    flowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
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

# **deleteFlowCategory**
> Completed deleteFlowCategory()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteFlowCategory(
    catId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **catId** | [**string**] |  | defaults to undefined|
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

# **deleteFlowCron**
> Completed deleteFlowCron()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let cronId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteFlowCron(
    flowId,
    cronId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **cronId** | [**string**] |  | defaults to undefined|
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

# **executeFlowCron**
> TaskResponse executeFlowCron()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let cronId: string; // (default to undefined)
let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.executeFlowCron(
    cronId,
    flowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cronId** | [**string**] |  | defaults to undefined|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **generateCommitMessage**
> FlowCommitResponse generateCommitMessage()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.generateCommitMessage(
    flowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowCommitResponse**

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

# **get**
> FlowDetailResponse get()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let branch: string; // (optional) (default to 'D')

const { status, data } = await apiInstance.get(
    flowId,
    workspaceId,
    branch
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **branch** | [**string**] |  | (optional) defaults to 'D'|


### Return type

**FlowDetailResponse**

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

# **getAllComponents**
> any getAllComponents()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

const { status, data } = await apiInstance.getAllComponents();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAttachments**
> Array<FlowSessionAttachmentResponse> getAttachments()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)

const { status, data } = await apiInstance.getAttachments(
    sessionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowSessionAttachmentResponse>**

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

# **getFlowVersions**
> Array<FlowVersionHistoryResponse> getFlowVersions()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getFlowVersions(
    flowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowVersionHistoryResponse>**

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

# **getInvokedFlowResults**
> TaskResponse getInvokedFlowResults()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let taskId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getInvokedFlowResults(
    flowId,
    taskId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **taskId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **getPublicFlow**
> FlowDetailResponse getPublicFlow()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)

const { status, data } = await apiInstance.getPublicFlow(
    flowId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

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

# **getTriggerTypes**
> TriggerResponse getTriggerTypes()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getTriggerTypes(
    flowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TriggerResponse**

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

# **invokeFlow**
> TaskResponse invokeFlow(flowInvokeRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowInvokeRequest: FlowInvokeRequest; //

const { status, data } = await apiInstance.invokeFlow(
    flowId,
    workspaceId,
    flowInvokeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowInvokeRequest** | **FlowInvokeRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **invokeFlowResponse**
> FlowSessionInvocationResponse invokeFlowResponse(flowSessionInvokeRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowSessionInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)
let flowSessionInvokeRequest: FlowSessionInvokeRequest; //

const { status, data } = await apiInstance.invokeFlowResponse(
    sessionId,
    flowSessionInvokeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSessionInvokeRequest** | **FlowSessionInvokeRequest**|  | |
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

# **invokeFlowSingleton**
> TaskResponse invokeFlowSingleton(flowInvokeRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowInvokeRequest: FlowInvokeRequest; //

const { status, data } = await apiInstance.invokeFlowSingleton(
    flowId,
    workspaceId,
    flowInvokeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowInvokeRequest** | **FlowInvokeRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **pollFlowResponse**
> Array<FlowSessionEvent> pollFlowResponse()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)
let fromTimestamp: string; // (default to undefined)

const { status, data } = await apiInstance.pollFlowResponse(
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

# **publishFlow**
> FlowDetailResponse publishFlow(flowCommitRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCommitRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowCommitRequest: FlowCommitRequest; //

const { status, data } = await apiInstance.publishFlow(
    flowId,
    workspaceId,
    flowCommitRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCommitRequest** | **FlowCommitRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

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

# **restoreFlowVersion**
> Completed restoreFlowVersion()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let branch: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.restoreFlowVersion(
    flowId,
    branch,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **branch** | [**string**] |  | defaults to undefined|
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

# **search**
> Array<FlowResponse> search(flowSearchRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowSearchRequest: FlowSearchRequest; //

const { status, data } = await apiInstance.search(
    workspaceId,
    flowSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowSearchRequest** | **FlowSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowResponse>**

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

# **searchAll**
> Array<FlowResponse> searchAll(allFlowsSearchRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    AllFlowsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let allFlowsSearchRequest: AllFlowsSearchRequest; //

const { status, data } = await apiInstance.searchAll(
    workspaceId,
    allFlowsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **allFlowsSearchRequest** | **AllFlowsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowResponse>**

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

# **searchFlowCategories**
> Array<FlowCategoryResponse> searchFlowCategories(flowCategorySearchRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCategorySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowCategorySearchRequest: FlowCategorySearchRequest; //

const { status, data } = await apiInstance.searchFlowCategories(
    workspaceId,
    flowCategorySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCategorySearchRequest** | **FlowCategorySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowCategoryResponse>**

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

# **searchFlowCrons**
> Array<FlowCronResponse> searchFlowCrons(flowCronSearchRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCronSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let workspaceId: string; // (default to undefined)
let flowCronSearchRequest: FlowCronSearchRequest; //

const { status, data } = await apiInstance.searchFlowCrons(
    workspaceId,
    flowCronSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCronSearchRequest** | **FlowCronSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowCronResponse>**

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

# **updateFlow**
> FlowDetailResponse updateFlow(flowUpdate)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowUpdate
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowUpdate: FlowUpdate; //

const { status, data } = await apiInstance.updateFlow(
    flowId,
    workspaceId,
    flowUpdate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowUpdate** | **FlowUpdate**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowDetailResponse**

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

# **updateFlowCategory**
> FlowCategoryResponse updateFlowCategory(flowCategoryCreateRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCategoryCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowCategoryCreateRequest: FlowCategoryCreateRequest; //

const { status, data } = await apiInstance.updateFlowCategory(
    catId,
    workspaceId,
    flowCategoryCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCategoryCreateRequest** | **FlowCategoryCreateRequest**|  | |
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowCategoryResponse**

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

# **updateFlowCron**
> FlowCronResponse updateFlowCron(flowCronUpdateRequest)


### Example

```typescript
import {
    FlowsApi,
    Configuration,
    FlowCronUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let cronId: string; // (default to undefined)
let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowCronUpdateRequest: FlowCronUpdateRequest; //

const { status, data } = await apiInstance.updateFlowCron(
    cronId,
    flowId,
    workspaceId,
    flowCronUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowCronUpdateRequest** | **FlowCronUpdateRequest**|  | |
| **cronId** | [**string**] |  | defaults to undefined|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowCronResponse**

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

# **uploadAttachments**
> FlowSessionAttachmentResponse uploadAttachments()


### Example

```typescript
import {
    FlowsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowsApi(configuration);

let sessionId: string; // (default to undefined)
let file: File; // (default to undefined)

const { status, data } = await apiInstance.uploadAttachments(
    sessionId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|


### Return type

**FlowSessionAttachmentResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

