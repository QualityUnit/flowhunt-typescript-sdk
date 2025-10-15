# MemoryApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createNode**](#createnode) | **POST** /v2/memory/node/create | Create Node|
|[**deleteNode**](#deletenode) | **DELETE** /v2/memory/node/{node_id} | Delete Node|
|[**getNode**](#getnode) | **POST** /v2/memory/node/{node_id} | Get Node|
|[**processDocuments**](#processdocuments) | **POST** /v2/memory/process-documents | Process Documents|
|[**searchMemoryCategories**](#searchmemorycategories) | **POST** /v2/memory/search | Search Memory Categories|
|[**searchMemoryNodeName**](#searchmemorynodename) | **POST** /v2/memory/search_node_name | Search Memory Node Name|
|[**searchMemoryNodePath**](#searchmemorynodepath) | **POST** /v2/memory/search_node_path | Search Memory Node Path|
|[**updateNode**](#updatenode) | **PUT** /v2/memory/node/{node_id} | Update Node|
|[**uploadDocument**](#uploaddocument) | **POST** /v2/memory/upload/{cat_id} | Upload Document|

# **createNode**
> MemoryNodeResponse createNode(nodeDetailRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    NodeDetailRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let workspaceId: string; // (default to undefined)
let nodeDetailRequest: NodeDetailRequest; //

const { status, data } = await apiInstance.createNode(
    workspaceId,
    nodeDetailRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **nodeDetailRequest** | **NodeDetailRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MemoryNodeResponse**

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

# **deleteNode**
> MemoryMessageResponse deleteNode(deleteNodeRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    DeleteNodeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let nodeId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let deleteNodeRequest: DeleteNodeRequest; //

const { status, data } = await apiInstance.deleteNode(
    nodeId,
    workspaceId,
    deleteNodeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deleteNodeRequest** | **DeleteNodeRequest**|  | |
| **nodeId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MemoryMessageResponse**

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

# **getNode**
> MemoryNodeDetailResponse getNode(getNodeRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    GetNodeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let nodeId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let getNodeRequest: GetNodeRequest; //

const { status, data } = await apiInstance.getNode(
    nodeId,
    workspaceId,
    getNodeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **getNodeRequest** | **GetNodeRequest**|  | |
| **nodeId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MemoryNodeDetailResponse**

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

# **processDocuments**
> MemoryMessageResponse processDocuments(memoryDocumentProcessRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    MemoryDocumentProcessRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let workspaceId: string; // (default to undefined)
let memoryDocumentProcessRequest: MemoryDocumentProcessRequest; //

const { status, data } = await apiInstance.processDocuments(
    workspaceId,
    memoryDocumentProcessRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **memoryDocumentProcessRequest** | **MemoryDocumentProcessRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MemoryMessageResponse**

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

# **searchMemoryCategories**
> Array<MemorySearchResponse> searchMemoryCategories(memorySearchRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    MemorySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let workspaceId: string; // (default to undefined)
let memorySearchRequest: MemorySearchRequest; //

const { status, data } = await apiInstance.searchMemoryCategories(
    workspaceId,
    memorySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **memorySearchRequest** | **MemorySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<MemorySearchResponse>**

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

# **searchMemoryNodeName**
> Array<MemorySearchResponse> searchMemoryNodeName(memoryNodeNameSearchRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    MemoryNodeNameSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let workspaceId: string; // (default to undefined)
let memoryNodeNameSearchRequest: MemoryNodeNameSearchRequest; //

const { status, data } = await apiInstance.searchMemoryNodeName(
    workspaceId,
    memoryNodeNameSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **memoryNodeNameSearchRequest** | **MemoryNodeNameSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<MemorySearchResponse>**

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

# **searchMemoryNodePath**
> Array<MemorySearchResponse> searchMemoryNodePath(memoryNodePathSearchRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    MemoryNodePathSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let workspaceId: string; // (default to undefined)
let memoryNodePathSearchRequest: MemoryNodePathSearchRequest; //

const { status, data } = await apiInstance.searchMemoryNodePath(
    workspaceId,
    memoryNodePathSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **memoryNodePathSearchRequest** | **MemoryNodePathSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<MemorySearchResponse>**

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

# **updateNode**
> MemoryNodeResponse updateNode(nodeUpdateRequest)


### Example

```typescript
import {
    MemoryApi,
    Configuration,
    NodeUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let nodeId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let nodeUpdateRequest: NodeUpdateRequest; //

const { status, data } = await apiInstance.updateNode(
    nodeId,
    workspaceId,
    nodeUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **nodeUpdateRequest** | **NodeUpdateRequest**|  | |
| **nodeId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MemoryNodeResponse**

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

# **uploadDocument**
> MemoryDocumentUploadResponse uploadDocument()


### Example

```typescript
import {
    MemoryApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MemoryApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: File; // (default to undefined)

const { status, data } = await apiInstance.uploadDocument(
    catId,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|


### Return type

**MemoryDocumentUploadResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

