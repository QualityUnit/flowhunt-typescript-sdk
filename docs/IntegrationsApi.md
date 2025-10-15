# IntegrationsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createIntegration**](#createintegration) | **POST** /v2/integrations/{slug}/integrate | Create Integration|
|[**customerDataRequest**](#customerdatarequest) | **POST** /v2/integrations/shopify/webhooks/customers/data_request | Customer Data Request|
|[**customerRedact**](#customerredact) | **POST** /v2/integrations/shopify/webhooks/customers/redact | Customer Redact|
|[**deleteIntegration**](#deleteintegration) | **DELETE** /v2/integrations/{slug}/{integration_id} | Delete Integration|
|[**getActors**](#getactors) | **GET** /v2/integrations/hubspot/actors/ | Get Actors|
|[**getAllIntegrations**](#getallintegrations) | **GET** /v2/integrations/all | Get All Integrations|
|[**getCalendars**](#getcalendars) | **GET** /v2/integrations/google/calendar | Get Calendars|
|[**getHubspotCustomChannelConnect**](#gethubspotcustomchannelconnect) | **GET** /v2/integrations/hubspot_custom_channel_connect | Get Hubspot Custom Channel Connect|
|[**getIntegration**](#getintegration) | **GET** /v2/integrations/{slug}/{integration_id} | Get Integration|
|[**getPickerToken**](#getpickertoken) | **GET** /v2/integrations/google/picker_token | Get Picker Token|
|[**getProfileInformation**](#getprofileinformation) | **GET** /v2/integrations/instagram/profile_information | Get Profile Information|
|[**getSheets**](#getsheets) | **GET** /v2/integrations/google/sheets/{document_id} | Get Sheets|
|[**getShopify**](#getshopify) | **GET** /v2/integrations/shopify/ | Get Shopify|
|[**getSlackChannels**](#getslackchannels) | **GET** /v2/integrations/slack/{slack_team_id}/channels | Get Slack Channels|
|[**getSlackWorkspaces**](#getslackworkspaces) | **GET** /v2/integrations/slack/ | Get Slack Workspaces|
|[**getWordpressPostCategories**](#getwordpresspostcategories) | **GET** /v2/integrations/wordpress/{integration_id}/categories | Get Wordpress Post Categories|
|[**getWordpressPostTags**](#getwordpressposttags) | **GET** /v2/integrations/wordpress/{integration_id}/tags | Get Wordpress Post Tags|
|[**getWordpressSites**](#getwordpresssites) | **GET** /v2/integrations/wordpress/sites | Get Wordpress Sites|
|[**integrationCallback**](#integrationcallback) | **GET** /v2/integrations/{slug}/callback | Integration Callback|
|[**searchIntegrations**](#searchintegrations) | **POST** /v2/integrations/{slug} | Search Integrations|
|[**shopRedact**](#shopredact) | **POST** /v2/integrations/shopify/webhooks/shop/redact | Shop Redact|
|[**subscriptionCancel**](#subscriptioncancel) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_cancel | Subscription Cancel|
|[**subscriptionUpdate**](#subscriptionupdate) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_update | Subscription Update|
|[**updateAdminConsent**](#updateadminconsent) | **POST** /v2/integrations/microsoft_entra_id/admin_consent | Update Admin Consent|

# **createIntegration**
> IntegrationFlowResponse createIntegration()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slug: IntegrationSlug; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.createIntegration(
    slug,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | **IntegrationSlug** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**IntegrationFlowResponse**

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

# **customerDataRequest**
> any customerDataRequest(customerDataRequestPayload)

Handle customer data request webhooks from Shopify.  This endpoint is called when a customer requests their data from a Shopify store.  Args:     request: The FastAPI request object     payload: The webhook payload  Returns:     A 200 OK response if the webhook is valid and processed successfully

### Example

```typescript
import {
    IntegrationsApi,
    Configuration,
    CustomerDataRequestPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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
    IntegrationsApi,
    Configuration,
    CustomerRedactPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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

# **deleteIntegration**
> Completed deleteIntegration()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slug: IntegrationSlug; // (default to undefined)
let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteIntegration(
    slug,
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | **IntegrationSlug** |  | defaults to undefined|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **getActors**
> HubSpotActorsResponse getActors()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getActors(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**HubSpotActorsResponse**

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

# **getAllIntegrations**
> Array<IntegrationResponse> getAllIntegrations()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAllIntegrations(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<IntegrationResponse>**

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

# **getCalendars**
> GoogleCalendarsResponse getCalendars()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getCalendars(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleCalendarsResponse**

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

# **getHubspotCustomChannelConnect**
> any getHubspotCustomChannelConnect()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.getHubspotCustomChannelConnect();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

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

# **getIntegration**
> IntegrationDetailResponse getIntegration()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slug: IntegrationSlug; // (default to undefined)
let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getIntegration(
    slug,
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | **IntegrationSlug** |  | defaults to undefined|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


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

# **getPickerToken**
> GooglePickerTokenResponse getPickerToken()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getPickerToken(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GooglePickerTokenResponse**

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

# **getProfileInformation**
> InstagramProfileInformationResponse getProfileInformation()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getProfileInformation(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**InstagramProfileInformationResponse**

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

# **getSheets**
> GoogleSheetsResponse getSheets()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let documentId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSheets(
    documentId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleSheetsResponse**

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

# **getShopify**
> ShopifyIntegrationResponse getShopify()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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

# **getSlackChannels**
> Array<SlackChannelResponse> getSlackChannels()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slackTeamId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSlackChannels(
    slackTeamId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slackTeamId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SlackChannelResponse>**

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

# **getSlackWorkspaces**
> Array<SlackWorkspaceResponse> getSlackWorkspaces()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getSlackWorkspaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SlackWorkspaceResponse>**

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

# **getWordpressPostCategories**
> Array<WordPressCategoryResponse> getWordpressPostCategories()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressPostCategories(
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressCategoryResponse>**

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

# **getWordpressPostTags**
> Array<WordPressTagsResponse> getWordpressPostTags()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let integrationId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressPostTags(
    integrationId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressTagsResponse>**

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

# **getWordpressSites**
> Array<WordPressSiteResponse> getWordpressSites()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getWordpressSites(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<WordPressSiteResponse>**

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

# **integrationCallback**
> any integrationCallback()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slug: IntegrationSlug; // (default to undefined)

const { status, data } = await apiInstance.integrationCallback(
    slug
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | **IntegrationSlug** |  | defaults to undefined|


### Return type

**any**

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

# **searchIntegrations**
> Array<IntegrationDetailResponse> searchIntegrations(integrationSearchRequest)


### Example

```typescript
import {
    IntegrationsApi,
    Configuration,
    IntegrationSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let slug: IntegrationSlug; // (default to undefined)
let workspaceId: string; // (default to undefined)
let integrationSearchRequest: IntegrationSearchRequest; //

const { status, data } = await apiInstance.searchIntegrations(
    slug,
    workspaceId,
    integrationSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **integrationSearchRequest** | **IntegrationSearchRequest**|  | |
| **slug** | **IntegrationSlug** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<IntegrationDetailResponse>**

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

# **shopRedact**
> any shopRedact(shopRedactPayload)

Handle shop redact webhooks from Shopify.  This endpoint is called 48 hours after a store owner uninstalls the app.  Args:     request: The FastAPI request object     payload: The webhook payload  Returns:     A 200 OK response if the webhook is valid and processed successfully

### Example

```typescript
import {
    IntegrationsApi,
    Configuration,
    ShopRedactPayload
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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

# **updateAdminConsent**
> IntegrationDetailResponse updateAdminConsent()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

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

