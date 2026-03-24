# ZendeskChannelApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adminUi**](#adminui) | **POST** /v2/integrations/zendesk_channel/admin_ui | Admin Ui|
|[**channelback**](#channelback) | **POST** /v2/integrations/zendesk_channel/channelback | Channelback|
|[**eventsCallback**](#eventscallback) | **POST** /v2/integrations/zendesk_channel/events | Events Callback|
|[**manifest**](#manifest) | **GET** /v2/integrations/zendesk_channel/manifest.json | Manifest|
|[**messagingWebhook**](#messagingwebhook) | **POST** /v2/integrations/zendesk_channel/messaging_webhook | Messaging Webhook|
|[**messagingWebhookHead**](#messagingwebhookhead) | **HEAD** /v2/integrations/zendesk_channel/messaging_webhook | Messaging Webhook Head|

# **adminUi**
> string adminUi()

Zendesk Channel Framework admin UI callback.  Zendesk sends a URL-encoded form POST with account information.  We persist the push credentials on the matching integration record and return a small HTML page that auto-submits back to Zendesk\'s ``return_url``.

### Example

```typescript
import {
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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

# **eventsCallback**
> any eventsCallback()

Zendesk Channel Framework event callback.  Receives event notifications from Zendesk (e.g. resource lifecycle events).  Logged for debugging and acknowledged with 200 OK.

### Example

```typescript
import {
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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

# **manifest**
> any manifest()

Return the Zendesk Channel Framework manifest.

### Example

```typescript
import {
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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
    ZendeskChannelApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new ZendeskChannelApi(configuration);

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

