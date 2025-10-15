# MediaApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getTranscript**](#gettranscript) | **POST** /v2/media/transcript | Get Transcript|
|[**getTranscriptResult**](#gettranscriptresult) | **POST** /v2/media/transcript_status | Get Transcript Result|
|[**getYoutubeTranscript**](#getyoutubetranscript) | **POST** /v2/media/youtube/transcript | Get Youtube Transcript|

# **getTranscript**
> DocumentContentResponse getTranscript()


### Example

```typescript
import {
    MediaApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MediaApi(configuration);

let workspaceId: string; // (default to undefined)
let file: File; // (default to undefined)
let postbackUrl: string; //The post back URL where to send the response in body (optional) (default to undefined)

const { status, data } = await apiInstance.getTranscript(
    workspaceId,
    file,
    postbackUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|
| **postbackUrl** | [**string**] | The post back URL where to send the response in body | (optional) defaults to undefined|


### Return type

**DocumentContentResponse**

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

# **getTranscriptResult**
> DocumentContentResponse getTranscriptResult(transcriptTaskRequest)


### Example

```typescript
import {
    MediaApi,
    Configuration,
    TranscriptTaskRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MediaApi(configuration);

let workspaceId: string; // (default to undefined)
let transcriptTaskRequest: TranscriptTaskRequest; //

const { status, data } = await apiInstance.getTranscriptResult(
    workspaceId,
    transcriptTaskRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **transcriptTaskRequest** | **TranscriptTaskRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentContentResponse**

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

# **getYoutubeTranscript**
> YoutubeTranscriptResponse getYoutubeTranscript(youtubeTranscriptRequest)


### Example

```typescript
import {
    MediaApi,
    Configuration,
    YoutubeTranscriptRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MediaApi(configuration);

let workspaceId: string; // (default to undefined)
let youtubeTranscriptRequest: YoutubeTranscriptRequest; //

const { status, data } = await apiInstance.getYoutubeTranscript(
    workspaceId,
    youtubeTranscriptRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **youtubeTranscriptRequest** | **YoutubeTranscriptRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**YoutubeTranscriptResponse**

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

