# TagsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTag**](#createtag) | **POST** /v2/tags/create | Create Tag|
|[**deleteTag**](#deletetag) | **DELETE** /v2/tags/{tag_id} | Delete Tag|
|[**searchTags**](#searchtags) | **POST** /v2/tags/search | Search Tags|
|[**updateTag**](#updatetag) | **PUT** /v2/tags/{tag_id} | Update Tag|

# **createTag**
> TagResponse createTag(tagCreateRequest)


### Example

```typescript
import {
    TagsApi,
    Configuration,
    TagCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TagsApi(configuration);

let workspaceId: string; // (default to undefined)
let tagCreateRequest: TagCreateRequest; //

const { status, data } = await apiInstance.createTag(
    workspaceId,
    tagCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagCreateRequest** | **TagCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TagResponse**

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

# **deleteTag**
> Completed deleteTag()


### Example

```typescript
import {
    TagsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TagsApi(configuration);

let tagId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteTag(
    tagId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagId** | [**string**] |  | defaults to undefined|
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

# **searchTags**
> Array<TagResponse> searchTags(tagSearchRequest)


### Example

```typescript
import {
    TagsApi,
    Configuration,
    TagSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TagsApi(configuration);

let workspaceId: string; // (default to undefined)
let tagSearchRequest: TagSearchRequest; //

const { status, data } = await apiInstance.searchTags(
    workspaceId,
    tagSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagSearchRequest** | **TagSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<TagResponse>**

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

# **updateTag**
> TagResponse updateTag(tagUpdateRequest)


### Example

```typescript
import {
    TagsApi,
    Configuration,
    TagUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new TagsApi(configuration);

let tagId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let tagUpdateRequest: TagUpdateRequest; //

const { status, data } = await apiInstance.updateTag(
    tagId,
    workspaceId,
    tagUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tagUpdateRequest** | **TagUpdateRequest**|  | |
| **tagId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TagResponse**

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

