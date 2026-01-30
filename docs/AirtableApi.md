# AirtableApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAirtableBases**](#getairtablebases) | **GET** /v2/integrations/airtable/ | Get Airtable Bases|
|[**getAirtableTables**](#getairtabletables) | **GET** /v2/integrations/airtable/bases/{base_id}/tables | Get Airtable Tables|

# **getAirtableBases**
> AirtableBasesResponse getAirtableBases()

Get all Airtable bases accessible through the workspace\'s Airtable integration.

### Example

```typescript
import {
    AirtableApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AirtableApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAirtableBases(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AirtableBasesResponse**

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

# **getAirtableTables**
> AirtableTablesResponse getAirtableTables()

Get all tables for a specific Airtable base.

### Example

```typescript
import {
    AirtableApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new AirtableApi(configuration);

let baseId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAirtableTables(
    baseId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **baseId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AirtableTablesResponse**

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

