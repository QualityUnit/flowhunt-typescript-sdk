# ChatbotsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createChatbot**](#createchatbot) | **POST** /v2/chatbots/create | Create Chatbot|
|[**deleteChatbot**](#deletechatbot) | **DELETE** /v2/chatbots/{chatbot_id} | Delete Chatbot|
|[**getChatbot**](#getchatbot) | **GET** /v2/chatbots/{chatbot_id} | Get Chatbot|
|[**searchChatbots**](#searchchatbots) | **POST** /v2/chatbots/ | Search Chatbots|
|[**updateChatbot**](#updatechatbot) | **PUT** /v2/chatbots/{chatbot_id} | Update Chatbot|

# **createChatbot**
> ChatbotResponse createChatbot(chatbotCreateRequest)


### Example

```typescript
import {
    ChatbotsApi,
    Configuration,
    ChatbotCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ChatbotsApi(configuration);

let workspaceId: string; // (default to undefined)
let chatbotCreateRequest: ChatbotCreateRequest; //

const { status, data } = await apiInstance.createChatbot(
    workspaceId,
    chatbotCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotCreateRequest** | **ChatbotCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ChatbotResponse**

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

# **deleteChatbot**
> Completed deleteChatbot()


### Example

```typescript
import {
    ChatbotsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ChatbotsApi(configuration);

let chatbotId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteChatbot(
    chatbotId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotId** | [**string**] |  | defaults to undefined|
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

# **getChatbot**
> ChatbotResponse getChatbot()


### Example

```typescript
import {
    ChatbotsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ChatbotsApi(configuration);

let chatbotId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getChatbot(
    chatbotId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ChatbotResponse**

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

# **searchChatbots**
> Array<ChatbotResponse> searchChatbots(chatbotSearchRequest)


### Example

```typescript
import {
    ChatbotsApi,
    Configuration,
    ChatbotSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ChatbotsApi(configuration);

let workspaceId: string; // (default to undefined)
let chatbotSearchRequest: ChatbotSearchRequest; //

const { status, data } = await apiInstance.searchChatbots(
    workspaceId,
    chatbotSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotSearchRequest** | **ChatbotSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ChatbotResponse>**

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

# **updateChatbot**
> ChatbotResponse updateChatbot(chatbotUpdateRequest)


### Example

```typescript
import {
    ChatbotsApi,
    Configuration,
    ChatbotUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ChatbotsApi(configuration);

let chatbotId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let chatbotUpdateRequest: ChatbotUpdateRequest; //

const { status, data } = await apiInstance.updateChatbot(
    chatbotId,
    workspaceId,
    chatbotUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chatbotUpdateRequest** | **ChatbotUpdateRequest**|  | |
| **chatbotId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ChatbotResponse**

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

