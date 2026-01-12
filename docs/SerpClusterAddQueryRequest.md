# SerpClusterAddQueryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**post_back_url** | **string** |  | [optional] [default to undefined]
**queries** | [**Array&lt;SerpKeyword&gt;**](SerpKeyword.md) | List of queries | [default to undefined]
**customer_id** | **string** | Customer ID of cluster | [optional] [default to undefined]
**campaign_id** | **string** | Campaign ID of cluster | [optional] [default to undefined]
**group_id** | **string** | Group ID of cluster - will be generated if not provided | [optional] [default to undefined]
**group_name** | **string** | Group name of cluster | [optional] [default to '']

## Example

```typescript
import { SerpClusterAddQueryRequest } from 'flowhunt';

const instance: SerpClusterAddQueryRequest = {
    post_back_url,
    queries,
    customer_id,
    campaign_id,
    group_id,
    group_name,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
