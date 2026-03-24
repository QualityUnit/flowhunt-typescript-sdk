# HubSpotApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getActors**](#getactors) | **GET** /v2/integrations/hubspot/actors/ | Get Actors|

# **getActors**
> HubSpotActorsResponse getActors()


### Example

```typescript
import {
    HubSpotApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new HubSpotApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getActors(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**HubSpotActorsResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

