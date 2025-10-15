# FineTuningsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createImageFt**](#createimageft) | **POST** /v2/photo_ai/images/ | Create Image Ft|
|[**deleteFileFt**](#deletefileft) | **DELETE** /v2/photo_ai/files/{file_key} | Delete File Ft|
|[**deleteImageFt**](#deleteimageft) | **DELETE** /v2/photo_ai/images/{ft_id} | Delete Image Ft|
|[**generateImagePrompt**](#generateimageprompt) | **POST** /v2/photo_ai/inference/images/generate-prompt | Generate Image Prompt|
|[**generateImages**](#generateimages) | **POST** /v2/photo_ai/inference/images | Generate Images|
|[**getFileFt**](#getfileft) | **GET** /v2/photo_ai/files/{file_key} | Get File Ft|
|[**getInferenceResults**](#getinferenceresults) | **GET** /v2/photo_ai/inference/results/{inference_id} | Get Inference Results|
|[**handleReplicateWebhook**](#handlereplicatewebhook) | **POST** /v2/photo_ai/webhooks/replicate | Handle Replicate Webhook|
|[**searchImageFts**](#searchimagefts) | **POST** /v2/photo_ai/images/search | Search Image Fts|
|[**searchInferenceHistory**](#searchinferencehistory) | **POST** /v2/photo_ai/inference/history | Search Inference History|
|[**updateImageFt**](#updateimageft) | **PUT** /v2/photo_ai/images/{ft_id} | Update Image Ft|
|[**uploadImageFt**](#uploadimageft) | **POST** /v2/photo_ai/files/{ft_type}/upload | Upload Image Ft|

# **createImageFt**
> ImageFTResponse createImageFt(imageFTCreateRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    ImageFTCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let imageFTCreateRequest: ImageFTCreateRequest; //

const { status, data } = await apiInstance.createImageFt(
    workspaceId,
    imageFTCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageFTCreateRequest** | **ImageFTCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImageFTResponse**

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

# **deleteFileFt**
> any deleteFileFt()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let fileKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let fileType: InferenceFileType; // (default to undefined)

const { status, data } = await apiInstance.deleteFileFt(
    fileKey,
    workspaceId,
    fileType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **fileKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **fileType** | **InferenceFileType** |  | defaults to undefined|


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteImageFt**
> Completed deleteImageFt()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let ftId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteImageFt(
    ftId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ftId** | [**string**] |  | defaults to undefined|
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

# **generateImagePrompt**
> ImagePromptResponse generateImagePrompt(imagePromptGenerationRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    ImagePromptGenerationRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let imagePromptGenerationRequest: ImagePromptGenerationRequest; //

const { status, data } = await apiInstance.generateImagePrompt(
    workspaceId,
    imagePromptGenerationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imagePromptGenerationRequest** | **ImagePromptGenerationRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImagePromptResponse**

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

# **generateImages**
> ImageInferenceScheduleResponse generateImages(imageInferenceRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    ImageInferenceRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let imageInferenceRequest: ImageInferenceRequest; //

const { status, data } = await apiInstance.generateImages(
    workspaceId,
    imageInferenceRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageInferenceRequest** | **ImageInferenceRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImageInferenceScheduleResponse**

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

# **getFileFt**
> any getFileFt()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let fileKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let fileType: InferenceFileType; // (default to undefined)

const { status, data } = await apiInstance.getFileFt(
    fileKey,
    workspaceId,
    fileType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **fileKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **fileType** | **InferenceFileType** |  | defaults to undefined|


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getInferenceResults**
> ImageInferenceResultResponse getInferenceResults()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let inferenceId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getInferenceResults(
    inferenceId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **inferenceId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImageInferenceResultResponse**

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

# **handleReplicateWebhook**
> Completed handleReplicateWebhook()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let ftId: string; // (default to undefined)

const { status, data } = await apiInstance.handleReplicateWebhook(
    workspaceId,
    ftId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **ftId** | [**string**] |  | defaults to undefined|


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

# **searchImageFts**
> Array<ImageFTResponse> searchImageFts(imageFTSearchRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    ImageFTSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let imageFTSearchRequest: ImageFTSearchRequest; //

const { status, data } = await apiInstance.searchImageFts(
    workspaceId,
    imageFTSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageFTSearchRequest** | **ImageFTSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ImageFTResponse>**

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

# **searchInferenceHistory**
> ImageInferenceScrollResponse searchInferenceHistory(inferenceHistorySearchRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    InferenceHistorySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let workspaceId: string; // (default to undefined)
let inferenceHistorySearchRequest: InferenceHistorySearchRequest; //

const { status, data } = await apiInstance.searchInferenceHistory(
    workspaceId,
    inferenceHistorySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **inferenceHistorySearchRequest** | **InferenceHistorySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImageInferenceScrollResponse**

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

# **updateImageFt**
> ImageFTResponse updateImageFt(imageFTUpdateRequest)


### Example

```typescript
import {
    FineTuningsApi,
    Configuration,
    ImageFTUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let ftId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let imageFTUpdateRequest: ImageFTUpdateRequest; //

const { status, data } = await apiInstance.updateImageFt(
    ftId,
    workspaceId,
    imageFTUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageFTUpdateRequest** | **ImageFTUpdateRequest**|  | |
| **ftId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ImageFTResponse**

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

# **uploadImageFt**
> FileUploadResponse uploadImageFt()


### Example

```typescript
import {
    FineTuningsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FineTuningsApi(configuration);

let ftType: FTType; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: File; // (default to undefined)

const { status, data } = await apiInstance.uploadImageFt(
    ftType,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ftType** | **FTType** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|


### Return type

**FileUploadResponse**

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

