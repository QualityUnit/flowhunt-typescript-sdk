# WixApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getMembers**](#getmembers) | **GET** /v2/integrations/wix/members | Get Members|

# **getMembers**
> WixMembersResponse getMembers()


### Example

```typescript
import {
    WixApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WixApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getMembers(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WixMembersResponse**

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

