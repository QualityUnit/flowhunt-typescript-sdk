# MicrosoftOutlookApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**updateAdminConsent**](#updateadminconsent) | **POST** /v2/integrations/microsoft_entra_id/admin_consent | Update Admin Consent|

# **updateAdminConsent**
> IntegrationDetailResponse updateAdminConsent()


### Example

```typescript
import {
    MicrosoftOutlookApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new MicrosoftOutlookApi(configuration);

let workspaceId: string; // (default to undefined)
let integrationId: string; // (default to undefined)

const { status, data } = await apiInstance.updateAdminConsent(
    workspaceId,
    integrationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **integrationId** | [**string**] |  | defaults to undefined|


### Return type

**IntegrationDetailResponse**

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

