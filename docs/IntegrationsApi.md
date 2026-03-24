# IntegrationsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adminUi**](#adminui) | **POST** /v2/integrations/zendesk_channel/admin_ui | Admin Ui|
|[**channelback**](#channelback) | **POST** /v2/integrations/zendesk_channel/channelback | Channelback|
|[**createIntegration**](#createintegration) | **POST** /v2/integrations/{slug}/integrate | Create Integration|
|[**customerDataRequest**](#customerdatarequest) | **POST** /v2/integrations/shopify/webhooks/customers/data_request | Customer Data Request|
|[**customerRedact**](#customerredact) | **POST** /v2/integrations/shopify/webhooks/customers/redact | Customer Redact|
|[**deleteIntegration**](#deleteintegration) | **DELETE** /v2/integrations/{slug}/{integration_id} | Delete Integration|
|[**deleteJiraWebhook**](#deletejirawebhook) | **DELETE** /v2/integrations/atlassian/jira/webhooks/{webhook_id} | Delete Jira Webhook|
|[**eventsCallback**](#eventscallback) | **POST** /v2/integrations/zendesk_channel/events | Events Callback|
|[**getActors**](#getactors) | **GET** /v2/integrations/hubspot/actors/ | Get Actors|
|[**getAirtableBases**](#getairtablebases) | **GET** /v2/integrations/airtable/ | Get Airtable Bases|
|[**getAirtableTables**](#getairtabletables) | **GET** /v2/integrations/airtable/bases/{base_id}/tables | Get Airtable Tables|
|[**getAllIntegrations**](#getallintegrations) | **GET** /v2/integrations/all | Get All Integrations|
|[**getBranches**](#getbranches) | **GET** /v2/integrations/gitlab/branches | Get Branches|
|[**getCalendars**](#getcalendars) | **GET** /v2/integrations/google/calendar | Get Calendars|
|[**getClickupSpaces**](#getclickupspaces) | **GET** /v2/integrations/clickup/{integration_id}/spaces | Get Clickup Spaces|
|[**getClickupWorkspaces**](#getclickupworkspaces) | **GET** /v2/integrations/clickup/ | Get Clickup Workspaces|
|[**getConfluencePages**](#getconfluencepages) | **GET** /v2/integrations/atlassian/confluence/spaces/{space_key}/pages | Get Confluence Pages|
|[**getConfluenceSpaces**](#getconfluencespaces) | **GET** /v2/integrations/atlassian/confluence/spaces | Get Confluence Spaces|
|[**getHubspotCustomChannelConnect**](#gethubspotcustomchannelconnect) | **GET** /v2/integrations/hubspot_custom_channel_connect | Get Hubspot Custom Channel Connect|
|[**getIntegration**](#getintegration) | **GET** /v2/integrations/{slug}/{integration_id} | Get Integration|
|[**getJiraAssignees**](#getjiraassignees) | **GET** /v2/integrations/atlassian/jira/projects/{project_key}/assignees | Get Jira Assignees|
|[**getJiraIssues**](#getjiraissues) | **GET** /v2/integrations/atlassian/jira/projects/{project_key}/issues | Get Jira Issues|
|[**getJiraProjects**](#getjiraprojects) | **GET** /v2/integrations/atlassian/jira/projects | Get Jira Projects|
|[**getJiraTransitions**](#getjiratransitions) | **GET** /v2/integrations/atlassian/jira/issues/{issue_key}/transitions | Get Jira Transitions|
|[**getMembers**](#getmembers) | **GET** /v2/integrations/wix/members | Get Members|
|[**getPickerToken**](#getpickertoken) | **GET** /v2/integrations/google/picker_token | Get Picker Token|
|[**getProfileInformation**](#getprofileinformation) | **GET** /v2/integrations/instagram/profile_information | Get Profile Information|
|[**getProjects**](#getprojects) | **GET** /v2/integrations/gitlab/projects | Get Projects|
|[**getRepos**](#getrepos) | **GET** /v2/integrations/github/repos | Get Repos|
|[**getSheets**](#getsheets) | **GET** /v2/integrations/google/sheets/{document_id} | Get Sheets|
|[**getShopify**](#getshopify) | **GET** /v2/integrations/shopify/ | Get Shopify|
|[**getSlackChannels**](#getslackchannels) | **GET** /v2/integrations/slack/{slack_team_id}/channels | Get Slack Channels|
|[**getSlackWorkspaces**](#getslackworkspaces) | **GET** /v2/integrations/slack/ | Get Slack Workspaces|
|[**getWordpressPostCategories**](#getwordpresspostcategories) | **GET** /v2/integrations/wordpress/{integration_id}/categories | Get Wordpress Post Categories|
|[**getWordpressPostTags**](#getwordpressposttags) | **GET** /v2/integrations/wordpress/{integration_id}/tags | Get Wordpress Post Tags|
|[**getWordpressSites**](#getwordpresssites) | **GET** /v2/integrations/wordpress/sites | Get Wordpress Sites|
|[**integrationCallback**](#integrationcallback) | **GET** /v2/integrations/{slug}/callback | Integration Callback|
|[**listJiraWebhooks**](#listjirawebhooks) | **GET** /v2/integrations/atlassian/jira/webhooks | List Jira Webhooks|
|[**listZendeskKbCategories**](#listzendeskkbcategories) | **GET** /v2/integrations/zendesk/kb/categories | List Zendesk Kb Categories|
|[**listZendeskKbLabels**](#listzendeskkblabels) | **GET** /v2/integrations/zendesk/kb/labels | List Zendesk Kb Labels|
|[**listZendeskKbSections**](#listzendeskkbsections) | **GET** /v2/integrations/zendesk/kb/sections | List Zendesk Kb Sections|
|[**manifest**](#manifest) | **GET** /v2/integrations/zendesk_channel/manifest.json | Manifest|
|[**messagingWebhook**](#messagingwebhook) | **POST** /v2/integrations/zendesk_channel/messaging_webhook | Messaging Webhook|
|[**messagingWebhookHead**](#messagingwebhookhead) | **HEAD** /v2/integrations/zendesk_channel/messaging_webhook | Messaging Webhook Head|
|[**searchIntegrations**](#searchintegrations) | **POST** /v2/integrations/{slug} | Search Integrations|
|[**shopRedact**](#shopredact) | **POST** /v2/integrations/shopify/webhooks/shop/redact | Shop Redact|
|[**subscriptionCancel**](#subscriptioncancel) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_cancel | Subscription Cancel|
|[**subscriptionUpdate**](#subscriptionupdate) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_update | Subscription Update|
|[**updateAdminConsent**](#updateadminconsent) | **POST** /v2/integrations/microsoft_entra_id/admin_consent | Update Admin Consent|

# **adminUi**
> string adminUi()

Zendesk Channel Framework admin UI callback.  Zendesk sends a URL-encoded form POST with account information.  We persist the push credentials on the matching integration record and return a small HTML page that auto-submits back to Zendesk\'s ``return_url``.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.adminUi();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/html


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **channelback**
> any channelback()

Zendesk Channel Framework channelback endpoint.  Called by Zendesk when an agent replies to a ticket that was created via the Channel Framework push API.  The agent\'s message is routed back to the originating chat session.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.channelback();
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
let redirectUri: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createIntegration(
    slug,
    workspaceId,
    redirectUri
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **slug** | **IntegrationSlug** |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **redirectUri** | [**string**] |  | (optional) defaults to undefined|


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

# **deleteJiraWebhook**
> deleteJiraWebhook()

Delete a registered Jira webhook by ID.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let webhookId: number; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteJiraWebhook(
    webhookId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhookId** | [**number**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **eventsCallback**
> any eventsCallback()

Zendesk Channel Framework event callback.  Receives event notifications from Zendesk (e.g. resource lifecycle events).  Logged for debugging and acknowledged with 200 OK.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.eventsCallback();
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

# **getAirtableBases**
> AirtableBasesResponse getAirtableBases()

Get all Airtable bases accessible through the workspace\'s Airtable integration.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAirtableBases(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AirtableBasesResponse**

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

# **getAirtableTables**
> AirtableTablesResponse getAirtableTables()

Get all tables for a specific Airtable base.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let baseId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getAirtableTables(
    baseId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **baseId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**AirtableTablesResponse**

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

# **getBranches**
> GitLabBranchesResponse getBranches()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)
let projectId: string; // (default to undefined)

const { status, data } = await apiInstance.getBranches(
    workspaceId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **projectId** | [**string**] |  | defaults to undefined|


### Return type

**GitLabBranchesResponse**

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

# **getClickupSpaces**
> Array<ClickUpSpaceResponse> getClickupSpaces()


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

const { status, data } = await apiInstance.getClickupSpaces(
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

**Array<ClickUpSpaceResponse>**

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

# **getClickupWorkspaces**
> Array<ClickUpWorkspaceResponse> getClickupWorkspaces()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getClickupWorkspaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ClickUpWorkspaceResponse>**

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

# **getConfluencePages**
> ConfluencePagesResponse getConfluencePages()

Get all pages in a Confluence space.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let spaceKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getConfluencePages(
    spaceKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **spaceKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ConfluencePagesResponse**

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

# **getConfluenceSpaces**
> ConfluenceSpacesResponse getConfluenceSpaces()

Get all Confluence spaces accessible through the workspace\'s Atlassian integration.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getConfluenceSpaces(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**ConfluenceSpacesResponse**

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

# **getJiraAssignees**
> JiraAssigneesResponse getJiraAssignees()

Get assignable users for a Jira project.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let projectKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraAssignees(
    projectKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraAssigneesResponse**

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

# **getJiraIssues**
> JiraIssuesResponse getJiraIssues()

Get issues for a Jira project.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let projectKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraIssues(
    projectKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraIssuesResponse**

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

# **getJiraProjects**
> JiraProjectsResponse getJiraProjects()

Get all Jira projects accessible through the workspace\'s Atlassian integration.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraProjects(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraProjectsResponse**

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

# **getJiraTransitions**
> JiraTransitionsResponse getJiraTransitions()

Get available transitions for a Jira issue.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let issueKey: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getJiraTransitions(
    issueKey,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **issueKey** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraTransitionsResponse**

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

# **getMembers**
> WixMembersResponse getMembers()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getMembers(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**WixMembersResponse**

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

# **getProjects**
> GitLabProjectsResponse getProjects()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getProjects(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GitLabProjectsResponse**

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

# **getRepos**
> GitHubReposResponse getRepos()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.getRepos(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GitHubReposResponse**

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

# **listJiraWebhooks**
> JiraWebhooksResponse listJiraWebhooks()

List all registered Jira webhooks for the workspace\'s Atlassian integration.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listJiraWebhooks(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**JiraWebhooksResponse**

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

# **listZendeskKbCategories**
> Array<ZendeskKBCategoryResponse> listZendeskKbCategories()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)
let locale: string; //Locale filter (e.g. en-us) (optional) (default to undefined)

const { status, data } = await apiInstance.listZendeskKbCategories(
    workspaceId,
    locale
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **locale** | [**string**] | Locale filter (e.g. en-us) | (optional) defaults to undefined|


### Return type

**Array<ZendeskKBCategoryResponse>**

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

# **listZendeskKbLabels**
> Array<ZendeskKBLabelResponse> listZendeskKbLabels()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.listZendeskKbLabels(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ZendeskKBLabelResponse>**

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

# **listZendeskKbSections**
> Array<ZendeskKBSectionResponse> listZendeskKbSections()


### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

let workspaceId: string; // (default to undefined)
let categoryId: number; //Category ID to filter sections (optional) (default to undefined)

const { status, data } = await apiInstance.listZendeskKbSections(
    workspaceId,
    categoryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **categoryId** | [**number**] | Category ID to filter sections | (optional) defaults to undefined|


### Return type

**Array<ZendeskKBSectionResponse>**

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

# **manifest**
> any manifest()

Return the Zendesk Channel Framework manifest.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.manifest();
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

# **messagingWebhook**
> any messagingWebhook()

Zendesk Sunshine Conversations (Messaging API) webhook endpoint.  Receives webhook events from the Sunshine Conversations API: - conversation:message -- agent replies to escalated conversations - switchboard:passControl -- control handed back to our bot - switchboard:releaseControl -- agent releases control  Agent messages are routed back to the originating FlowHunt session via the ZendeskAgentReply trigger.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.messagingWebhook();
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

# **messagingWebhookHead**
> any messagingWebhookHead()

Health check endpoint for Zendesk webhook registration.

### Example

```typescript
import {
    IntegrationsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new IntegrationsApi(configuration);

const { status, data } = await apiInstance.messagingWebhookHead();
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

