# ObservabilityDriverApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**activateLangfuseObservabilityDriver**](#activatelangfuseobservabilitydriver) | **POST** /v2/observability_driver/langfuse | Activate Langfuse Observability Driver|
|[**activatePowerBiObservabilityDriver**](#activatepowerbiobservabilitydriver) | **POST** /v2/observability_driver/power_bi | Activate Power Bi Observability Driver|
|[**createPowerBiPushDataset**](#createpowerbipushdataset) | **POST** /v2/observability_driver/power_bi/push_dataset | Create Power Bi Push Dataset|
|[**deleteObservabilityDriver**](#deleteobservabilitydriver) | **DELETE** /v2/observability_driver/{driver_type} | Delete Observability Driver|
|[**getObservabilityDriver**](#getobservabilitydriver) | **GET** /v2/observability_driver/{driver_type} | Get Observability Driver|
|[**getObservabilityDriverWorkspace**](#getobservabilitydriverworkspace) | **POST** /v2/observability_driver/ | Get Observability Driver Workspace|
|[**listPowerBiDatasets**](#listpowerbidatasets) | **POST** /v2/observability_driver/power_bi/datasets | List Power Bi Datasets|
|[**listPowerBiTables**](#listpowerbitables) | **POST** /v2/observability_driver/power_bi/tables | List Power Bi Tables|
|[**listPowerBiWorkspaces**](#listpowerbiworkspaces) | **GET** /v2/observability_driver/power_bi/workspaces | List Power Bi Workspaces|
|[**updateLangfuseObservabilityDriver**](#updatelangfuseobservabilitydriver) | **PUT** /v2/observability_driver/langfuse | Update Langfuse Observability Driver|
|[**updatePowerBiObservabilityDriver**](#updatepowerbiobservabilitydriver) | **PUT** /v2/observability_driver/power_bi | Update Power Bi Observability Driver|
|[**validatePushDatasetTable**](#validatepushdatasettable) | **POST** /v2/observability_driver/power_bi/validate_push_dataset | Validate Push Dataset Table|

# **activateLangfuseObservabilityDriver**
> ObservabilityDriverResponse activateLangfuseObservabilityDriver(langfuseRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    LangfuseRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let langfuseRequest: LangfuseRequest; //

const { status, data } = await apiInstance.activateLangfuseObservabilityDriver(
    workspaceId,
    langfuseRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **langfuseRequest** | **LangfuseRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ObservabilityDriverResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activatePowerBiObservabilityDriver**
> ObservabilityDriverResponse activatePowerBiObservabilityDriver(powerBiRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiRequest: PowerBiRequest; //

const { status, data } = await apiInstance.activatePowerBiObservabilityDriver(
    workspaceId,
    powerBiRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiRequest** | **PowerBiRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ObservabilityDriverResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createPowerBiPushDataset**
> MicrosoftPowerBiPushDatasetResponse createPowerBiPushDataset(powerBiPushDatasetRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiPushDatasetRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiPushDatasetRequest: PowerBiPushDatasetRequest; //

const { status, data } = await apiInstance.createPowerBiPushDataset(
    workspaceId,
    powerBiPushDatasetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiPushDatasetRequest** | **PowerBiPushDatasetRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MicrosoftPowerBiPushDatasetResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteObservabilityDriver**
> DriverSuccessResponse deleteObservabilityDriver()


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let driverType: DriverType; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteObservabilityDriver(
    driverType,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **driverType** | **DriverType** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DriverSuccessResponse**

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

# **getObservabilityDriver**
> ObservabilityDriverResponse getObservabilityDriver()


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let driverType: DriverType; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getObservabilityDriver(
    driverType,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **driverType** | **DriverType** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ObservabilityDriverResponse**

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

# **getObservabilityDriverWorkspace**
> Array<ObservabilityDriverResponse> getObservabilityDriverWorkspace()


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getObservabilityDriverWorkspace(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ObservabilityDriverResponse>**

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

# **listPowerBiDatasets**
> MicrosoftPowerBiDatasetsResponse listPowerBiDatasets(powerBiDatasetRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiDatasetRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiDatasetRequest: PowerBiDatasetRequest; //

const { status, data } = await apiInstance.listPowerBiDatasets(
    workspaceId,
    powerBiDatasetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiDatasetRequest** | **PowerBiDatasetRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MicrosoftPowerBiDatasetsResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listPowerBiTables**
> MicrosoftPowerBiTablesResponse listPowerBiTables(powerBiTableRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiTableRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiTableRequest: PowerBiTableRequest; //

const { status, data } = await apiInstance.listPowerBiTables(
    workspaceId,
    powerBiTableRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiTableRequest** | **PowerBiTableRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MicrosoftPowerBiTablesResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listPowerBiWorkspaces**
> MicrosoftPowerBiWorkspacesResponse listPowerBiWorkspaces()


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listPowerBiWorkspaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MicrosoftPowerBiWorkspacesResponse**

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

# **updateLangfuseObservabilityDriver**
> ObservabilityDriverResponse updateLangfuseObservabilityDriver(langfuseRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    LangfuseRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let langfuseRequest: LangfuseRequest; //

const { status, data } = await apiInstance.updateLangfuseObservabilityDriver(
    workspaceId,
    langfuseRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **langfuseRequest** | **LangfuseRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ObservabilityDriverResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updatePowerBiObservabilityDriver**
> ObservabilityDriverResponse updatePowerBiObservabilityDriver(powerBiRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiRequest: PowerBiRequest; //

const { status, data } = await apiInstance.updatePowerBiObservabilityDriver(
    workspaceId,
    powerBiRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiRequest** | **PowerBiRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ObservabilityDriverResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validatePushDatasetTable**
> MicrosoftPowerBiTableValidateResponse validatePushDatasetTable(powerBiRequest)


### Example

```typescript
import {
    ObservabilityDriverApi,
    Configuration,
    PowerBiRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ObservabilityDriverApi(configuration);

let workspaceId: string; // (default to undefined)
let powerBiRequest: PowerBiRequest; //

const { status, data } = await apiInstance.validatePushDatasetTable(
    workspaceId,
    powerBiRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **powerBiRequest** | **PowerBiRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**MicrosoftPowerBiTableValidateResponse**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

