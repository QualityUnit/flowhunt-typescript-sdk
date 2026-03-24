# GoogleAdsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addKeywordToGroup**](#addkeywordtogroup) | **POST** /v2/integrations/google_ads/keyword/add_to_group | Add Keyword To Group|
|[**analyzeNotAssignedKeywords**](#analyzenotassignedkeywords) | **POST** /v2/integrations/google_ads/analyze_not_assigned_keywords | Analyze Not Assigned Keywords|
|[**getGoogleAdsCampaigns**](#getgoogleadscampaigns) | **POST** /v2/integrations/google_ads/campaigns | Get Google Ads Campaigns|
|[**getGoogleAdsCustomers**](#getgoogleadscustomers) | **POST** /v2/integrations/google_ads/customers | Get Google Ads Customers|
|[**getGoogleAdsGroups**](#getgoogleadsgroups) | **POST** /v2/integrations/google_ads/groups | Get Google Ads Groups|
|[**getRecommendations**](#getrecommendations) | **POST** /v2/integrations/google_ads/recommendations/ | Get Recommendations|
|[**importGoogleAdsCampaigns**](#importgoogleadscampaigns) | **POST** /v2/integrations/google_ads/campaigns/import | Import Google Ads Campaigns|
|[**importGoogleAdsCustomers**](#importgoogleadscustomers) | **POST** /v2/integrations/google_ads/customers/import | Import Google Ads Customers|
|[**importGoogleAdsGroups**](#importgoogleadsgroups) | **POST** /v2/integrations/google_ads/groups/import | Import Google Ads Groups|
|[**removeKeywordFromGroup**](#removekeywordfromgroup) | **POST** /v2/integrations/google_ads/keyword/remove_from_group | Remove Keyword From Group|
|[**updateGoogleAdsCampaign**](#updategoogleadscampaign) | **PUT** /v2/integrations/google_ads/campaigns/{customer_id}/{campaign_id} | Update Google Ads Campaign|
|[**updateGoogleAdsCustomerUpdate**](#updategoogleadscustomerupdate) | **PUT** /v2/integrations/google_ads/customers/{customer_id} | Update Google Ads Customer Update|
|[**updateGoogleAdsGroup**](#updategoogleadsgroup) | **PUT** /v2/integrations/google_ads/groups/{customer_id}/{campaign_id}/{group_id} | Update Google Ads Group|

# **addKeywordToGroup**
> Completed addKeywordToGroup(googleAdsKeywordAddRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsKeywordAddRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsKeywordAddRequest: GoogleAdsKeywordAddRequest; //

const { status, data } = await apiInstance.addKeywordToGroup(
    workspaceId,
    googleAdsKeywordAddRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsKeywordAddRequest** | **GoogleAdsKeywordAddRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **analyzeNotAssignedKeywords**
> Completed analyzeNotAssignedKeywords(googleAdsAnalyzeKeywordsRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsAnalyzeKeywordsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsAnalyzeKeywordsRequest: GoogleAdsAnalyzeKeywordsRequest; //

const { status, data } = await apiInstance.analyzeNotAssignedKeywords(
    workspaceId,
    googleAdsAnalyzeKeywordsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsAnalyzeKeywordsRequest** | **GoogleAdsAnalyzeKeywordsRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **getGoogleAdsCampaigns**
> Array<GoogleAdsCampaignResponse> getGoogleAdsCampaigns(googleAdsCampaignsSearchRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsCampaignsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsCampaignsSearchRequest: GoogleAdsCampaignsSearchRequest; //

const { status, data } = await apiInstance.getGoogleAdsCampaigns(
    workspaceId,
    googleAdsCampaignsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCampaignsSearchRequest** | **GoogleAdsCampaignsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GoogleAdsCampaignResponse>**

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

# **getGoogleAdsCustomers**
> GoogleAdsCustomersResponse getGoogleAdsCustomers(googleAdsCustomersSearchRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsCustomersSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsCustomersSearchRequest: GoogleAdsCustomersSearchRequest; //

const { status, data } = await apiInstance.getGoogleAdsCustomers(
    workspaceId,
    googleAdsCustomersSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCustomersSearchRequest** | **GoogleAdsCustomersSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsCustomersResponse**

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

# **getGoogleAdsGroups**
> Array<GoogleAdsGroupResponse> getGoogleAdsGroups(googleAdsGroupsSearchRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsGroupsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsGroupsSearchRequest: GoogleAdsGroupsSearchRequest; //

const { status, data } = await apiInstance.getGoogleAdsGroups(
    workspaceId,
    googleAdsGroupsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsGroupsSearchRequest** | **GoogleAdsGroupsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GoogleAdsGroupResponse>**

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

# **getRecommendations**
> Array<GoogleAdsKeywordRecommendation> getRecommendations(googleAdsRecommendationsRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsRecommendationsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsRecommendationsRequest: GoogleAdsRecommendationsRequest; //

const { status, data } = await apiInstance.getRecommendations(
    workspaceId,
    googleAdsRecommendationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsRecommendationsRequest** | **GoogleAdsRecommendationsRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GoogleAdsKeywordRecommendation>**

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

# **importGoogleAdsCampaigns**
> GoogleAdsCampaignsResponse importGoogleAdsCampaigns(googleAdsCampaignsSearchRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsCampaignsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsCampaignsSearchRequest: GoogleAdsCampaignsSearchRequest; //

const { status, data } = await apiInstance.importGoogleAdsCampaigns(
    workspaceId,
    googleAdsCampaignsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCampaignsSearchRequest** | **GoogleAdsCampaignsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsCampaignsResponse**

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

# **importGoogleAdsCustomers**
> GoogleAdsCustomersResponse importGoogleAdsCustomers()


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.importGoogleAdsCustomers(
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsCustomersResponse**

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

# **importGoogleAdsGroups**
> GoogleAdsGroupsResponse importGoogleAdsGroups(googleAdsGroupsSearchRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsGroupsSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsGroupsSearchRequest: GoogleAdsGroupsSearchRequest; //

const { status, data } = await apiInstance.importGoogleAdsGroups(
    workspaceId,
    googleAdsGroupsSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsGroupsSearchRequest** | **GoogleAdsGroupsSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsGroupsResponse**

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

# **removeKeywordFromGroup**
> Completed removeKeywordFromGroup(googleAdsKeywordRemoveRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsKeywordRemoveRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let workspaceId: string; // (default to undefined)
let googleAdsKeywordRemoveRequest: GoogleAdsKeywordRemoveRequest; //

const { status, data } = await apiInstance.removeKeywordFromGroup(
    workspaceId,
    googleAdsKeywordRemoveRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsKeywordRemoveRequest** | **GoogleAdsKeywordRemoveRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

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

# **updateGoogleAdsCampaign**
> GoogleAdsCampaignResponse updateGoogleAdsCampaign(googleAdsCampaignUpdateRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsCampaignUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let googleAdsCampaignUpdateRequest: GoogleAdsCampaignUpdateRequest; //

const { status, data } = await apiInstance.updateGoogleAdsCampaign(
    customerId,
    campaignId,
    workspaceId,
    googleAdsCampaignUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCampaignUpdateRequest** | **GoogleAdsCampaignUpdateRequest**|  | |
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsCampaignResponse**

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

# **updateGoogleAdsCustomerUpdate**
> GoogleAdsCustomerResponse updateGoogleAdsCustomerUpdate(googleAdsCustomerUpdateRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsCustomerUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let customerId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let googleAdsCustomerUpdateRequest: GoogleAdsCustomerUpdateRequest; //

const { status, data } = await apiInstance.updateGoogleAdsCustomerUpdate(
    customerId,
    workspaceId,
    googleAdsCustomerUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCustomerUpdateRequest** | **GoogleAdsCustomerUpdateRequest**|  | |
| **customerId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsCustomerResponse**

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

# **updateGoogleAdsGroup**
> GoogleAdsGroupResponse updateGoogleAdsGroup(googleAdsGroupUpdateRequest)


### Example

```typescript
import {
    GoogleAdsApi,
    Configuration,
    GoogleAdsGroupUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new GoogleAdsApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let groupId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let googleAdsGroupUpdateRequest: GoogleAdsGroupUpdateRequest; //

const { status, data } = await apiInstance.updateGoogleAdsGroup(
    customerId,
    campaignId,
    groupId,
    workspaceId,
    googleAdsGroupUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsGroupUpdateRequest** | **GoogleAdsGroupUpdateRequest**|  | |
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
| **groupId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**GoogleAdsGroupResponse**

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

