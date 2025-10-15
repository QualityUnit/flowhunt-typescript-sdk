# WorkspacesSSODomainVerificationApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDomainVerification**](#createdomainverification) | **POST** /v2/workspaces/{workspace_id}/sso/domain-verification | Create Domain Verification|
|[**deleteDomainVerification**](#deletedomainverification) | **DELETE** /v2/workspaces/{workspace_id}/sso/domain-verification | Delete Domain Verification|
|[**listDomainVerifications**](#listdomainverifications) | **GET** /v2/workspaces/{workspace_id}/sso/domain-verification | List Domain Verifications|
|[**verifyDomain**](#verifydomain) | **POST** /v2/workspaces/{workspace_id}/sso/domain-verification/verify | Verify Domain|

# **createDomainVerification**
> WorkspaceSSODomainVerificationResponse createDomainVerification(workspaceSSODomainVerificationCreateRequest)

Create a new domain verification record. Admin endpoint - requires workspace admin permissions. Enterprise feature - requires enterprise subscription.

### Example

```typescript
import {
    WorkspacesSSODomainVerificationApi,
    Configuration,
    WorkspaceSSODomainVerificationCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSODomainVerificationApi(configuration);

let workspaceId: string; // (default to undefined)
let workspaceSSODomainVerificationCreateRequest: WorkspaceSSODomainVerificationCreateRequest; //

const { status, data } = await apiInstance.createDomainVerification(
    workspaceId,
    workspaceSSODomainVerificationCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceSSODomainVerificationCreateRequest** | **WorkspaceSSODomainVerificationCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSODomainVerificationResponse**

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

# **deleteDomainVerification**
> Completed deleteDomainVerification()

Delete a domain verification record. Admin endpoint - requires workspace admin permissions. Enterprise feature - requires enterprise subscription.

### Example

```typescript
import {
    WorkspacesSSODomainVerificationApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSODomainVerificationApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteDomainVerification(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
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

# **listDomainVerifications**
> Array<WorkspaceSSODomainVerificationResponse> listDomainVerifications()

List all domain verifications for a workspace. Admin endpoint - requires workspace admin permissions. Enterprise feature - requires enterprise subscription.

### Example

```typescript
import {
    WorkspacesSSODomainVerificationApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSODomainVerificationApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listDomainVerifications(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WorkspaceSSODomainVerificationResponse>**

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

# **verifyDomain**
> WorkspaceSSODomainVerificationResponse verifyDomain()

Verify a domain by checking DNS TXT records. Admin endpoint - requires workspace admin permissions. Enterprise feature - requires enterprise subscription.

### Example

```typescript
import {
    WorkspacesSSODomainVerificationApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WorkspacesSSODomainVerificationApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.verifyDomain(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WorkspaceSSODomainVerificationResponse**

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

