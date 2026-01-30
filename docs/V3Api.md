# V3Api

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**checkMigrationReadiness**](#checkmigrationreadiness) | **GET** /v3/flows/{flow_id}/migration-readiness | Check Migration Readiness|
|[**createV3FlowAssistantSession**](#createv3flowassistantsession) | **POST** /v3/flow-assistants/create | Create V3 Flow Assistant Session|
|[**getAllComponentsV3**](#getallcomponentsv3) | **GET** /v3/flows/components/all | Get All Components V3|
|[**getTool**](#gettool) | **GET** /v3/tools/{step_name} | Get Tool|
|[**getV3Components**](#getv3components) | **GET** /v3/flows/components/v3 | Get V3 Components|
|[**invokeV3FlowAssistantResponse**](#invokev3flowassistantresponse) | **POST** /v3/flow-assistants/{session_id}/invoke | Invoke V3 Flow Assistant Response|
|[**listTools**](#listtools) | **GET** /v3/tools | List Tools|
|[**migrateFlowToV3**](#migrateflowtov3) | **POST** /v3/flows/{flow_id}/migrate-to-v3 | Migrate Flow To V3|
|[**pollV3FlowAssistantResponse**](#pollv3flowassistantresponse) | **POST** /v3/flow-assistants/{session_id}/invocation_response/{from_timestamp} | Poll V3 Flow Assistant Response|
|[**validateComponent**](#validatecomponent) | **POST** /v3/flows/components/{component_id}/validate | Validate Component|
|[**validateFlow**](#validateflow) | **POST** /v3/flows/validate | Validate Flow|

# **checkMigrationReadiness**
> { [key: string]: any; } checkMigrationReadiness()

Check if a flow is ready to be migrated to v3.  Returns information about: - Whether the flow can be migrated - Current engine version - Incompatible components (if any) - List of available v3 components  Args:     workspace_id: The workspace ID     flow_id: The flow ID to check     flow_v3_controller: Injected controller     user: Current authenticated user  Returns:     Dict with migration readiness information

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.checkMigrationReadiness(
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

**{ [key: string]: any; }**

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

# **createV3FlowAssistantSession**
> FlowSessionResponse createV3FlowAssistantSession(flowAssistantSessionCreateRequest)

Create a new assistant session.  Returns session_id and created_at for the new session.

### Example

```typescript
import {
    V3Api,
    Configuration,
    FlowAssistantSessionCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

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

# **getAllComponentsV3**
> { [key: string]: any; } getAllComponentsV3()

Get all v3 components with full metadata, organized by category.  Returns V2-compatible component structure with rich metadata including: - display_name, description, icon - Parameter definitions with types, defaults, UI field types - Output field definitions - Category organization  This endpoint is compatible with the v2 flow editor UI.  Returns:     Dict mapping category names to component definitions.     Example: {\"inputs\": {\"ChatInput\": {...}}, \"llms\": {\"OpenAILLM\": {...}}}

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

const { status, data } = await apiInstance.getAllComponentsV3();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**{ [key: string]: any; }**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getTool**
> V3ToolResponse getTool()

Get a specific tool with full parameter details.  Returns detailed information about a tool including all parameters that can be configured or locked.  Args:     workspace_id: The workspace ID     step_name: The step name to retrieve     tools_controller: Injected controller     user: Current authenticated user  Returns:     V3ToolResponse with full tool details  Raises:     404: If tool not found

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let stepName: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getTool(
    stepName,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **stepName** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**V3ToolResponse**

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

# **getV3Components**
> { [key: string]: any; } getV3Components()

Get list of v3-compatible components.  Returns:     Dict with list of registered v3 components and count

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

const { status, data } = await apiInstance.getV3Components();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**{ [key: string]: any; }**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **invokeV3FlowAssistantResponse**
> FlowSessionInvocationResponse invokeV3FlowAssistantResponse(flowAssistantInvokeRequest)

Start an assistant invocation.  Returns immediately - client polls for events via invocation_response endpoint.

### Example

```typescript
import {
    V3Api,
    Configuration,
    FlowAssistantInvokeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

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

# **listTools**
> V3ToolListResponse listTools()

List all available V3 tools.  Returns a list of tools that can be used with AI Agents. Supports optional search and category filtering.  Args:     workspace_id: The workspace ID     search: Optional search query     category: Optional category filter     tools_controller: Injected controller     user: Current authenticated user  Returns:     V3ToolListResponse with list of available tools

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let workspaceId: string; // (default to undefined)
let search: string; //Search query for tool name, description, or category (optional) (default to undefined)
let category: string; //Filter by category (optional) (default to undefined)

const { status, data } = await apiInstance.listTools(
    workspaceId,
    search,
    category
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **search** | [**string**] | Search query for tool name, description, or category | (optional) defaults to undefined|
| **category** | [**string**] | Filter by category | (optional) defaults to undefined|


### Return type

**V3ToolListResponse**

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

# **migrateFlowToV3**
> FlowDetailResponse migrateFlowToV3()

Migrate a v2 flow to v3 engine.  This endpoint: 1. Validates that all components in the flow are v3-compatible 2. Creates a new draft version of the flow with engine_version=\'v3\' 3. Returns the migrated flow details  Args:     workspace_id: The workspace ID     flow_id: The flow ID to migrate     force: If True, skip compatibility check (dangerous!)     remove_incompatible: If True, remove incompatible components instead of failing     flow_v3_controller: Injected controller     user: Current authenticated user  Returns:     FlowDetailResponse with the migrated flow

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let force: boolean; //Skip compatibility check if True (optional) (default to false)
let removeIncompatible: boolean; //Remove incompatible components instead of failing (optional) (default to false)

const { status, data } = await apiInstance.migrateFlowToV3(
    flowId,
    workspaceId,
    force,
    removeIncompatible
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **force** | [**boolean**] | Skip compatibility check if True | (optional) defaults to false|
| **removeIncompatible** | [**boolean**] | Remove incompatible components instead of failing | (optional) defaults to false|


### Return type

**FlowDetailResponse**

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

# **pollV3FlowAssistantResponse**
> Array<FlowSessionEvent> pollV3FlowAssistantResponse()

Poll for events after the given timestamp.  Used by client to receive streamed responses from the assistant.

### Example

```typescript
import {
    V3Api,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

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

# **validateComponent**
> ComponentValidationResponse validateComponent(componentValidateRequest)

Validate a V3 component configuration.  Validates that all required parameters have values and performs any component-specific validation rules.  Args:     component_id: The component type to validate (e.g., \"OpenAILLM\")     request: Request body with template values  Returns:     ComponentValidationResponse with is_valid flag and error list

### Example

```typescript
import {
    V3Api,
    Configuration,
    ComponentValidateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let componentId: string; // (default to undefined)
let componentValidateRequest: ComponentValidateRequest; //

const { status, data } = await apiInstance.validateComponent(
    componentId,
    componentValidateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **componentValidateRequest** | **ComponentValidateRequest**|  | |
| **componentId** | [**string**] |  | defaults to undefined|


### Return type

**ComponentValidationResponse**

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

# **validateFlow**
> FlowValidationResponse validateFlow(flowValidateRequest)

Validate an entire V3 flow before publishing.  Validates all nodes in the flow, checking that required parameters have values and all component configurations are valid.  Args:     request: Request body with list of nodes to validate  Returns:     FlowValidationResponse with is_valid flag and list of errors     including node_id and component_type for each error

### Example

```typescript
import {
    V3Api,
    Configuration,
    FlowValidateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new V3Api(configuration);

let flowValidateRequest: FlowValidateRequest; //

const { status, data } = await apiInstance.validateFlow(
    flowValidateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowValidateRequest** | **FlowValidateRequest**|  | |


### Return type

**FlowValidationResponse**

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

