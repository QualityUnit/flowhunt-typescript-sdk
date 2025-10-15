# ImagesApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**convertImage**](#convertimage) | **POST** /v2/images/convert | Convert Image|
|[**getScreenshot**](#getscreenshot) | **POST** /v2/images/screenshot | Get Screenshot|
|[**optimizeImage**](#optimizeimage) | **POST** /v2/images/optimize | Optimize Image|

# **convertImage**
> TaskResponse convertImage(imageConvertRequest)


### Example

```typescript
import {
    ImagesApi,
    Configuration,
    ImageConvertRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

let workspaceId: string; // (default to undefined)
let imageConvertRequest: ImageConvertRequest; //

const { status, data } = await apiInstance.convertImage(
    workspaceId,
    imageConvertRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageConvertRequest** | **ImageConvertRequest**|  | |
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

# **getScreenshot**
> ScreenshotResponse getScreenshot(screenshotRequest)


### Example

```typescript
import {
    ImagesApi,
    Configuration,
    ScreenshotRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

let workspaceId: string; // (default to undefined)
let screenshotRequest: ScreenshotRequest; //

const { status, data } = await apiInstance.getScreenshot(
    workspaceId,
    screenshotRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **screenshotRequest** | **ScreenshotRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ScreenshotResponse**

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

# **optimizeImage**
> TaskResponse optimizeImage(imageOptimizeRequest)


### Example

```typescript
import {
    ImagesApi,
    Configuration,
    ImageOptimizeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ImagesApi(configuration);

let workspaceId: string; // (default to undefined)
let imageOptimizeRequest: ImageOptimizeRequest; //

const { status, data } = await apiInstance.optimizeImage(
    workspaceId,
    imageOptimizeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **imageOptimizeRequest** | **ImageOptimizeRequest**|  | |
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

