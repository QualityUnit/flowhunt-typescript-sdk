# FlowBatchApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addRows**](#addrows) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows | Add Rows|
|[**addRows_0**](#addrows_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows | Add Rows|
|[**createBatchRun**](#createbatchrun) | **POST** /v2/flows/{flow_id}/batch | Create Batch Run|
|[**createBatchRun_0**](#createbatchrun_0) | **POST** /v2/flows/{flow_id}/batch | Create Batch Run|
|[**deleteBatchRun**](#deletebatchrun) | **DELETE** /v2/flows/{flow_id}/batch/{batch_run_id} | Delete Batch Run|
|[**deleteBatchRun_0**](#deletebatchrun_0) | **DELETE** /v2/flows/{flow_id}/batch/{batch_run_id} | Delete Batch Run|
|[**deleteRow**](#deleterow) | **DELETE** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id} | Delete Row|
|[**deleteRow_0**](#deleterow_0) | **DELETE** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id} | Delete Row|
|[**executeBatch**](#executebatch) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/execute | Execute Batch|
|[**executeBatch_0**](#executebatch_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/execute | Execute Batch|
|[**executeFiltered**](#executefiltered) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/execute-filtered | Execute Filtered|
|[**executeFiltered_0**](#executefiltered_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/execute-filtered | Execute Filtered|
|[**executeRow**](#executerow) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id}/execute | Execute Row|
|[**executeRow_0**](#executerow_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id}/execute | Execute Row|
|[**exportCsv**](#exportcsv) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id}/export-csv | Export Csv|
|[**exportCsv_0**](#exportcsv_0) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id}/export-csv | Export Csv|
|[**getBatchRun**](#getbatchrun) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id} | Get Batch Run|
|[**getBatchRun_0**](#getbatchrun_0) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id} | Get Batch Run|
|[**getExportZipStatus**](#getexportzipstatus) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id}/export-zip/{task_id} | Get Export Zip Status|
|[**getExportZipStatus_0**](#getexportzipstatus_0) | **GET** /v2/flows/{flow_id}/batch/{batch_run_id}/export-zip/{task_id} | Get Export Zip Status|
|[**importCsv**](#importcsv) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/import-csv | Import Csv|
|[**importCsv_0**](#importcsv_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/import-csv | Import Csv|
|[**listBatchRuns**](#listbatchruns) | **GET** /v2/flows/{flow_id}/batch | List Batch Runs|
|[**listBatchRuns_0**](#listbatchruns_0) | **GET** /v2/flows/{flow_id}/batch | List Batch Runs|
|[**startExportZip**](#startexportzip) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/export-zip | Start Export Zip|
|[**startExportZip_0**](#startexportzip_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/export-zip | Start Export Zip|
|[**stopAllRows**](#stopallrows) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/stop-all | Stop All Rows|
|[**stopAllRows_0**](#stopallrows_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/stop-all | Stop All Rows|
|[**stopRow**](#stoprow) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id}/stop | Stop Row|
|[**stopRow_0**](#stoprow_0) | **POST** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id}/stop | Stop Row|
|[**updateBatchRun**](#updatebatchrun) | **PUT** /v2/flows/{flow_id}/batch/{batch_run_id} | Update Batch Run|
|[**updateBatchRun_0**](#updatebatchrun_0) | **PUT** /v2/flows/{flow_id}/batch/{batch_run_id} | Update Batch Run|
|[**updateRow**](#updaterow) | **PUT** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id} | Update Row|
|[**updateRow_0**](#updaterow_0) | **PUT** /v2/flows/{flow_id}/batch/{batch_run_id}/rows/{row_id} | Update Row|

# **addRows**
> Array<FlowBatchRowResponse> addRows(flowBatchRowsBulkCreateRequest)

Add one or more rows to a batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRowsBulkCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRowsBulkCreateRequest: FlowBatchRowsBulkCreateRequest; //

const { status, data } = await apiInstance.addRows(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchRowsBulkCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRowsBulkCreateRequest** | **FlowBatchRowsBulkCreateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowBatchRowResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **addRows_0**
> Array<FlowBatchRowResponse> addRows_0(flowBatchRowsBulkCreateRequest)

Add one or more rows to a batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRowsBulkCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRowsBulkCreateRequest: FlowBatchRowsBulkCreateRequest; //

const { status, data } = await apiInstance.addRows_0(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchRowsBulkCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRowsBulkCreateRequest** | **FlowBatchRowsBulkCreateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FlowBatchRowResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createBatchRun**
> FlowBatchRunResponse createBatchRun(flowBatchRunCreateRequest)

Create a new batch run for a flow.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRunCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRunCreateRequest: FlowBatchRunCreateRequest; //

const { status, data } = await apiInstance.createBatchRun(
    flowId,
    workspaceId,
    flowBatchRunCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRunCreateRequest** | **FlowBatchRunCreateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createBatchRun_0**
> FlowBatchRunResponse createBatchRun_0(flowBatchRunCreateRequest)

Create a new batch run for a flow.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRunCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRunCreateRequest: FlowBatchRunCreateRequest; //

const { status, data } = await apiInstance.createBatchRun_0(
    flowId,
    workspaceId,
    flowBatchRunCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRunCreateRequest** | **FlowBatchRunCreateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteBatchRun**
> Completed deleteBatchRun()

Delete a batch run and all its rows.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteBatchRun(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
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

# **deleteBatchRun_0**
> Completed deleteBatchRun_0()

Delete a batch run and all its rows.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteBatchRun_0(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
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

# **deleteRow**
> Completed deleteRow()

Delete a row from a batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteRow(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
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

# **deleteRow_0**
> Completed deleteRow_0()

Delete a row from a batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteRow_0(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
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

# **executeBatch**
> FlowBatchRunResponse executeBatch()

Execute pending rows (or all non-running rows when rerun_all=true) in the batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let rerunAll: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.executeBatch(
    flowId,
    batchRunId,
    workspaceId,
    rerunAll
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **rerunAll** | [**boolean**] |  | (optional) defaults to false|


### Return type

**FlowBatchRunResponse**

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

# **executeBatch_0**
> FlowBatchRunResponse executeBatch_0()

Execute pending rows (or all non-running rows when rerun_all=true) in the batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let rerunAll: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.executeBatch_0(
    flowId,
    batchRunId,
    workspaceId,
    rerunAll
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **rerunAll** | [**boolean**] |  | (optional) defaults to false|


### Return type

**FlowBatchRunResponse**

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

# **executeFiltered**
> FlowBatchRunResponse executeFiltered(flowBatchFilteredExecuteRequest)

Execute rows matching an optional search filter.  - ``rerun_all=false`` — run only **pending** rows matching the filter. - ``rerun_all=true``  — reset matching completed/failed rows to pending,   then run them. - ``max_concurrency`` — optional override for ``max_parallel`` (capped by   the subscription plan limit).

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchFilteredExecuteRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchFilteredExecuteRequest: FlowBatchFilteredExecuteRequest; //

const { status, data } = await apiInstance.executeFiltered(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchFilteredExecuteRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchFilteredExecuteRequest** | **FlowBatchFilteredExecuteRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

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

# **executeFiltered_0**
> FlowBatchRunResponse executeFiltered_0(flowBatchFilteredExecuteRequest)

Execute rows matching an optional search filter.  - ``rerun_all=false`` — run only **pending** rows matching the filter. - ``rerun_all=true``  — reset matching completed/failed rows to pending,   then run them. - ``max_concurrency`` — optional override for ``max_parallel`` (capped by   the subscription plan limit).

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchFilteredExecuteRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchFilteredExecuteRequest: FlowBatchFilteredExecuteRequest; //

const { status, data } = await apiInstance.executeFiltered_0(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchFilteredExecuteRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchFilteredExecuteRequest** | **FlowBatchFilteredExecuteRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

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

# **executeRow**
> FlowBatchRowResponse executeRow()

Execute a single row in the batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.executeRow(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

# **executeRow_0**
> FlowBatchRowResponse executeRow_0()

Execute a single row in the batch run.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.executeRow_0(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

# **exportCsv**
> any exportCsv()

Export batch results as CSV.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.exportCsv(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**any**

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

# **exportCsv_0**
> any exportCsv_0()

Export batch results as CSV.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.exportCsv_0(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**any**

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

# **getBatchRun**
> FlowBatchRunDetailResponse getBatchRun()

Get batch run details with cursor-based paginated rows.  Use ``rows_cursor`` (the ``next_cursor`` from a previous response) to fetch subsequent pages.  ``rows_status`` filters rows by their execution status.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let rowsLimit: number; // (optional) (default to 50)
let rowsCursor: number; // (optional) (default to undefined)
let rowsStatus: FlowBatchRowStatus; // (optional) (default to undefined)

const { status, data } = await apiInstance.getBatchRun(
    flowId,
    batchRunId,
    workspaceId,
    rowsLimit,
    rowsCursor,
    rowsStatus
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **rowsLimit** | [**number**] |  | (optional) defaults to 50|
| **rowsCursor** | [**number**] |  | (optional) defaults to undefined|
| **rowsStatus** | **FlowBatchRowStatus** |  | (optional) defaults to undefined|


### Return type

**FlowBatchRunDetailResponse**

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

# **getBatchRun_0**
> FlowBatchRunDetailResponse getBatchRun_0()

Get batch run details with cursor-based paginated rows.  Use ``rows_cursor`` (the ``next_cursor`` from a previous response) to fetch subsequent pages.  ``rows_status`` filters rows by their execution status.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let rowsLimit: number; // (optional) (default to 50)
let rowsCursor: number; // (optional) (default to undefined)
let rowsStatus: FlowBatchRowStatus; // (optional) (default to undefined)

const { status, data } = await apiInstance.getBatchRun_0(
    flowId,
    batchRunId,
    workspaceId,
    rowsLimit,
    rowsCursor,
    rowsStatus
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **rowsLimit** | [**number**] |  | (optional) defaults to 50|
| **rowsCursor** | [**number**] |  | (optional) defaults to undefined|
| **rowsStatus** | **FlowBatchRowStatus** |  | (optional) defaults to undefined|


### Return type

**FlowBatchRunDetailResponse**

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

# **getExportZipStatus**
> TaskResponse getExportZipStatus()

Poll the status of a batch ZIP export task. Returns a presigned URL on success.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let taskId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getExportZipStatus(
    flowId,
    batchRunId,
    taskId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **taskId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **getExportZipStatus_0**
> TaskResponse getExportZipStatus_0()

Poll the status of a batch ZIP export task. Returns a presigned URL on success.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let taskId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getExportZipStatus_0(
    flowId,
    batchRunId,
    taskId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **taskId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **importCsv**
> FlowBatchRunDetailResponse importCsv()

Import CSV file to populate batch rows.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: string; // (default to undefined)

const { status, data } = await apiInstance.importCsv(
    flowId,
    batchRunId,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunDetailResponse**

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

# **importCsv_0**
> FlowBatchRunDetailResponse importCsv_0()

Import CSV file to populate batch rows.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: string; // (default to undefined)

const { status, data } = await apiInstance.importCsv_0(
    flowId,
    batchRunId,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunDetailResponse**

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

# **listBatchRuns**
> Array<FlowBatchRunResponse> listBatchRuns()

List all batch runs for a flow.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let limit: number; // (optional) (default to 50)
let offset: number; // (optional) (default to 0)

const { status, data } = await apiInstance.listBatchRuns(
    flowId,
    workspaceId,
    limit,
    offset
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 50|
| **offset** | [**number**] |  | (optional) defaults to 0|


### Return type

**Array<FlowBatchRunResponse>**

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

# **listBatchRuns_0**
> Array<FlowBatchRunResponse> listBatchRuns_0()

List all batch runs for a flow.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let limit: number; // (optional) (default to 50)
let offset: number; // (optional) (default to 0)

const { status, data } = await apiInstance.listBatchRuns_0(
    flowId,
    workspaceId,
    limit,
    offset
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 50|
| **offset** | [**number**] |  | (optional) defaults to 0|


### Return type

**Array<FlowBatchRunResponse>**

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

# **startExportZip**
> TaskResponse startExportZip()

Start an async batch ZIP export. Returns a task ID for polling.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.startExportZip(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **startExportZip_0**
> TaskResponse startExportZip_0()

Start an async batch ZIP export. Returns a task ID for polling.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.startExportZip_0(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **stopAllRows**
> Completed stopAllRows()

Stop all running rows in a batch run, resetting them to pending.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.stopAllRows(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
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

# **stopAllRows_0**
> Completed stopAllRows_0()

Stop all running rows in a batch run, resetting them to pending.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.stopAllRows_0(
    flowId,
    batchRunId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
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

# **stopRow**
> FlowBatchRowResponse stopRow()

Stop a running row and reset it to pending status.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.stopRow(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

# **stopRow_0**
> FlowBatchRowResponse stopRow_0()

Stop a running row and reset it to pending status.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.stopRow_0(
    flowId,
    batchRunId,
    rowId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

# **updateBatchRun**
> FlowBatchRunResponse updateBatchRun(flowBatchRunUpdateRequest)

Update batch run metadata.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRunUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRunUpdateRequest: FlowBatchRunUpdateRequest; //

const { status, data } = await apiInstance.updateBatchRun(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchRunUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRunUpdateRequest** | **FlowBatchRunUpdateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

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

# **updateBatchRun_0**
> FlowBatchRunResponse updateBatchRun_0(flowBatchRunUpdateRequest)

Update batch run metadata.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRunUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRunUpdateRequest: FlowBatchRunUpdateRequest; //

const { status, data } = await apiInstance.updateBatchRun_0(
    flowId,
    batchRunId,
    workspaceId,
    flowBatchRunUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRunUpdateRequest** | **FlowBatchRunUpdateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRunResponse**

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

# **updateRow**
> FlowBatchRowResponse updateRow(flowBatchRowUpdateRequest)

Update a row\'s input data.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRowUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRowUpdateRequest: FlowBatchRowUpdateRequest; //

const { status, data } = await apiInstance.updateRow(
    flowId,
    batchRunId,
    rowId,
    workspaceId,
    flowBatchRowUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRowUpdateRequest** | **FlowBatchRowUpdateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

# **updateRow_0**
> FlowBatchRowResponse updateRow_0(flowBatchRowUpdateRequest)

Update a row\'s input data.

### Example

```typescript
import {
    FlowBatchApi,
    Configuration,
    FlowBatchRowUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new FlowBatchApi(configuration);

let flowId: string; // (default to undefined)
let batchRunId: string; // (default to undefined)
let rowId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let flowBatchRowUpdateRequest: FlowBatchRowUpdateRequest; //

const { status, data } = await apiInstance.updateRow_0(
    flowId,
    batchRunId,
    rowId,
    workspaceId,
    flowBatchRowUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **flowBatchRowUpdateRequest** | **FlowBatchRowUpdateRequest**|  | |
| **flowId** | [**string**] |  | defaults to undefined|
| **batchRunId** | [**string**] |  | defaults to undefined|
| **rowId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**FlowBatchRowResponse**

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

