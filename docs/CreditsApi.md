# CreditsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCreditBalance**](#getcreditbalance) | **GET** /v2/credits/balance | Get Credit Balance|
|[**getWorkspaceCreditBalance**](#getworkspacecreditbalance) | **GET** /v2/credits/workspace_balance | Get Workspace Credit Balance|
|[**searchCreditTransactions**](#searchcredittransactions) | **POST** /v2/credits/search | Search Credit Transactions|
|[**searchDailyCreditTransactions**](#searchdailycredittransactions) | **POST** /v2/credits/search_daily | Search Daily Credit Transactions|

# **getCreditBalance**
> CreditBalanceResponse getCreditBalance()

Get the credit balance for the current user.

### Example

```typescript
import {
    CreditsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new CreditsApi(configuration);

const { status, data } = await apiInstance.getCreditBalance();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CreditBalanceResponse**

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

# **getWorkspaceCreditBalance**
> CreditBalanceResponse getWorkspaceCreditBalance()

Get the credit balance for a workspace.

### Example

```typescript
import {
    CreditsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new CreditsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWorkspaceCreditBalance(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**CreditBalanceResponse**

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

# **searchCreditTransactions**
> Array<CreditTransactionResponse> searchCreditTransactions(creditTransactionSearchRequest)

Search for credit transactions based on criteria.

### Example

```typescript
import {
    CreditsApi,
    Configuration,
    CreditTransactionSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new CreditsApi(configuration);

let workspaceId: string; // (default to undefined)
let creditTransactionSearchRequest: CreditTransactionSearchRequest; //

const { status, data } = await apiInstance.searchCreditTransactions(
    workspaceId,
    creditTransactionSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **creditTransactionSearchRequest** | **CreditTransactionSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<CreditTransactionResponse>**

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

# **searchDailyCreditTransactions**
> Array<CreditDailyTransactionResponse> searchDailyCreditTransactions(creditDailyTransactionSearchRequest)

Search for daily credit transactions based on criteria.

### Example

```typescript
import {
    CreditsApi,
    Configuration,
    CreditDailyTransactionSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new CreditsApi(configuration);

let workspaceId: string; // (default to undefined)
let creditDailyTransactionSearchRequest: CreditDailyTransactionSearchRequest; //

const { status, data } = await apiInstance.searchDailyCreditTransactions(
    workspaceId,
    creditDailyTransactionSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **creditDailyTransactionSearchRequest** | **CreditDailyTransactionSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<CreditDailyTransactionResponse>**

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

