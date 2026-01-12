# FlowWebhooksApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**executeThirdPartyWebhook**](#executethirdpartywebhook) | **POST** /v2/flows/webhooks/third_party_integrations/{trigger_type} | Execute Third Party Webhook|
|[**executeWebhook**](#executewebhook) | **POST** /v2/flows/webhooks/{chatbot_id} | Execute Webhook|
|[**executeWebhookFromFlow**](#executewebhookfromflow) | **POST** /v2/flows/webhooks/from_flow/{flow_id} | Execute Webhook From Flow|
|[**getInstallationMetadata**](#getinstallationmetadata) | **GET** /v2/flows/webhooks/third_party_integrations/installation_metadata | Get Installation Metadata|

# **executeThirdPartyWebhook**
> any executeThirdPartyWebhook()


### Example

```typescript
import {
    FlowWebhooksApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowWebhooksApi(configuration);

let triggerType: TriggerType; // (default to undefined)

const { status, data } = await apiInstance.executeThirdPartyWebhook(
    triggerType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **triggerType** | **TriggerType** |  | defaults to undefined|


### Return type

**any**

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

# **executeWebhook**
> FlowSessionInvocationResponse executeWebhook()


### Example

```typescript
import {
    FlowWebhooksApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowWebhooksApi(configuration);

let chatbotId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let triggerType: TriggerType; // (default to undefined)

const { status, data } = await apiInstance.executeWebhook(
    chatbotId,
    workspaceId,
    triggerType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **triggerType** | **TriggerType** |  | defaults to undefined|


### Return type

**FlowSessionInvocationResponse**

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

# **executeWebhookFromFlow**
> FlowSessionInvocationResponse executeWebhookFromFlow()


### Example

```typescript
import {
    FlowWebhooksApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowWebhooksApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let triggerType: TriggerType; // (default to undefined)

const { status, data } = await apiInstance.executeWebhookFromFlow(
    flowId,
    workspaceId,
    triggerType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **triggerType** | **TriggerType** |  | defaults to undefined|


### Return type

**FlowSessionInvocationResponse**

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

# **getInstallationMetadata**
> { [key: string]: any; } getInstallationMetadata()


### Example

```typescript
import {
    FlowWebhooksApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowWebhooksApi(configuration);

let workspaceId: string; // (default to undefined)
let flowId: string; // (default to undefined)
let appId: string; // (default to undefined)
let triggerType: 'on_flow_form_submission'; // (default to undefined)

const { status, data } = await apiInstance.getInstallationMetadata(
    workspaceId,
    flowId,
    appId,
    triggerType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **flowId** | [**string**] |  | defaults to undefined|
| **appId** | [**string**] |  | defaults to undefined|
| **triggerType** | [**&#39;on_flow_form_submission&#39;**]**Array<&#39;on_flow_form_submission&#39;>** |  | defaults to undefined|


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

