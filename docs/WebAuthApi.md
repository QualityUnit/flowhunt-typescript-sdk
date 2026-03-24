# WebAuthApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getUser**](#getuser) | **GET** /v2/auth/me | Get User|

# **getUser**
> UserResponse getUser()

Get current authenticated user details.  This endpoint returns the current user\'s details including their product plans and API key workspace information. It follows DDD principles by delegating the business logic to the application service layer.  Args:     user: The current authenticated user (injected by dependency)     request: The HTTP request object     user_service: The user application service (injected by dependency)  Returns:     UserResponse: The user details response

### Example

```typescript
import {
    WebAuthApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new WebAuthApi(configuration);

const { status, data } = await apiInstance.getUser();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserResponse**

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

