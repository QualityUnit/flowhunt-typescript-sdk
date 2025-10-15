# BillingApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addAddonToSubscription**](#addaddontosubscription) | **POST** /v2/billing/addons/{product_id}/add | Add Addon To Subscription|
|[**confirmShopifySubscription**](#confirmshopifysubscription) | **GET** /v2/billing/shopify/confirm | Confirm Shopify Subscription|
|[**createChangePlanPortal**](#createchangeplanportal) | **POST** /v2/billing/portal/change-plan/create | Create Change Plan Portal|
|[**createCheckout**](#createcheckout) | **POST** /v2/billing/checkout/create | Create Checkout|
|[**createUpdateInfoPortal**](#createupdateinfoportal) | **POST** /v2/billing/portal/update-info/create | Create Update Info Portal|
|[**getPricingPlans**](#getpricingplans) | **GET** /v2/billing/plans | Get Pricing Plans|
|[**getUserPlan**](#getuserplan) | **GET** /v2/billing/plans/me | Get User Plan|
|[**stripeWebhook**](#stripewebhook) | **POST** /v2/billing/webhook | Stripe Webhook|

# **addAddonToSubscription**
> string addAddonToSubscription(addOnAddRequest)


### Example

```typescript
import {
    BillingApi,
    Configuration,
    AddOnAddRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

let productId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let addOnAddRequest: AddOnAddRequest; //

const { status, data } = await apiInstance.addAddonToSubscription(
    productId,
    workspaceId,
    addOnAddRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **addOnAddRequest** | **AddOnAddRequest**|  | |
| **productId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **confirmShopifySubscription**
> ShopifySubscriptionConfirmResponse confirmShopifySubscription()

Handle Shopify subscription confirmation redirect. This is the redirect URI after successful purchase of any Shopify plan.  Args:     charge_id: The charge ID from Shopify (query parameter)     shop: The shop domain (query parameter)  Returns:     ShopifySubscriptionConfirmResponse with subscription details

### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

let chargeId: string; // (default to undefined)
let shop: string; // (default to undefined)

const { status, data } = await apiInstance.confirmShopifySubscription(
    chargeId,
    shop
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **chargeId** | [**string**] |  | defaults to undefined|
| **shop** | [**string**] |  | defaults to undefined|


### Return type

**ShopifySubscriptionConfirmResponse**

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

# **createChangePlanPortal**
> any createChangePlanPortal()


### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

const { status, data } = await apiInstance.createChangePlanPortal();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createCheckout**
> string createCheckout(checkoutCreateRequest)


### Example

```typescript
import {
    BillingApi,
    Configuration,
    CheckoutCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

let checkoutCreateRequest: CheckoutCreateRequest; //

const { status, data } = await apiInstance.createCheckout(
    checkoutCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **checkoutCreateRequest** | **CheckoutCreateRequest**|  | |


### Return type

**string**

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

# **createUpdateInfoPortal**
> string createUpdateInfoPortal()


### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

const { status, data } = await apiInstance.createUpdateInfoPortal();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**string**

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

# **getPricingPlans**
> PlanResponse getPricingPlans()


### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

const { status, data } = await apiInstance.getPricingPlans();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**PlanResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserPlan**
> UserPlanResponse getUserPlan()


### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getUserPlan(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**UserPlanResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **stripeWebhook**
> Completed stripeWebhook()


### Example

```typescript
import {
    BillingApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new BillingApi(configuration);

const { status, data } = await apiInstance.stripeWebhook();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Completed**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

