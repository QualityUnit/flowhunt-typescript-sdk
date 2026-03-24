# SemanticSearchApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getSimilarDocsByDocId**](#getsimilardocsbydocid) | **POST** /v2/similarities/document/live | Get Similar Docs By Doc Id|
|[**getSimilarDocsByQuery**](#getsimilardocsbyquery) | **POST** /v2/similarities/query/live | Get Similar Docs By Query|
|[**scheduleSimilarDocsByDocId**](#schedulesimilardocsbydocid) | **POST** /v2/similarities/document | Schedule Similar Docs By Doc Id|
|[**scheduleSimilarDocsByQuery**](#schedulesimilardocsbyquery) | **POST** /v2/similarities/query | Schedule Similar Docs By Query|

# **getSimilarDocsByDocId**
> Array<VectorDocumentResponse> getSimilarDocsByDocId(documentSimilarityRequest)


### Example

```typescript
import {
    SemanticSearchApi,
    Configuration,
    DocumentSimilarityRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SemanticSearchApi(configuration);

let workspaceId: string; // (default to undefined)
let documentSimilarityRequest: DocumentSimilarityRequest; //

const { status, data } = await apiInstance.getSimilarDocsByDocId(
    workspaceId,
    documentSimilarityRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentSimilarityRequest** | **DocumentSimilarityRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<VectorDocumentResponse>**

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

# **getSimilarDocsByQuery**
> Array<VectorDocumentResponse> getSimilarDocsByQuery(querySimilarityRequest)


### Example

```typescript
import {
    SemanticSearchApi,
    Configuration,
    QuerySimilarityRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SemanticSearchApi(configuration);

let workspaceId: string; // (default to undefined)
let querySimilarityRequest: QuerySimilarityRequest; //

const { status, data } = await apiInstance.getSimilarDocsByQuery(
    workspaceId,
    querySimilarityRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **querySimilarityRequest** | **QuerySimilarityRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<VectorDocumentResponse>**

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

# **scheduleSimilarDocsByDocId**
> VectorDocumentsTaskResponse scheduleSimilarDocsByDocId(documentSimilarityTaskRequest)


### Example

```typescript
import {
    SemanticSearchApi,
    Configuration,
    DocumentSimilarityTaskRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SemanticSearchApi(configuration);

let workspaceId: string; // (default to undefined)
let documentSimilarityTaskRequest: DocumentSimilarityTaskRequest; //

const { status, data } = await apiInstance.scheduleSimilarDocsByDocId(
    workspaceId,
    documentSimilarityTaskRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentSimilarityTaskRequest** | **DocumentSimilarityTaskRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**VectorDocumentsTaskResponse**

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

# **scheduleSimilarDocsByQuery**
> VectorDocumentsTaskResponse scheduleSimilarDocsByQuery(querySimilarityTaskRequest)


### Example

```typescript
import {
    SemanticSearchApi,
    Configuration,
    QuerySimilarityTaskRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SemanticSearchApi(configuration);

let workspaceId: string; // (default to undefined)
let querySimilarityTaskRequest: QuerySimilarityTaskRequest; //

const { status, data } = await apiInstance.scheduleSimilarDocsByQuery(
    workspaceId,
    querySimilarityTaskRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **querySimilarityTaskRequest** | **QuerySimilarityTaskRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**VectorDocumentsTaskResponse**

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

