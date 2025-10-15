# MeApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getUserSettings**](#getusersettings) | **GET** /v2/users/me/settings | Get User Settings|
|[**updateUserSettings**](#updateusersettings) | **PUT** /v2/users/me/settings | Update User Settings|

# **getUserSettings**
> UserSettingsResponse getUserSettings()

Get current user settings with defaults applied.

### Example

```typescript
import {
    MeApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MeApi(configuration);

const { status, data } = await apiInstance.getUserSettings();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserSettingsResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUserSettings**
> UserSettingsResponse updateUserSettings(updateUserSettingsRequest)

Update current user settings (UPSERT operation).

### Example

```typescript
import {
    MeApi,
    Configuration,
    UpdateUserSettingsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MeApi(configuration);

let updateUserSettingsRequest: UpdateUserSettingsRequest; //

const { status, data } = await apiInstance.updateUserSettings(
    updateUserSettingsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUserSettingsRequest** | **UpdateUserSettingsRequest**|  | |


### Return type

**UserSettingsResponse**

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

