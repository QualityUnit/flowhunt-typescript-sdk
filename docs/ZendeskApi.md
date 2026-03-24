# ZendeskApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**listZendeskKbCategories**](#listzendeskkbcategories) | **GET** /v2/integrations/zendesk/kb/categories | List Zendesk Kb Categories|
|[**listZendeskKbLabels**](#listzendeskkblabels) | **GET** /v2/integrations/zendesk/kb/labels | List Zendesk Kb Labels|
|[**listZendeskKbSections**](#listzendeskkbsections) | **GET** /v2/integrations/zendesk/kb/sections | List Zendesk Kb Sections|

# **listZendeskKbCategories**
> Array<ZendeskKBCategoryResponse> listZendeskKbCategories()


### Example

```typescript
import {
    ZendeskApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskApi(configuration);

let workspaceId: string; // (default to undefined)
let locale: string; //Locale filter (e.g. en-us) (optional) (default to undefined)

const { status, data } = await apiInstance.listZendeskKbCategories(
    workspaceId,
    locale
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **locale** | [**string**] | Locale filter (e.g. en-us) | (optional) defaults to undefined|


### Return type

**Array<ZendeskKBCategoryResponse>**

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

# **listZendeskKbLabels**
> Array<ZendeskKBLabelResponse> listZendeskKbLabels()


### Example

```typescript
import {
    ZendeskApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listZendeskKbLabels(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ZendeskKBLabelResponse>**

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

# **listZendeskKbSections**
> Array<ZendeskKBSectionResponse> listZendeskKbSections()


### Example

```typescript
import {
    ZendeskApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskApi(configuration);

let workspaceId: string; // (default to undefined)
let categoryId: number; //Category ID to filter sections (optional) (default to undefined)

const { status, data } = await apiInstance.listZendeskKbSections(
    workspaceId,
    categoryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **categoryId** | [**number**] | Category ID to filter sections | (optional) defaults to undefined|


### Return type

**Array<ZendeskKBSectionResponse>**

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

