# WordPressApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getWordpressPostCategories**](#getwordpresspostcategories) | **GET** /v2/integrations/wordpress/{integration_id}/categories | Get Wordpress Post Categories|
|[**getWordpressPostTags**](#getwordpressposttags) | **GET** /v2/integrations/wordpress/{integration_id}/tags | Get Wordpress Post Tags|
|[**getWordpressSites**](#getwordpresssites) | **GET** /v2/integrations/wordpress/sites | Get Wordpress Sites|

# **getWordpressPostCategories**
> Array<WordPressCategoryResponse> getWordpressPostCategories()


### Example

```typescript
import {
    WordPressApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WordPressApi(configuration);

let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressPostCategories(
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressCategoryResponse>**

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

# **getWordpressPostTags**
> Array<WordPressTagsResponse> getWordpressPostTags()


### Example

```typescript
import {
    WordPressApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WordPressApi(configuration);

let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressPostTags(
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressTagsResponse>**

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

# **getWordpressSites**
> Array<WordPressSiteResponse> getWordpressSites()


### Example

```typescript
import {
    WordPressApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WordPressApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressSites(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressSiteResponse>**

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

