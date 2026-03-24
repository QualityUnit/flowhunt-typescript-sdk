# SerpClusterGroupSubClustersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** | Customer ID of cluster | [default to undefined]
**campaign_id** | **string** |  | [optional] [default to undefined]
**group_id** | **string** |  | [optional] [default to undefined]
**min_cluster_strength** | **number** |  | [optional] [default to undefined]
**suggest_other_matching_keywords** | **boolean** |  | [optional] [default to undefined]
**include_negative_keywords** | **boolean** |  | [optional] [default to undefined]
**include_all_members** | **boolean** |  | [optional] [default to undefined]
**include_group_keywords** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { SerpClusterGroupSubClustersRequest } from 'flowhunt';

const instance: SerpClusterGroupSubClustersRequest = {
    customer_id,
    campaign_id,
    group_id,
    min_cluster_strength,
    suggest_other_matching_keywords,
    include_negative_keywords,
    include_all_members,
    include_group_keywords,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
