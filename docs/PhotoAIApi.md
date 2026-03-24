# PhotoAIApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**explore**](#explore) | **GET** /v2/photo_ai/public/explore | Explore|
|[**getEffects**](#geteffects) | **GET** /v2/photo_ai/public/effects | Get Effects|
|[**getStyles**](#getstyles) | **GET** /v2/photo_ai/public/styles | Get Styles|
|[**getTemplates**](#gettemplates) | **GET** /v2/photo_ai/public/templates | Get Templates|

# **explore**
> Array<CommunityImageGenerationsResponse> explore()


### Example

```typescript
import {
    PhotoAIApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PhotoAIApi(configuration);

const { status, data } = await apiInstance.explore();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<CommunityImageGenerationsResponse>**

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

# **getEffects**
> Array<PhotoAIEffectResponse> getEffects()


### Example

```typescript
import {
    PhotoAIApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PhotoAIApi(configuration);

const { status, data } = await apiInstance.getEffects();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<PhotoAIEffectResponse>**

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

# **getStyles**
> Array<PhotoAIStyleResponse> getStyles()


### Example

```typescript
import {
    PhotoAIApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PhotoAIApi(configuration);

const { status, data } = await apiInstance.getStyles();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<PhotoAIStyleResponse>**

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

# **getTemplates**
> Array<PhotoAITemplateResponse> getTemplates()


### Example

```typescript
import {
    PhotoAIApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new PhotoAIApi(configuration);

const { status, data } = await apiInstance.getTemplates();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<PhotoAITemplateResponse>**

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

