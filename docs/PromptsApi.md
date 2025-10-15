# PromptsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createPrompt**](#createprompt) | **POST** /v2/prompts/create | Create Prompt|
|[**createPromptCategory**](#createpromptcategory) | **POST** /v2/prompts/categories/create | Create Prompt Category|
|[**deletePrompt**](#deleteprompt) | **DELETE** /v2/prompts/{prompt_id} | Delete Prompt|
|[**deletePromptCategory**](#deletepromptcategory) | **DELETE** /v2/prompts/categories/{cat_id} | Delete Prompt Category|
|[**searchPromptCategories**](#searchpromptcategories) | **POST** /v2/prompts/categories/search | Search Prompt Categories|
|[**searchPrompts**](#searchprompts) | **POST** /v2/prompts/search | Search Prompts|
|[**updatePrompt**](#updateprompt) | **PUT** /v2/prompts/{prompt_id} | Update Prompt|
|[**updatePromptCategory**](#updatepromptcategory) | **PUT** /v2/prompts/categories/{cat_id} | Update Prompt Category|

# **createPrompt**
> PromptResponse createPrompt(promptCreateRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let workspaceId: string; // (default to undefined)
let promptCreateRequest: PromptCreateRequest; //

const { status, data } = await apiInstance.createPrompt(
    workspaceId,
    promptCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptCreateRequest** | **PromptCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**PromptResponse**

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

# **createPromptCategory**
> PromptCategoryResponse createPromptCategory(promptCategoryCreateRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptCategoryCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let workspaceId: string; // (default to undefined)
let promptCategoryCreateRequest: PromptCategoryCreateRequest; //

const { status, data } = await apiInstance.createPromptCategory(
    workspaceId,
    promptCategoryCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptCategoryCreateRequest** | **PromptCategoryCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**PromptCategoryResponse**

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

# **deletePrompt**
> Completed deletePrompt()


### Example

```typescript
import {
    PromptsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let promptId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deletePrompt(
    promptId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptId** | [**string**] |  | defaults to undefined|
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

# **deletePromptCategory**
> Completed deletePromptCategory()


### Example

```typescript
import {
    PromptsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deletePromptCategory(
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

# **searchPromptCategories**
> Array<PromptCategoryResponse> searchPromptCategories(promptCategorySearchRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptCategorySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let workspaceId: string; // (default to undefined)
let promptCategorySearchRequest: PromptCategorySearchRequest; //

const { status, data } = await apiInstance.searchPromptCategories(
    workspaceId,
    promptCategorySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptCategorySearchRequest** | **PromptCategorySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<PromptCategoryResponse>**

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

# **searchPrompts**
> Array<PromptResponse> searchPrompts(promptSearchRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let workspaceId: string; // (default to undefined)
let promptSearchRequest: PromptSearchRequest; //

const { status, data } = await apiInstance.searchPrompts(
    workspaceId,
    promptSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptSearchRequest** | **PromptSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<PromptResponse>**

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

# **updatePrompt**
> PromptResponse updatePrompt(promptUpdateRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let promptId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let promptUpdateRequest: PromptUpdateRequest; //

const { status, data } = await apiInstance.updatePrompt(
    promptId,
    workspaceId,
    promptUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptUpdateRequest** | **PromptUpdateRequest**|  | |
| **promptId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**PromptResponse**

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

# **updatePromptCategory**
> PromptCategoryResponse updatePromptCategory(promptCategoryUpdateRequest)


### Example

```typescript
import {
    PromptsApi,
    Configuration,
    PromptCategoryUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PromptsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let promptCategoryUpdateRequest: PromptCategoryUpdateRequest; //

const { status, data } = await apiInstance.updatePromptCategory(
    catId,
    workspaceId,
    promptCategoryUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **promptCategoryUpdateRequest** | **PromptCategoryUpdateRequest**|  | |
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**PromptCategoryResponse**

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

