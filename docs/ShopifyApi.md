# ShopifyApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**customerDataRequest**](#customerdatarequest) | **POST** /v2/integrations/shopify/webhooks/customers/data_request | Customer Data Request|
|[**customerRedact**](#customerredact) | **POST** /v2/integrations/shopify/webhooks/customers/redact | Customer Redact|
|[**getShopify**](#getshopify) | **GET** /v2/integrations/shopify/ | Get Shopify|
|[**shopRedact**](#shopredact) | **POST** /v2/integrations/shopify/webhooks/shop/redact | Shop Redact|
|[**subscriptionCancel**](#subscriptioncancel) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_cancel | Subscription Cancel|
|[**subscriptionUpdate**](#subscriptionupdate) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_update | Subscription Update|

# **customerDataRequest**
> any customerDataRequest(customerDataRequestPayload)

Handle customer data request webhooks from Shopify.  This endpoint is called when a customer requests their data from a Shopify store.  Args:     request: The FastAPI request object     payload: The webhook payload  Returns:     A 200 OK response if the webhook is valid and processed successfully

### Example

```typescript
import {
    ShopifyApi,
    Configuration,
    CustomerDataRequestPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let customerDataRequestPayload: CustomerDataRequestPayload; //

const { status, data } = await apiInstance.customerDataRequest(
    customerDataRequestPayload
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerDataRequestPayload** | **CustomerDataRequestPayload**|  | |


### Return type

**any**

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

# **customerRedact**
> any customerRedact(customerRedactPayload)

Handle customer redact webhooks from Shopify.  This endpoint is called when a customer requests their data to be deleted from a Shopify store.  Args:     request: The FastAPI request object     payload: The webhook payload  Returns:     A 200 OK response if the webhook is valid and processed successfully

### Example

```typescript
import {
    ShopifyApi,
    Configuration,
    CustomerRedactPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let customerRedactPayload: CustomerRedactPayload; //

const { status, data } = await apiInstance.customerRedact(
    customerRedactPayload
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerRedactPayload** | **CustomerRedactPayload**|  | |


### Return type

**any**

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

# **getShopify**
> ShopifyIntegrationResponse getShopify()


### Example

```typescript
import {
    ShopifyApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getShopify(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ShopifyIntegrationResponse**

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

# **shopRedact**
> any shopRedact(shopRedactPayload)

Handle shop redact webhooks from Shopify.  This endpoint is called 48 hours after a store owner uninstalls the app.  Args:     request: The FastAPI request object     payload: The webhook payload  Returns:     A 200 OK response if the webhook is valid and processed successfully

### Example

```typescript
import {
    ShopifyApi,
    Configuration,
    ShopRedactPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let shopRedactPayload: ShopRedactPayload; //

const { status, data } = await apiInstance.shopRedact(
    shopRedactPayload
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **shopRedactPayload** | **ShopRedactPayload**|  | |


### Return type

**any**

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

# **subscriptionCancel**
> any subscriptionCancel()

Handle subscription cancellation webhooks from Shopify.

### Example

```typescript
import {
    ShopifyApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let xShopifyHmacSha256: string; // (optional) (default to undefined)
let xShopifyTopic: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.subscriptionCancel(
    xShopifyHmacSha256,
    xShopifyTopic
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **xShopifyHmacSha256** | [**string**] |  | (optional) defaults to undefined|
| **xShopifyTopic** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

# **subscriptionUpdate**
> any subscriptionUpdate()

Handle subscription update webhooks from Shopify.  This is called when a subscription is created, updated, or activated.

### Example

```typescript
import {
    ShopifyApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ShopifyApi(configuration);

let xShopifyHmacSha256: string; // (optional) (default to undefined)
let xShopifyTopic: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.subscriptionUpdate(
    xShopifyHmacSha256,
    xShopifyTopic
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **xShopifyHmacSha256** | [**string**] |  | (optional) defaults to undefined|
| **xShopifyTopic** | [**string**] |  | (optional) defaults to undefined|


### Return type

**any**

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

