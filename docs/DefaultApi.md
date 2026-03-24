# DefaultApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getBranding**](#getbranding) | **GET** /v2/settings/branding | Get Branding|
|[**getPublicBranding**](#getpublicbranding) | **GET** /v2/settings/branding/public | Get Public Branding|
|[**updateBranding**](#updatebranding) | **PUT** /v2/settings/branding | Update Branding|

# **getBranding**
> BrandingResponse getBranding()

Get dashboard branding settings for the workspace.

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getBranding(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**BrandingResponse**

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

# **getPublicBranding**
> BrandingResponse getPublicBranding()

Get branding by slug (public, no auth required).

### Example

```typescript
import {
    DefaultApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let slug: string; // (default to undefined)

const { status, data } = await apiInstance.getPublicBranding(
    slug
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | [**string**] |  | defaults to undefined|


### Return type

**BrandingResponse**

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

# **updateBranding**
> BrandingResponse updateBranding(brandingUpdateRequest)

Update dashboard branding settings. Requires white-label addon.

### Example

```typescript
import {
    DefaultApi,
    Configuration,
    BrandingUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

let workspaceId: string; // (default to undefined)
let brandingUpdateRequest: BrandingUpdateRequest; //

const { status, data } = await apiInstance.updateBranding(
    workspaceId,
    brandingUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **brandingUpdateRequest** | **BrandingUpdateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**BrandingResponse**

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

