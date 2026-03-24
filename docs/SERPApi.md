# SERPApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchClusterQuery**](#searchclusterquery) | **POST** /v2/serp/clusters/keywords | Search Cluster Query|
|[**serpClusterAddQueries**](#serpclusteraddqueries) | **POST** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id}/add_keywords | Serp Cluster Add Queries|
|[**serpClusterDeleteCampaign**](#serpclusterdeletecampaign) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id} | Serp Cluster Delete Campaign|
|[**serpClusterDeleteCustomer**](#serpclusterdeletecustomer) | **DELETE** /v2/serp/clusters/{customer_id} | Serp Cluster Delete Customer|
|[**serpClusterDeleteGroup**](#serpclusterdeletegroup) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id} | Serp Cluster Delete Group|
|[**serpClusterDeleteGroupQueries**](#serpclusterdeletegroupqueries) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id}/delete_queries | Serp Cluster Delete Group Queries|
|[**serpClusterGetGraphNodes**](#serpclustergetgraphnodes) | **POST** /v2/serp/clusters/graph_nodes | Serp Cluster Get Graph Nodes|
|[**serpClusterGetMatchingGroupsToQuery**](#serpclustergetmatchinggroupstoquery) | **POST** /v2/serp/clusters/recommended_groups | Serp Cluster Get Matching Groups To Query|
|[**serpClusterGetRelatedKeywordsToQuery**](#serpclustergetrelatedkeywordstoquery) | **POST** /v2/serp/clusters/related_keywords | Serp Cluster Get Related Keywords To Query|
|[**serpClusterSplitToSubClusters**](#serpclustersplittosubclusters) | **POST** /v2/serp/clusters/split_sub_clusters | Serp Cluster Split To Sub Clusters|
|[**serpSearch**](#serpsearch) | **POST** /v2/serp/serp/search | Serp Search|
|[**serpVolumes**](#serpvolumes) | **POST** /v2/serp/serp/volumes | Serp Volumes|
|[**serpVolumesPingback**](#serpvolumespingback) | **GET** /v2/serp/serp/volumes/pingback/{id}/{tag} | Serp Volumes Pingback|

# **searchClusterQuery**
> Array<SerpClusterKeywordResponse> searchClusterQuery(serpClusterGroupSearchRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterGroupSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpClusterGroupSearchRequest: SerpClusterGroupSearchRequest; //

const { status, data } = await apiInstance.searchClusterQuery(
    workspaceId,
    serpClusterGroupSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterGroupSearchRequest** | **SerpClusterGroupSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SerpClusterKeywordResponse>**

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

# **serpClusterAddQueries**
> Completed serpClusterAddQueries(serpClusterAddQueryRequests)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterAddQueryRequests
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let groupId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let serpClusterAddQueryRequests: SerpClusterAddQueryRequests; //

const { status, data } = await apiInstance.serpClusterAddQueries(
    customerId,
    campaignId,
    groupId,
    workspaceId,
    serpClusterAddQueryRequests
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterAddQueryRequests** | **SerpClusterAddQueryRequests**|  | |
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
| **groupId** | [**string**] |  | defaults to undefined|
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

# **serpClusterDeleteCampaign**
> Completed serpClusterDeleteCampaign()


### Example

```typescript
import {
    SERPApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.serpClusterDeleteCampaign(
    customerId,
    campaignId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
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

# **serpClusterDeleteCustomer**
> Completed serpClusterDeleteCustomer()


### Example

```typescript
import {
    SERPApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let customerId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.serpClusterDeleteCustomer(
    customerId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] |  | defaults to undefined|
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

# **serpClusterDeleteGroup**
> Completed serpClusterDeleteGroup()


### Example

```typescript
import {
    SERPApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let groupId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.serpClusterDeleteGroup(
    customerId,
    campaignId,
    groupId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
| **groupId** | [**string**] |  | defaults to undefined|
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

# **serpClusterDeleteGroupQueries**
> Completed serpClusterDeleteGroupQueries(serpQueryRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpQueryRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let customerId: string; // (default to undefined)
let campaignId: string; // (default to undefined)
let groupId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let serpQueryRequest: SerpQueryRequest; //

const { status, data } = await apiInstance.serpClusterDeleteGroupQueries(
    customerId,
    campaignId,
    groupId,
    workspaceId,
    serpQueryRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpQueryRequest** | **SerpQueryRequest**|  | |
| **customerId** | [**string**] |  | defaults to undefined|
| **campaignId** | [**string**] |  | defaults to undefined|
| **groupId** | [**string**] |  | defaults to undefined|
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

# **serpClusterGetGraphNodes**
> Array<SerpKeywordRelation> serpClusterGetGraphNodes(serpClusterGroupIntersectionsRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterGroupIntersectionsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpClusterGroupIntersectionsRequest: SerpClusterGroupIntersectionsRequest; //

const { status, data } = await apiInstance.serpClusterGetGraphNodes(
    workspaceId,
    serpClusterGroupIntersectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterGroupIntersectionsRequest** | **SerpClusterGroupIntersectionsRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SerpKeywordRelation>**

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

# **serpClusterGetMatchingGroupsToQuery**
> Array<SerpGroupIntersection> serpClusterGetMatchingGroupsToQuery(serpClusterBestGroupsRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterBestGroupsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpClusterBestGroupsRequest: SerpClusterBestGroupsRequest; //

const { status, data } = await apiInstance.serpClusterGetMatchingGroupsToQuery(
    workspaceId,
    serpClusterBestGroupsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterBestGroupsRequest** | **SerpClusterBestGroupsRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SerpGroupIntersection>**

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

# **serpClusterGetRelatedKeywordsToQuery**
> Array<SerpKeywordRelation> serpClusterGetRelatedKeywordsToQuery(serpClusterKeywordIntersectionsRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterKeywordIntersectionsRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpClusterKeywordIntersectionsRequest: SerpClusterKeywordIntersectionsRequest; //

const { status, data } = await apiInstance.serpClusterGetRelatedKeywordsToQuery(
    workspaceId,
    serpClusterKeywordIntersectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterKeywordIntersectionsRequest** | **SerpClusterKeywordIntersectionsRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SerpKeywordRelation>**

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

# **serpClusterSplitToSubClusters**
> Array<SerpSubclusterKeywordsResponse> serpClusterSplitToSubClusters(serpClusterGroupSubClustersRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpClusterGroupSubClustersRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpClusterGroupSubClustersRequest: SerpClusterGroupSubClustersRequest; //

const { status, data } = await apiInstance.serpClusterSplitToSubClusters(
    workspaceId,
    serpClusterGroupSubClustersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpClusterGroupSubClustersRequest** | **SerpClusterGroupSubClustersRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<SerpSubclusterKeywordsResponse>**

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

# **serpSearch**
> Array<TaskResponse> serpSearch(serpSearchRequests)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpSearchRequests
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpSearchRequests: SerpSearchRequests; //

const { status, data } = await apiInstance.serpSearch(
    workspaceId,
    serpSearchRequests
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpSearchRequests** | **SerpSearchRequests**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<TaskResponse>**

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

# **serpVolumes**
> TaskResponse serpVolumes(serpVolumeRequest)


### Example

```typescript
import {
    SERPApi,
    Configuration,
    SerpVolumeRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let workspaceId: string; // (default to undefined)
let serpVolumeRequest: SerpVolumeRequest; //

const { status, data } = await apiInstance.serpVolumes(
    workspaceId,
    serpVolumeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **serpVolumeRequest** | **SerpVolumeRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

# **serpVolumesPingback**
> TaskResponse serpVolumesPingback()


### Example

```typescript
import {
    SERPApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new SERPApi(configuration);

let id: string; // (default to undefined)
let tag: string; // (default to undefined)

const { status, data } = await apiInstance.serpVolumesPingback(
    id,
    tag
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **tag** | [**string**] |  | defaults to undefined|


### Return type

**TaskResponse**

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

